# mypy issue reproducer

Instructions:

1. Create a virtual environment (`python3 -m virtualenv venv`)
2. Activate the virtual environment (`source venv/bin/activate`)
3. Install mypy and the demo module (`python3 -m pip install mypy src/`)
4. Run mypy on `t.py` (`mypy t.py`)


## Expected Output


```
t.py:3: note: Revealed type is "def () -> module.Optional"
```


## Actual Output

```
t.py:3: note: Revealed type is "typing._SpecialForm"
```
