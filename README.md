# bbl Scoop Bucket

[Scoop](https://scoop.sh) bucket for [bbl](https://github.com/nehemiaharchives/bbl), a command-line Bible reader and search tool.

## Install

```pwsh
scoop bucket add bbl https://github.com/nehemiaharchives/scoop-bucket
scoop install bbl/bbl
```

The `bbl` manifest installs the Windows x64 CLI and seeds the default local data directory with:

- `%USERPROFILE%\.bbl\packs\webus.zip`
- `%USERPROFILE%\.bbl\bin\bbl-search-common.exe`

This gives new users an out-of-the-box `webus` Bible pack and common search binary.

## Use

```pwsh
bbl --version
bbl john 3:16 in webus
bbl search love in webus
```

## Uninstall

```pwsh
scoop uninstall bbl
```

Uninstalling removes `%USERPROFILE%\.bbl`, including downloaded packs, search binaries, `config.json`, and `history.json`.

## Manifests

Current manifests:

- `bbl`: installs `bbl` v2.0 for Windows x64 from the official GitHub release.

