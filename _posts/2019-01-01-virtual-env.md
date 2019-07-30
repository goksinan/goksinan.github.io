---
title: "Creating a Virtual Environment"
date: 2019-05-23
tags: [Virtual environment, pip]
excerpt: "Creating a virtual environment and adding packages to eat"
category: "blog"
classes: wide
---

**(For macOS)**

---

### Create a virtual environment called ***venv*** using `venv` package
```python
python3 -m venv venv
```

### Activate the virtual environment
```python
source venv/bin/activate
```

### See the installed packages
```python
pip list
```

### Install a new package, e.g. numpy
```python
pip install numpy
```

### Deactivate the virtual environment
```python
deactivate
```

### Delete the virtual environment
```python
rm -rf venv/
```

### How to create a requirements.txt file?
```python
pip freeze > requirements.txt
```

### How to use requirements.txt file after creating a new environment?
```python
pip install -r requirements.txt
```

### How to make system packages available when creating a new environment?
```python
python3 -m venv venv --system-site-packages
source venv/bin/activate
```

### How to see the local packages that we installed? (Not the system packages we brought)
```python
pip list --local
```
