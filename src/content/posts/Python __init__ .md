---
title: Python __init__.py
published: 2025-03-07
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

## Bilibili

<iframe width="100%" height="468" src="//player.bilibili.com/player.html?bvid=BV1QA94YPEMK" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>

