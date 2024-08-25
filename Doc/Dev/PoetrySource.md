# Poetry Mirrors Source

## Command

```bash
poetry source add --priority=default mirrors https://pypi.tuna.tsinghua.edu.cn/simple/
```

## Toml

```toml
# pyproject.toml

[[tool.poetry.source]]
name = "mirrors"
url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
priority = "default"
```
