---
title: Python __init__
published: 2025-3-7
tags: [Python]
category: Python
draft: false
---

## Why we need to write __init__.py ?

When we import a module in main.py, they are under the same directory. The imported module will be executed intermediately. But if you want to import a package, it will only execute the **__init__.py** in the package. 

## So what should we put in the __init__.py?

- the initialization of the package : the environment variable, the logging, etc...
- the public interface to manage packages
- the package information

