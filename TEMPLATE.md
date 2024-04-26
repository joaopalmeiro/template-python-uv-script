# Template Notes

- Zed:
  - [EditorConfig](https://github.com/zed-industries/zed/issues/8534) issue
  - [Top-Ranking Issues (All Time)](https://github.com/zed-industries/zed/issues/5393) issue
  - https://zed.dev/docs/telemetry
  - https://zed.dev/docs/configuring-zed
  - https://github.com/zed-industries/zed/releases
  - Current global configuration: https://github.com/joaopalmeiro/dotfiles
- Ruff:
  - https://github.com/astral-sh/ruff/issues/809
  - https://github.com/astral-sh/ruff/discussions/3363
  - https://github.com/astral-sh/ruff/issues/1530
  - https://github.com/astral-sh/ruff/releases
  - [`docs`: remove `.` from check and format commands](https://github.com/astral-sh/ruff/pull/10217)
  - https://github.com/astral-sh/ruff?tab=readme-ov-file#usage
- uv:
  - https://github.com/astral-sh/uv?tab=readme-ov-file#python-discovery
  - https://github.com/astral-sh/uv/releases
  - https://github.com/astral-sh/uv/blob/0.1.17/PIP_COMPATIBILITY.md
  - `uv pip check`:
    - https://github.com/astral-sh/uv/blob/0.1.24/PIP_COMPATIBILITY.md
    - [Add `uv pip check`](https://github.com/astral-sh/uv/pull/2397)
    - https://github.com/astral-sh/uv/blob/0.1.24/PIP_COMPATIBILITY.md#pip-check
    - https://pip.pypa.io/en/stable/cli/pip_check/
- File nesting:
  - https://code.visualstudio.com/updates/v1_67#_explorer-file-nesting
  - https://github.com/antfu/vscode-file-nesting-config?tab=readme-ov-file#update-manually:
    - Example: `"Pipfile": ".editorconfig, .flake8, .isort.cfg, .python-version, Pipfile, Pipfile.lock, requirements*.in, requirements*.pip, requirements*.txt, tox.ini"`
  - https://code.visualstudio.com/docs/getstarted/settings#_default-settings:
    - Example: `"package.json": "package-lock.json, yarn.lock, pnpm-lock.yaml, bun.lockb"`
  - PyCharm also supports file nesting: https://www.jetbrains.com/help/pycharm/file-nesting-dialog.html
- mypy:
  - https://pypi.org/project/mypy/
  - https://github.com/python/mypy/blob/master/CHANGELOG.md#mypy-110
  - Config source:
    - https://github.com/pydantic/pydantic/blob/v2.6.3/docs/integrations/mypy.md#configuring-the-plugin
    - https://github.com/FlorianWilhelm/the-hatchlor/blob/v0.3/%7B%7Bcookiecutter.project_slug%7D%7D/pyproject.toml#L81
    - https://github.com/python/mypy/blob/1.9.0/docs/source/config_file.rst
    - https://github.com/python/mypy/blob/1.9.0/docs/source/config_file.rst#example-mypyini
    - https://github.com/python/mypy/blob/1.9.0/docs/source/existing_code.rst#introduce-stricter-options
    - https://github.com/python/mypy/blob/master/CHANGELOG.md#mypy-19

## Commands

```bash
zed ~/Documents/GitHub/template-python-uv-script/
```

```bash
uv --help
```

```bash
uv venv --help
```

```bash
uv pip install --help
```

```bash
uv pip list --help
```

```bash
which ruff
```

```bash
uv pip check --help
```

```bash
uv pip sync requirements.txt
```

```bash
uv pip sync --reinstall --refresh --strict requirements.txt
```
