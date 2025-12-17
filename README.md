[![Logo](https://patx.github.io/mongokv/logo.png)](https://patx.github.io/mongokv) is a tiny sync/async key-value store 
backed by PyMongo that provides a dead-simple Redis-like API (`set`, `get`, etc). Safe across threads, processes, and ASGI workers. 
[Read the API docs and user guide to get started](https://patx.github.io/mongokv).


### Usage

```
>>> from mongokv import Mkv

>>> db = Mkv('mongodb://localhost:27071')
>>> db.set('hello', {'name': 'world', 'status': 'green'})

>>> db.get('hello')
{'name': 'world', 'status': 'green'}
```


### Install

```
pip3 install mongokv
```

