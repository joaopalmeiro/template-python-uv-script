# template-python-uv-script

[![uv](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/uv/main/assets/badge/v0.json)](https://github.com/astral-sh/uv)
[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)

Opinionated [Python](https://www.python.org/) + [uv](https://github.com/astral-sh/uv) template for new scripts.

## Getting Started

1. Go to or create the project folder.
2. Get the template files:

```bash
npx degit github:joaopalmeiro/template-python-uv-script
```

or

```bash
npx degit github:joaopalmeiro/template-python-uv-script --force
```

3. Search for `template-python-uv-script` and replace it with the project name.
4. Search for `Opinionated [Python](https://www.python.org/) + [uv](https://github.com/astral-sh/uv) template for new scripts.` and replace it with the (short) project description.
5. Search for `João Palmeiro` and replace it with the author's name.
6. Open the [requirements.txt](requirements.txt) file and add the project-specific dependencies.
7. Delete the [TEMPLATE.md](TEMPLATE.md) file.
8. Delete the [`Getting Started`](#getting-started) section.

## Development

Install [pyenv](https://github.com/pyenv/pyenv) (if necessary).

```bash
pyenv install && pyenv versions
```

```bash
pip install uv==0.1.15 && uv --version
```

```bash
uv venv .venv
```

```bash
source .venv/bin/activate
```

```bash
which python && python --version
```

```bash
uv pip install -r requirements.txt
```

```bash
uv pip list --strict
```

```bash
ruff check .
```

```bash
ruff check --fix .
```

```bash
ruff format .
```

```bash
python 01.py
```

```bash
deactivate
```
