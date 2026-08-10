# gdb

Image with [gdb](https://www.sourceware.org/gdb) for attaching to processes running in other
containers.

Built from [Wolfi](https://github.com/wolfi-dev/os) rather than Alpine, because `gdb` has to call
functions inside the process it attaches to, and the targets are glibc processes.

## Usage

```bash
docker pull ghcr.io/hpedrorodrigues/gdb
```

Attaching to a process of another container requires sharing its process namespace and the
`SYS_PTRACE` capability. On Kubernetes, `kubectl debug --target` does both:

```bash
kubectl debug <pod> \
  --target <container> \
  --image ghcr.io/hpedrorodrigues/gdb \
  --profile sysadmin \
  --stdin --tty
```

Set the sysroot to the filesystem of the target **before** attaching, so the symbols of its own
libraries resolve, otherwise every call fails with `No symbol table is loaded`:

```bash
gdb -batch \
  -ex 'set confirm off' \
  -ex 'set sysroot /proc/<pid>/root' \
  -ex 'attach <pid>' \
  -ex 'print (int) malloc_trim(0)' \
  -ex detach
```
