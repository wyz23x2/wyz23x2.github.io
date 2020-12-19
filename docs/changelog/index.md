# Changelog
  
### 1.2.1
#### _Release date: 2020-12-12_
- Added ``relationlist.ver``.
- Deprecated ``generator(func=True)``. Use the new ``generator_func()`` instead.
- We switched to [a new license](../license).
  
### 1.1.1
#### _Release date: 2020-7-20_
- Fixed ``related()`` to use the new ``get_relation()`` instead of the old ``get_relate()``.
- Corrected ``get_relate()`` and ``get_relates()`` deprecation warning messages to show v1.4 instead of v1.2.
  
### 1.1.0
#### _Release date: 2020-7-19_
- ``repr()`` now returns something like ``RelationList(1, 2, 3)`` instead of the old ``([1, 2, 3], [], {1: 0, 2: 0, 3: 0})``.
- ``iter()`` now returns ``iter(value)`` instead of ``iter(elm)``. Programs that need to support older versions should simply switch to ``iter(elm)``.
- ``get_relate()`` is renamed to ``get_relation()``. The former is kept for backwards compatibility, but warns a DeprecationWarning and will be removed in v1.4.
- ``get_relates()`` is renamed to ``get_relations()``. The former is kept for backwards compatibility, but warns a DeprecationWarning and will be removed in v1.4.
- ``remove_relations()`` now returns a bool, ``False`` when error suppressed by ``err='ignore'``, ``True`` when no errors occured, to match ``delete()``.
- ``get_relations()`` now raises ``ValueError`` rather than ``KeyError`` to match other methods. Programs that need to support older versions should catch both.
  
### 1.0.0
#### _Release date: 2020-7-17_
First release.

[← Documentation](..)  
[← Home](/)
