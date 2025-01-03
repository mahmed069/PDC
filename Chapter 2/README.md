# Concurrency and Parallelism in Python

Python programs showcasing different aspects of concurrency, parallelism, and GPU computing.

## Table of Contents
1. [Multiprocessing and Multithreading](#multiprocessing-and-multithreading)
2. [Semaphore for Thread Synchronization](#semaphore-for-thread-synchronization)
3. [Vector Addition with ThreadPoolExecutor](#vector-addition-with-threadpoolexecutor)
4. [Calculating Fibonacci with Threads](#calculating-fibonacci-with-threads)
5. [GPU Computing with CUDA](#gpu-computing-with-cuda)
6. [Data Parallelism with NumPy](#data-parallelism-with-numpy)
7. [Thread Synchronization for Bank Transactions](#thread-synchronization-for-bank-transactions)
8. [MPI for Distributed Computing](#mpi-for-distributed-computing)
9. [Multiprocessing for Square and Cube Calculations](#multiprocessing-for-square-and-cube-calculations)
10. [Producer-Consumer Model with Multiprocessing](#producer-consumer-model-with-multiprocessing)

## Multiprocessing and Multithreading
### Code Overview:
- Demonstrates processing a large list using **multiprocessing** and **multithreading**.
- Compares execution times for both approaches.

### Key Concepts:
- `multiprocessing.Process`
- `threading.Thread`

### Example Usage:
```bash
python multiprocessing_and_multithreading.py
```

## Semaphore for Thread Synchronization
### Code Overview:
- Uses a **semaphore** to manage access to a shared resource.

### Key Concepts:
- `threading.Semaphore`

### Example Usage:
```bash
python semaphore_example.py
```

## Vector Addition with ThreadPoolExecutor
### Code Overview:
- Performs vector addition in parallel using `ThreadPoolExecutor`.

### Key Concepts:
- `concurrent.futures.ThreadPoolExecutor`
- Slicing arrays for parallel computation

### Example Usage:
```bash
python vector_add_threadpool.py
```

## Calculating Fibonacci with Threads
### Code Overview:
- Spawns multiple threads to compute Fibonacci numbers.

### Key Concepts:
- Recursive functions
- `threading.Thread`

### Example Usage:
```bash
python fibonacci_threads.py
```

## GPU Computing with CUDA
### Code Overview:
- Uses **Numba** and **CUDA** to perform parallel vector addition on the GPU.

### Key Concepts:
- `numba.cuda`
- Thread and block configurations

### Example Usage:
```bash
python gpu_vector_addition.py
```

## Data Parallelism with NumPy
### Code Overview:
- Performs vector addition using **NumPy** for efficient computation.

### Key Concepts:
- Array operations in NumPy

### Example Usage:
```bash
python numpy_parallelism.py
```

## Thread Synchronization for Bank Transactions
### Code Overview:
- Uses a lock to synchronize deposit and withdraw operations.

### Key Concepts:
- `threading.Lock`
- Critical sections

### Example Usage:
```bash
python bank_transactions.py
```

## MPI for Distributed Computing
### Code Overview:
- Demonstrates inter-process communication using **MPI** with `mpi4py`.

### Key Concepts:
- `MPI.COMM_WORLD`
- `comm.send` and `comm.recv`

### Example Usage:
```bash
mpiexec -n 2 python mpi_example.py
```

## Multiprocessing for Square and Cube Calculations
### Code Overview:
- Demonstrates multiprocessing to calculate squares and cubes of numbers.

### Key Concepts:
- `multiprocessing.Process`

### Example Usage:
```bash
python multiprocessing_calculations.py
```

## Producer-Consumer Model with Multiprocessing
### Code Overview:
- Implements a **producer-consumer** model using a shared queue.

### Key Concepts:
- `multiprocessing.Queue`
- `Process` for producer and consumer tasks

### Example Usage:
```bash
python producer_consumer.py
```

---

## Requirements
- Python 3.8+
- Libraries:
  - `NumPy`
  - `Numba`
  - `mpi4py`

## Installation
To install required dependencies:
```bash
pip install numpy numba mpi4py
```

## Notes
- Ensure you have CUDA installed for GPU-based examples.
- Use an MPI implementation (e.g., OpenMPI) for running MPI examples.

## License
This repository is licensed under the MIT License. Feel free to use and modify the code.



![image](https://github.com/user-attachments/assets/a3de4947-d933-4b97-b4b1-6fc5f9e23c24)

![image](https://github.com/user-attachments/assets/e5ee6406-d1eb-480c-8c32-dadc00a0c26c)

![image](https://github.com/user-attachments/assets/3aabe744-614f-4f15-b942-44de8a813032)

![image](https://github.com/user-attachments/assets/6e64fd62-4657-4a1f-8f85-5883b9cca0f4)

![image](https://github.com/user-attachments/assets/28d44586-724d-4888-9fab-103d2d51b6a7)

![image](https://github.com/user-attachments/assets/7b81d051-8f7e-4df1-8b57-8d427e7298cd)

