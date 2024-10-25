# brew-install

[![CI](https://github.com/gerlero/brew-install/actions/workflows/ci.yml/badge.svg)](https://github.com/gerlero/brew-install/actions/workflows/ci.yml)
[![Release](https://github.com/gerlero/brew-install/actions/workflows/update-tags.yml/badge.svg)](https://github.com/gerlero/brew-install/actions/workflows/update-tags.yml)

GitHub Action to install and cache Homebrew packages.

## Usage

```yaml
- uses: gerlero/brew-install@v1
  with:
    packages: python
```

## Inputs

### `packages`

**Required**. A formula or cask name or a whitespace-separated list of formula/cask names to install.

### `cache`

Whether to cache installed packages between runs. Default: `true`.

### `type`

The type of the packages to install. Possible values: `any`, `formula`, `cask`. Default: `any`.

## Related actions

- [`gerlero/apt-install`](https://github.com/gerlero/apt-install): GitHub Action to install and cache APT packages..
