# Datetime JSON

Serialize and deserialize datetime objects to and from JSON.

This package provides:

* 4 functions that wrap the `json` module:
    - `load/loads` - Deserialize a JSON string containing datetime objects
    - `dump/dumps` - Serialize python object containting datetime objects to JSON

* two classes that wrap derived from `json.JSONEncoder` and `json.JSONDecoder`:
    - `JSONEncoder` - Serialize a datetime object to JSON
    - `JSONDecoder` - Deserialize a JSON string to a datetime object

Usage:

```python
>>> from datetimejson import dumps, loads
>>> from datetime import datetime
>>> now = datetime.now()
>>> print(now)
2023-02-13 11:27:56.687439
>>> json_string = dumps(now)
>>> print(json_string)
{"__type__": "datetime", "year": 2023, "month": 2, "day": 13, "hour": 11, "minute": 27, "second": 56, "microsecond": 687439}
>>> print(loads(json_string))
2023-02-13 11:27:56.687439
>>> 
```
