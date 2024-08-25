# Poetry

## Basic

```bash
# 初始化项目
poetry init  

# 激活虚拟环境
poetry shell

# 安装pyproject.toml里或poetry.lock里列出来的包
poetry install

# 只安装生产用依赖
poetry install --no-dev

# 安装一个新的包
poetry add httpx

# 升级已安装的一个或多个包
poetry update httpx ipython

# 展示已安装的包
poetry show --tree

# 卸载已安装的包
poetry remove gunicorn

# 在不激活虚拟环境时执行命令
poetry run python manage.py runserver
```

## Import `requirements.txt`

```bash
cat requirements.txt|xargs poetry add
# or
poetry add `cat requirements.txt`
```

## Export `requirements.txt`

```bash
poetry export --output requirements.txt
# or
poetry export --with=dev --without-hashes -o dev_requirements.txt
```

## Ref

https://blog.csdn.net/jaket5219999/article/details/117556155
https://www.cnblogs.com/waketzheng/p/17142322.html
