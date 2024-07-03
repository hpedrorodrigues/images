# envsubst

Simple image containing only `sh` and [envsubst]. Useful for replacing environment variables in files.

## Usage

```bash
docker pull ghcr.io/hpedrorodrigues/envsubst
```

## Signature

Verify the signature of the image:

```bash
cosign verify ghcr.io/hpedrorodrigues/envsubst:<tag> \
  --certificate-oidc-issuer=https://token.actions.githubusercontent.com \
  --certificate-identity=https://github.com/hpedrorodrigues/images/.github/workflows/_shared_publish.yml@refs/heads/main
```

[envsubst]: https://www.gnu.org/software/gettext/manual/html_node/envsubst-Invocation.html
