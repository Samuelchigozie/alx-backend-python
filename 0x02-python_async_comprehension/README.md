# Async Comprehension

This repository contains tasks focused on utilizing asynchronous comprehensions in Python 3.

## Tasks Overview

### 0. Async Generator

[**0-async_generator.py**](0-async_generator.py) consists of an asynchronous coroutine called `async_generator`. This coroutine loops 10 times, asynchronously waiting for 1 second on each iteration, and then yields a random number between 0 and 10. The `random` module is used for generating random numbers.

### 1. Async Comprehensions

[**1-async_comprehension.py**](1-async_comprehension.py) is a script that imports `async_generator` from the previous task and defines a coroutine named `async_comprehension`. This coroutine collects 10 random numbers using an asynchronous comprehension over `async_generator` and then returns the list of 10 random numbers.

### 2. Run time for four parallel comprehensions

[**2-measure_runtime.py**](2-measure_runtime.py) contains a script that imports `async_comprehension` from the previous file and defines a coroutine named `measure_runtime`. This coroutine executes `async_comprehension` four times in parallel using `asyncio.gather` to measure the total runtime and return the result.

## Resources

- [PEP 530 – Asynchronous Comprehensions](https://intranet.alxswe.com/rltoken/hlwtED-iLsdORSgly8DsyQ)
- [What’s New in Python: Asynchronous Comprehensions / Generators](https://intranet.alxswe.com/rltoken/0OkbObYzCKtO7ZUAxfKvkw)
- [Type-hints for generators](https://intranet.alxswe.com/rltoken/l4Fnno568VbVIn9GvrFVtQ)