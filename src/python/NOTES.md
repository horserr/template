## Build target

The `target` option selects the build stage in `.devcontainer/Containerfile`:

- `uv` (default): `base` + [uv](https://docs.astral.sh/uv/)
- `pixi`: `base` + [pixi](https://pixi.sh/)
- `base`: plain `ghcr.io/horserr/base` image

Lifecycle scripts (`onCreate.sh` / `postCreate.sh`) are expected to be baked into
`ghcr.io/horserr/base` at `/usr/local/share/devcontainer/`.
