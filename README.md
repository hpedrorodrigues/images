# Reusable Images

- [envsubst](./envsubst)

## Development

### Useful commands

```bash
# build an image
task common:build -d <tool-name>

# load a tar into docker daemon
task common:load -d <tool-name>
```

### Reference

- [The apko File Format][apko_file]
- [OCI Image Format Specification / Annotations][image_spec_annotations]




[apko_file]: https://github.com/chainguard-dev/apko/blob/278d65cd558b9fd0225d072a1f3a2256e2cd85d7/docs/apko_file.md
[image_spec_annotations]: https://github.com/opencontainers/image-spec/blob/f5f87016de46439ccf91b5381cf76faaae2bc28f/annotations.md
