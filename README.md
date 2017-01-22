# ignore-node_modules

> Ignores node_modules directories from macOS Spotlight search

I got tired of Spotlight draining my battery and hogging my CPU.  It seems my node_modules were partly to blame.

This tells Spotlight to not index `node_modules` directories.  It does this by simply adding an empty file named `.metadata_never_index` in the top-most `node_modules` directory found while searching.

## Usage

Stop indexing all `node_modules` directories in your $HOME directory (recursively):

```bash
./ignore-node_modules
```

Stop indexing all `node_modules` directories found within another directory (recursively):

```bash
./ignore-node_modules ~/path/to/folder
```

## Install

1. Either [clone this repo](https://help.github.com/articles/cloning-a-repository/) or [download the zip file](archive/master.zip)
2. Add this to your $PATH

## License

MIT