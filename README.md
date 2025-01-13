# Website des Berliner-Rhetorik-Salons

## Install

### uv Python Project Management

... for Linux/macOS
``` console
$ curl -LsSf https://astral.sh/uv/install.sh | sh
```

... for Windows
``` console
> powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
```

### git

``` console
$ sudo apt install git
$ git clone git@github.com:veit/brs_site.git
```

### Initialise project

``` console
$ cd brs_site
$ uv sync

## Create docs
``` console
$ uv sync --extra docs
$ cd docs
$ uv run make html
```

## Create dev environment
``` console
$ uv sync --extra dev
```

### Open web browser

URL: file:///home/jordan/proj/sphinx-playground/_build/html/index.html
