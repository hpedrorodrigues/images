# Prettier

Simple image containing [prettier]. Useful for formatting files without the need to install/set up Nodejs.

## Usage

```bash
docker pull ghcr.io/hpedrorodrigues/prettier
```

## Signature

Verify the signature of the image:

```bash
cosign verify ghcr.io/hpedrorodrigues/prettier:<tag> \
  --certificate-oidc-issuer=https://token.actions.githubusercontent.com \
  --certificate-identity=https://github.com/hpedrorodrigues/images/.github/workflows/shared_publish.yml@refs/heads/main
```

[prettier]: https://prettier.io
