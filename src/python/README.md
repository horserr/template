
# Python with uv or pixi (python)

Choose between uv and pixi

## Options

| Options Id | Description | Type | Default Value |
|-----|-----|-----|-----|
| target | Containerfile build target (base = plain base image, uv = base + uv, pixi = base + pixi). | string | uv |

## Build target

The `target` option selects the build stage in `.devcontainer/Containerfile`:

- `uv` (default): `base` + [uv](https://docs.astral.sh/uv/)
- `pixi`: `base` + [pixi](https://pixi.sh/)
- `base`: plain `ghcr.io/horserr/base` image

Lifecycle scripts (`onCreate.sh` / `postCreate.sh`) are expected to be baked into
`ghcr.io/horserr/base` at `/usr/local/share/devcontainer/`.


---

_Note: This file was auto-generated from the [devcontainer-template.json](https://github.com/horserr/template/blob/main/src/python/devcontainer-template.json).  Add additional notes to a `NOTES.md`._
