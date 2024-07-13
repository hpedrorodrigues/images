# Hadolint

Simple image containing [hadolint]. Useful for linting Dockerfiles.

## Usage

```bash
docker pull ghcr.io/hpedrorodrigues/hadolint
```

## Signature

Verify the signature of the image:

```bash
cosign verify ghcr.io/hpedrorodrigues/hadolint:<tag> \
  --certificate-oidc-issuer=https://token.actions.githubusercontent.com \
  --certificate-identity=https://github.com/hpedrorodrigues/images/.github/workflows/_shared_publish.yml@refs/heads/main
```

[hadolint]: https://github.com/hadolint/hadolint
