# homebrew-narsil

The Homebrew tap for [narsil](https://github.com/AlexsJones/narsil), a persistent agent harness: a
daemon that runs your agents and a terminal UI that attaches to it.

```sh
brew install AlexsJones/narsil/narsil
narsil setup
```

macOS (Apple silicon and Intel) and Linux (x86_64 and arm64). It needs Homebrew 7.0.11 or newer
(`brew update`). If Homebrew asks you to trust the tap first:

```sh
brew trust --tap AlexsJones/narsil
```

To upgrade: `brew upgrade narsil`. To remove: `brew uninstall narsil && brew untap AlexsJones/narsil`.

The binaries are not signed with an Apple developer certificate. On macOS the cask clears the
quarantine flag on the one file it installs, so that it will run.

`Casks/narsil.rb` is written by [GoReleaser](https://goreleaser.com) each time a version of narsil is
released. Do not edit it by hand: change `.goreleaser.yaml` in the narsil repository instead.
