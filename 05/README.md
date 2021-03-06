## Exercise 5

### Problem

For this fifth exercise, we want to manipulate classes.

We would like to create a class `Runner` representing a runner.
```python
>>> from runner import Runner
>>> r = Runner('Sara', run_speed=20) # km/h
>>> r.run(distance=10)               # distance is km, result in hours
0.5

```

The `Runner` class should be able to handle:
* comparisons between runners (we must be able to compare runners with `runner_1 < runner_2`)
* a nice display (with `print runner`)

### Bonus

Write a unit test in a separate file `test.py`.

### Help

To compare objects with `<=` or `=>`, their classes must implement the `__lt__` and `___gt__` methods.

