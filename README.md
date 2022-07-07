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

### Installation

#### Archlinux

```console
pacman -S python-pre-commit python-poetry direnv
```

#### macOS

```console
brew install pre-commit poetry direnv
```

### Setup

Enter the project repo, then:

```console
$ direnv allow
[...]
$ pre-commit install --install-hooks
[...]
$ poetry install && poetry shell
$
```
