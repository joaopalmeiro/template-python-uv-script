# Notes

- https://github.com/joaopalmeiro/template-python-uv-script

## Commands

```bash
deactivate && uv venv .venv && source .venv/bin/activate && uv pip install -r requirements.txt --strict
```

```bash
uv venv .venv && source .venv/bin/activate && uv pip install -r requirements.txt --strict
```

```bash
echo "Cache directory:" && uv cache dir && \
echo "\nTool directory:" && uv tool dir && \
echo "\nPython directory:" && uv python dir
```

### Clean slate

```bash
rm -rf .mypy_cache/ .ruff_cache/ .venv/
```
