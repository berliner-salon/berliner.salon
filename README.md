# Website des Berliner Salons

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
$ git clone git@github.com:berliner-salon/berliner.salon.git
```

### Initialise project

``` console
$ cd berliner.salon
$ uv sync
```

## Create docs
``` console
$ uv sync --extra docs
$ uv run python -m sphinx -b html docs/ docs/_build/html/
```

## Create dev environment
``` console
$ uv sync --extra dev
```

### Open web browser

:sampl:`file:///{PATH/TO/PROJECT}/_build/html/index.html`

## Deployment

After ``git pull`` the page is built on GitHub Pages:
https://berliner-salon.github.io/berliner.salon/
