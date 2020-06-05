# Bug when install from path

```console
$ poetry --version
Poetry version 1.0.7

$ poetry install
Creating virtualenv foo-fgjGiKom-py3.8 in /Users/albert/Library/Caches/pypoetry/virtualenvs
Installing dependencies from lock file


Package operations: 1 install, 0 updates, 0 removals

  - Installing bar (0.1.0 deps/bar)

$ poetry run python
Python 3.8.0 (default, Oct 17 2019, 13:31:12)
[Clang 10.0.1 (clang-1001.0.46.4)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
(imported collections, datetime, functools, itertools, math, os, pprint, re, sys, time)
>>> import bar
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ModuleNotFoundError: No module named 'bar'
>>>

```
