# ShellCheck

Simple image wrapping [shellcheck] (a static analysis tool for shell scripts).

## Usage

```bash
docker pull ghcr.io/hpedrorodrigues/shellcheck
```

## Signature

Verify the signature of the image:

```bash
cosign verify ghcr.io/hpedrorodrigues/shellcheck:<tag> \
  --certificate-oidc-issuer=https://token.actions.githubusercontent.com \
  --certificate-identity=https://github.com/hpedrorodrigues/images/.github/workflows/shared_publish.yml@refs/heads/main
```

[shellcheck]: https://www.shellcheck.net
