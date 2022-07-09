# dickbag.org

<!-- mdformat-toc start --slug=github --no-anchors --maxlevel=3 --minlevel=1 -->

- [dickbag.org](#dickbagorg)
  - [Development dependencies](#development-dependencies)
    - [Installation](#installation)
    - [Setup](#setup)

<!-- mdformat-toc end -->

If you don't know what this is, you probably shouldn't be here.

## Development dependencies

You need some stuff to work on this.

- [pre-commit](https://pre-commit.com/) installs and manages git hooks to help prevent you from
  committing garbage to the repo.
- [poetry](https://python-poetry.org/) is a python dependency resolver and virtual environment manager.
- [direnv](https://direnv.net/) allows directory-specific env var configuration.
- [pyenv](https://github.com/pyenv/pyenv) manages python versions and lets us switch interpreters without
  being chained to the crusty, out of date debian repos or whatever.

### Installation

#### Archlinux

```console
pacman -S python-pre-commit python-poetry direnv pyenv
```

#### macOS

```console
brew install pre-commit poetry direnv pyenv
```

### Setup

Enter the project repo, then:

```console
$ pyenv install
[...]
$ direnv allow
[...]
$ pre-commit install --install-hooks
[...]
$ poetry install && poetry shell
$
```
