# Snippets

## `ruff.toml` file

```toml
# Minimal:
# https://docs.astral.sh/ruff/settings/#lint_extend-select
# https://docs.astral.sh/ruff/rules/#isort-i
# extend-select = ["I"]
```

## `.vscode/settings.json` file

```json
{
  "explorer.fileNesting.enabled": true,
  "explorer.fileNesting.expand": true,
  "explorer.fileNesting.patterns": {
    "README.md": "NOTES.md, TEMPLATE.md",
    "requirements.txt": ".python-version, mypy.ini, ruff.toml"
  }
}
```

```markdown
7. Remove `, TEMPLATE.md` from the `README.md` file nesting pattern in the [.vscode/settings.json](.vscode/settings.json) file.
```

## `pyproject.toml` file

```toml
[project]
name = "template-python-uv-script"
version = "0.0.0"
requires-python = ">=3.10"
dependencies = []

[dependency-groups]
dev = ["mypy==1.12.0", "ruff==0.6.9"]

[tool.uv]
package = false
python-downloads = "manual"
python-preference = "only-managed"
```
