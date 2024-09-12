# OCI Images

- [debug](./debug)
- [envsubst](./envsubst)
- [hadolint](./hadolint)
- [prettier](./prettier)
- [shellcheck](./shellcheck)
- [shfmt](./shfmt)
- [tf](./tf)
- [tools](./tools)

## Development

This project uses [task](https://taskfile.dev) to manage the build process on local environments.

Feel free to take a look at the [Taskfile.yaml](./Taskfile.yaml) to see the available tasks.

## Signature

Verify the signature of an image:

<details>
<summary>example</summary>

```bash
cosign verify ghcr.io/hpedrorodrigues/<tool>:<tag> \
  --certificate-oidc-issuer=https://token.actions.githubusercontent.com \
  --certificate-identity=https://github.com/hpedrorodrigues/images/.github/workflows/_shared_publish.yml@refs/heads/main
```

</details>

## Reference

- [SLSA specification](https://slsa.dev)
- [Sigstore docs](https://docs.sigstore.dev)
- [apko docs](https://github.com/chainguard-dev/apko/tree/4389ab6f93a7eabb4eb2a9d137ae291349095a04/docs)
- [melange docs](https://github.com/chainguard-dev/melange/tree/e855ba4a69a3256aa04754dd96906f222d88cbbd/docs)
- [OCI Image Format Specification](https://github.com/opencontainers/image-spec/blob/036563a4a268d7c08b51a08f05a02a0fe74c7268/spec.md)
