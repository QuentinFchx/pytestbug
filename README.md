Reproduction case for https://github.com/microsoft/vscode-python/issues/21705

1. Create a virtual env with the following dependencies

```
mkvirtualenv pytestbug
pip install pytest
pip install pytest-describe
```

2. Open the project in VSCode

3. Install/Enable the vscode-python extension (ms-python.python) and set the virtualenv to `pytestbug` (or whatever you configured above)

4. Discover tests -> You should only see 2 tests instead of 4 (cf. underlying issue linked at the top of the file).
