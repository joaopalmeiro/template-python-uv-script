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
