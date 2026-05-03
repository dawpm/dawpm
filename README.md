# dawpm

A package manager for DAW plugins.

`dawpm` lets you install free and open-source plugins (VST, VST3) for FL Studio with one command, instead of clicking through download pages, unzipping, and copying DLLs into the right folder by hand.

```bash
npm i -g @dawpm/cli
dawpm install @dsk/overture
```

## Repos

- [`dawpm/core`](https://github.com/dawpm/core): schemas, registry client, installer, DAW adapters
- [`dawpm/cli`](https://github.com/dawpm/cli): the `dawpm` command-line tool
- [`dawpm/registry`](https://github.com/dawpm/registry): the Next.js registry frontend
- [`dawpm/registry-data`](https://github.com/dawpm/registry-data): the source-of-truth plugin data

## Adding a plugin

Open a PR on the registry data repo with a `src/plugins/<ns>/<name>/index.yaml` file. The registry rebuilds and redeploys automatically on merge.
