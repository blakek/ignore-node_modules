# ignore-node_modules

> Ignores node_modules directories from macOS Spotlight search

I got tired of Spotlight draining battery and CPU. It seems `node_modules` were
partly to blame.

This script signals Spotlight to not index `node_modules` directories.

It works by adding an empty file named `.metadata_never_index` in the top-most
`node_modules` directory found while searching.

## Usage

Stop indexing all `node_modules` directories in your current directory
(recursively):

```bash
./ignore-node_modules
```

Stop indexing all `node_modules` directories found within another directory
(recursively):

```bash
./ignore-node_modules /path/to/folder
```

## Install

You can install using [Homebrew](https://brew.sh/) or manually build from
source:

### Install with Homebrew

Running this in your terminal adds [my
tap](https://github.com/blakek/homebrew-blakek) and installs the package:

```bash
brew tap blakek/blakek && brew install blakek/blakek/ignore-node_modules
```

### Build from Source

1. Either [clone this
   repo](https://help.github.com/articles/cloning-a-repository/) or [download
   the zip
   file](https://github.com/blakek/ignore-node_modules/archive/master.zip)
2. Add `ignore-node_modules` to your \$PATH (e.g. `/usr/local/bin`)
3. Make sure file permissions allow execution (e.g. `chmod +x ignore-node_modules`). This shouldn't be necessary when cloning, but is
   likely when downloading from a browser.

## License

MIT
