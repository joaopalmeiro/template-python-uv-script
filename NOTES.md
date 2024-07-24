# Notes

- https://github.com/joaopalmeiro/template-python-uv-script

## Commands

```bash
pip config unset global.require-virtualenv
```

```bash
rm -rf .venv/ .mypy_cache/ .ruff_cache/
```

```bash
deactivate && uv venv .venv && source .venv/bin/activate && uv pip install -r requirements.txt
```

```bash
uv venv .venv && source .venv/bin/activate && uv pip install -r requirements.txt
```

### Clean slate

```bash
rm -rf .mypy_cache/ .ruff_cache/ .venv/
```
