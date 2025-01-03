# Python Asynchronous Programming and Multithreading Examples

This repository contains examples demonstrating the use of Python's `asyncio` library, `concurrent.futures`, and threading concepts. These scripts explore asynchronous tasks, coroutines, thread pools, process pools, and finite state machines.

---

## Table of Contents

1. [Asyncio Coroutine Examples](#1-asyncio-coroutine-examples)
   - [Basic Coroutines](#basic-coroutines)
   - [Finite State Machine](#finite-state-machine)
   - [Parallel Computation with Asyncio](#parallel-computation-with-asyncio)
2. [Multithreading and Multiprocessing](#2-multithreading-and-multiprocessing)
   - [Thread Pool Executor](#thread-pool-executor)
   - [Process Pool Executor](#process-pool-executor)
3. [Requirements](#4-requirements)
4. [License](#5-license)

---

## 1. Asyncio Coroutine Examples

### Basic Coroutines

**File**: `basic_coroutines.py`  
**Description**: Demonstrates coroutine functions to compute:
- The sum of integers up to a given number.
- The factorial of a number.

Key Features:
- Uses `asyncio.Future` and `asyncio.sleep`.
- Displays results when computations are complete.

---

### Finite State Machine

**File**: `finite_state_machine.py`  
**Description**: Simulates a finite state machine using coroutines.

Key Features:
- Randomly transitions between states (`state1`, `state2`, `state3`).
- Ends at a specific state with computed results.

---

### Parallel Computation with Asyncio

**File**: `asyncio_tasks.py`  
**Description**: Executes multiple tasks in parallel using `asyncio`.

Key Features:
- Computes factorials, Fibonacci numbers, and binomial coefficients.
- Tasks run concurrently with simulated delays.

---

## 2. Multithreading and Multiprocessing

### Thread Pool Executor

**File**: `thread_pool.py`  
**Description**: Demonstrates multithreading using `ThreadPoolExecutor`.

Key Features:
- Computes cubes of numbers.
- Maps tasks to a thread pool for concurrent execution.
- Efficient for I/O-bound tasks.

---

### Process Pool Executor

**File**: `process_pool.py`  
**Description**: Uses `ProcessPoolExecutor` for heavy computations.

Key Features:
- Computes results for a large list of numbers.
- Compares sequential, thread pool, and process pool executions.

---




## 3. Requirements

    Python 3.x
    Libraries:
        asyncio
        concurrent.futures
        random
        time

## 4. License

This project is licensed under the MIT License. See the LICENSE file for details.


![image](https://github.com/user-attachments/assets/c6a57d39-da1c-4511-a9b0-96c806c28ac6)

![image](https://github.com/user-attachments/assets/fd6481ce-d029-4251-8ff3-04467b122569)

![image](https://github.com/user-attachments/assets/03a243f9-aa2f-40ff-8b18-793408a05664)

![image](https://github.com/user-attachments/assets/473eb959-75b9-4327-9641-f3383182dcc0)

![image](https://github.com/user-attachments/assets/58d3f9c4-c0c1-4a78-aab6-bcda995fb898)

![image](https://github.com/user-attachments/assets/69f76627-74bd-4df8-884b-8cd2729aea81)

