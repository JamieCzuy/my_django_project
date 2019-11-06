# Step #2 - Create the Virtual Environment

1. From in the root folder of the repo run:
```bash
python -m venv venv 
```

2. Activate the virtual environment:
```bash
source ./venv/bin/activate
```

You should see the prompt change, it should now be prepended with `(venv)`

3. Verify using python from the virtual environment:
```bash
which python
```

Output should be something like:
```bash
/Users/<user_id>/projects/<project_name>/venv/bin/python
```

For me it was:
```bash
/Users/jamie/projects/my_django_project/venv/bin/python
```

4. Check pip
```bash
pip list
```

Output should be something like:
```bash
Package    Version
---------- -------
pip        19.2.3 
setuptools 41.2.0 
WARNING: You are using pip version 19.2.3, however version 19.3.1 is available.
You should consider upgrading via the 'pip install --upgrade pip' command.
```

5. Update pip and setuptools:
```bash
pip install --upgrade pip setuptools
```

Output:
```bash
Collecting pip
  Using cached https://files.pythonhosted.org/packages/00/b6/9cfa56b4081ad13874b0c6f96af8ce16cfbc1cb06bedf8e9164ce5551ec1/pip-19.3.1-py2.py3-none-any.whl
Collecting setuptools
  Using cached https://files.pythonhosted.org/packages/d9/de/554b6310ac87c5b921bc45634b07b11394fe63bc4cb5176f5240addf18ab/setuptools-41.6.0-py2.py3-none-any.whl
Installing collected packages: pip, setuptools
  Found existing installation: pip 19.2.3
    Uninstalling pip-19.2.3:
      Successfully uninstalled pip-19.2.3
  Found existing installation: setuptools 41.2.0
    Uninstalling setuptools-41.2.0:
      Successfully uninstalled setuptools-41.2.0
Successfully installed pip-19.3.1 setuptools-41.6.0
```

6. Verify update
```bash
pip list
```

Output
```bash
Package    Version
---------- -------
pip        19.3.1 
setuptools 41.6.0 
```

7. Create `.gitignore` file to ignore `venv` folder:
Using your editor create `.gitignore` with contents:
```
# Ignore these Folders:
tmp/
venv/

# Ignore these Files:
.DS_Store
 ```