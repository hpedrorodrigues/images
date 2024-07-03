# debug

Image with tools for debugging and troubleshooting network issues.

## Usage

```bash
docker pull ghcr.io/hpedrorodrigues/debug
```

## Signature

Verify the signature of the image:

```bash
cosign verify ghcr.io/hpedrorodrigues/debug:<tag> \
  --certificate-oidc-issuer=https://token.actions.githubusercontent.com \
  --certificate-identity=https://github.com/hpedrorodrigues/images/.github/workflows/_shared_publish.yml@refs/heads/main
```
