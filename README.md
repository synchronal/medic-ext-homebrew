# Medic Hombrew

An extension pack for using [medic](https://github.com/synchronal/medic-rs)
with homebrew.

## Installation

```shell
brew tap synchronal/tap
brew install medic-ext-hombrew
```

Example `Brewfile`:

```shell
tap 'synchronal/tap'

brew  'synchronal/tap/medic'
brew  'synchronal/tap/medic-ext-homebrew'
```

## Usage

```toml
[doctor]

checks = [
  { check = "homebrew" },
]
```


# medic-check-homebrew

Checks for whether a hombrew Brewfile is present, and whether all packages
it declares are up to date.


```shell
medic-check-hombrew
medic-check-homebrew --cd <path>
```
