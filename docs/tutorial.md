---
permalink: /docs/tutorial.html
---
# Relationlist Tutorial
  
## <a id="install">Installation</a>
``relationlist`` is published on [PyPI](https://pypi.org/project/relationlist/). It requires Python >=3.8. Install it by:   
(Note: replace ``py -3`` with ``python3`` on macOS/Unix/Linux)  
``py -3 -m pip install --user relationlist``  
To install the newest review version:  
``py -3 -m pip install --pre --user relationlist``  
Now test:
```python
>>> import relationlist
>>> relationlist.ver.raw  # May be different if downloaded with --pre
'1.2.1'
>>> # You're ready to use relationlist!
```
## <a id="impinit">Import and Initialize</a>
Import relationlist like this:
```python
>>> import relationlist
```
If you want to reduce typing, type this:
```python
>>> import relationlist as rl  # "rl" is easy and avoids conflict with "import random as r"
```
Now create a ``RelationList`` object. It has only one parameter, default ``()``, like ``list()``, ``tuple()`` eg..
```python
>>> rlis = rl.RelationList([1, 2, 3])
```
You can check the value and print it.
```python
>>> rlis.value
[1, 2, 3]
>>> print(rlis)
[1, 2, 3]
>>> rlis
RelationList(1, 2, 3)
```
Congratulations, you have successfully created a ``RelationList``!
## <a id="adddelete">Adding and Deleting</a>
  
<!--[&emsp;&nbsp;API Reference →](apiref.html)  -->
[← Documentation](index.html)  
[← Home](/)
