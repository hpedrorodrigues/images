# debug

Image with tools for debugging and troubleshooting.

## Usage

```bash
docker pull ghcr.io/hpedrorodrigues/debug
```

## Signature

Verify the signature of the image:

```bash
cosign verify ghcr.io/hpedrorodrigues/debug:<tag> \
  --certificate-oidc-issuer=https://token.actions.githubusercontent.com \
  --certificate-identity=https://github.com/hpedrorodrigues/images/.github/workflows/publish.yml@refs/heads/main
```
