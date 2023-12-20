# Async

This repository consists of tasks designed to teach and implement asynchronous code in Python 3.

## Tasks Overview

### 0. The basics of async

[**0-basic_async_syntax.py**](0-basic_async_syntax.py) contains an asynchronous coroutine named `wait_random` that takes an integer argument `max_delay` (default value of 10) and waits for a random delay between 0 and `max_delay` seconds (float value). The `random` module is used.

### 1. Let's execute multiple coroutines at the same time with async

[**1-concurrent_coroutines.py**](1-concurrent_coroutines.py) is a script that imports `wait_random` from the previous file and implements an asynchronous routine named `wait_n`. This routine takes two integer arguments (`n` and `max_delay`) and spawns `wait_random` `n` times with the specified `max_delay`. The function returns a list of all the delays in ascending order without using `sort()` due to concurrency.

### 2. Measure the runtime

[**2-measure_runtime.py**](2-measure_runtime.py) contains a script that imports `wait_n` from the previous file and creates a function named `measure_time`. This function takes two integer arguments (`n` and `max_delay`), measures the total execution time for `wait_n(n, max_delay)`, and returns `total_time / n`. The `time` module is used to measure an approximate elapsed time.

### 3. Tasks

[**3-tasks.py**](3-tasks.py) is a script that imports `wait_random` from [0-basic_async_syntax](0-basic_async_syntax) and defines a regular function (not an async function) named `task_wait_random`. This function takes an integer `max_delay` and returns an `asyncio.Task`.

### 4. Tasks

[**4-tasks.py**](4-tasks.py) is a script that takes the code from `wait_n` and modifies it into a new function named `task_wait_n`. The code is almost identical to `wait_n`, except that `task_wait_random` is being called.

## Resources

- [Async IO in Python: A Complete Walkthrough](https://intranet.alxswe.com/rltoken/zYkXScziW1D5rNdNEvObjQ)
- [asyncio - Asynchronous I/O](https://intranet.alxswe.com/rltoken/aZUO4GiWHbPIrVBIwptFAw)
- [random.uniform](https://intranet.alxswe.com/rltoken/72mVf1s8rx2ih_U2WjBmaA)