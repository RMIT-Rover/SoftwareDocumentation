# Sofware Documentation

Requires Python3

After cloning and changing directory to folder.

```
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

Serve local dev version of documentation on localhost:8000
```
mkdocs serve
```

```
mkdocs build
ghp-import site
```