# Python 2 to Python 3.6+ Conversion Report

## Files Converted

- `ConfigReport.py`
- `ConfigUtils.py`
- `ConfigDump.py`
- `WAuJ_utilities.py`

## Changes Made

| Change | Files |
|---|---|
| `print 'x'` → `print('x')` | All 4 files |
| `True=1` / `False=0` removed | `ConfigReport.py`, `ConfigUtils.py`, `ConfigDump.py` |
| `dict.has_key(k)` → `k in dict` | `ConfigUtils.py`, `WAuJ_utilities.py` |
| `except X, e:` → `except X as e:` | `WAuJ_utilities.py` |
| `dict.keys()[0]` → `list(dict.keys())[0]` | `ConfigUtils.py`, `WAuJ_utilities.py` |
| `keys = d.keys(); keys.pop()` → `keys = list(d.keys()); keys.pop()` | `ConfigUtils.py` |
| `names = d.keys(); names.sort()` → `names = sorted(d.keys())` | `WAuJ_utilities.py` |
| `` `value` `` → `repr(value)` | `WAuJ_utilities.py` |
| `cmp()` sort lambda → `key=` parameter | `WAuJ_utilities.py` |
| `raise X, msg` → `raise X(msg)` | `WAuJ_utilities.py` |
| `tarfile.readline()` bytes → decoded string | `ConfigUtils.py` |
| Multi-line triple-quoted `print` statements fixed | `WAuJ_utilities.py` |
