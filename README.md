# Skylands Homebrew Tap

The Homebrew cask for [Skylands](https://skylands.ai), for macOS and Linux.

## Install

```sh
brew tap skylands-ai/tap
brew trust skylands-ai/tap
brew install --cask skylands
```

Homebrew won't load a cask from a third-party tap until you've trusted the tap.

## Upgrade and Uninstall

```sh
brew upgrade
brew uninstall --cask skylands
```

A service from `skylands daemon install` or `skylands devworld install` follows upgrades and uninstalls on its own. See [Run as a Service](https://docs.skylands.ai/operations/service/).

## The Cask

Each Skylands release writes `Casks/skylands.rb` and commits it here, so changes made to it by hand are overwritten. Change the cask in the `homebrew_casks` section of [`.goreleaser.yaml`](https://github.com/skylands-ai/skylands/blob/main/.goreleaser.yaml) in the Skylands repository.

For everything else, see the [Skylands documentation](https://docs.skylands.ai).
