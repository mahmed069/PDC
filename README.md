# Parallel and Distributed Computing with Python: Examples and Concepts

This repository showcases Python scripts and examples covering **parallel computing**, **distributed systems**, and **asynchronous programming** using libraries such as `asyncio`, `mpi4py`, and `concurrent.futures`.

---

## Table of Contents

1. [Introduction](#1-introduction)
2. [Parallel and Distributed Computing](#2-parallel-and-distributed-computing)
   - [Parallel Computing](#parallel-computing)
   - [Distributed Computing](#distributed-computing)
3. [Examples in This Repository](#3-examples-in-this-repository)
4. [How to Run the Examples](#4-how-to-run-the-examples)
5. [Requirements](#5-requirements)
6. [License](#6-license)

---

## 1. Introduction

Modern applications often require high performance and scalability to process large datasets or execute complex computations. **Parallel computing** and **distributed computing** are two strategies to improve efficiency by dividing work among multiple processors, cores, or machines.

This repository provides hands-on examples for learning and experimenting with parallel and distributed systems in Python. Concepts like MPI, thread pools, process pools, and asynchronous coroutines are demonstrated.

---

## 2. Parallel and Distributed Computing

### Parallel Computing

Parallel computing focuses on executing multiple tasks simultaneously on multiple cores or threads of a single machine. This can be achieved through:

- **Multithreading**: Multiple threads share the same memory space.
- **Multiprocessing**: Processes run independently with separate memory space.

Key libraries in Python:
- `concurrent.futures`
- `threading`
- `multiprocessing`

**Example**: Computing the factorials and cubes of numbers concurrently using a thread pool or process pool.

---

### Distributed Computing

Distributed computing extends parallelism to multiple machines, often interconnected over a network. Each machine processes a subset of tasks and communicates via a protocol like MPI (Message Passing Interface).

Key library in Python:
- `mpi4py`

**Example**: Sending and receiving data across processes using MPI to simulate distributed tasks.

---

## 3. Examples in This Repository

### Message Passing Interface (MPI)

**Files**: 
- `mpi_send_recv.py`
- `mpi_scatter_gather.py`

**Description**: Demonstrates how to use the `mpi4py` library to:
- Send and receive data between processes.
- Broadcast and scatter data across multiple processes.

---

### Asynchronous Programming

**Files**: 
- `asyncio_coroutines.py`
- `asyncio_tasks.py`
- `finite_state_machine.py`

**Description**: Uses Python's `asyncio` library to:
- Compute sums, factorials, and Fibonacci numbers asynchronously.
- Simulate a finite state machine using coroutines.
- Manage parallel execution of tasks with delays.

---

### Threading and Multiprocessing

**Files**: 
- `thread_pool.py`
- `process_pool.py`

**Description**: Demonstrates the difference between thread pools and process pools for concurrent execution.

Key Features:
- Compute cubes of numbers.
- Compare sequential, multithreaded, and multiprocessed execution times.

---

### Mixed Examples

**File**: `event_loop_tasks.py`

**Description**: Demonstrates task scheduling using an event loop, where tasks call each other in a cyclic manner until a condition is met.

---

## 4. How to Run the Examples

1. Install Python 3.x and required libraries:
   ```bash
   pip install mpi4py


## Python 3.x
Libraries:

    asyncio
    mpi4py
    concurrent.futures
    time
    random

## 6. License

This project is licensed under the MIT License. See the LICENSE file for details.
Author

Created by Your Name. Contributions and feedback are welcome!
Key Concepts in Parallel and Distributed Computing
Parallel Computing

Parallel computing involves splitting a task into smaller subtasks and running them simultaneously. It is commonly used in:

    Image and video processing
    Machine learning and AI
    Scientific simulations

## Distributed Computing

Distributed computing involves coordinating tasks across multiple machines. It is used for:

    Large-scale data processing (e.g., Hadoop, Spark)
    Cloud computing and microservices
    High-performance simulations
