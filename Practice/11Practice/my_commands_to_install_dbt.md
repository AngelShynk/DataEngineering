
### Suggested commands to install and run DBT for Mac OS.

**uv** - is a fast Python package and environment manager written in Rust. It replaces common tools such as pip, virtualenv, pip-tools, and parts of poetry.
More info about uv - https://docs.astral.sh/uv/.

```
python -m venv venv
source venv/bin/activate
python --version
python -m pip install --upgrade pip
pip install uv
uv pip install -r requirements.txt
dbt build
dbt docs generate
dbt docs serve
dbt docs serve --port 8081
```
