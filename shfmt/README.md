# shfmt

Simple image wrapping [shfmt] (a shell formatter).

## Usage

```bash
docker pull ghcr.io/hpedrorodrigues/shfmt
```

## Signature

Verify the signature of the image:

```bash
cosign verify ghcr.io/hpedrorodrigues/shfmt:<tag> \
  --certificate-oidc-issuer=https://token.actions.githubusercontent.com \
  --certificate-identity=https://github.com/hpedrorodrigues/images/.github/workflows/shared_publish.yml@refs/heads/main
```

[shfmt]: https://github.com/mvdan/sh
