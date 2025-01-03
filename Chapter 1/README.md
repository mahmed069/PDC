# Python Code Examples with Multithreading, Multiprocessing, and GPU Computing

This repository contains advanced Python examples that demonstrate the use of threading, multiprocessing, and GPU computations for performance optimization and concurrent programming.

## Features

### 1. GPU Vector Addition
This example showcases GPU computing using Numba's CUDA capabilities. A simple vector addition operation is performed on the GPU.

- **Modules Used**: `NumPy`, `Numba` (CUDA support)
- **Key Function**:
  - `vector_add(a, b, c)`: Performs element-wise addition of two arrays on the GPU.
- **Steps**:
  1. Initialize random input arrays.
  2. Configure grid and block dimensions.
  3. Perform GPU computation.

### 2. ThreadPoolExecutor vs. Threading
Compares execution time between `ThreadPoolExecutor` and the traditional `threading` library for running simple tasks concurrently.

- **Tasks**:
  - `task_1()`: Prints "Task 1 executed".
  - `task_2()`: Prints "Task 2 executed".
- **Metrics**: Measures and compares execution times.

### 3. Fibonacci Calculation with Threads
Calculates Fibonacci numbers using multiple threads to demonstrate the performance of threading in computationally intensive tasks.

- **Key Function**:
  - `calc_fibonacci(n)`: Recursively calculates the nth Fibonacci number.
- **Metrics**: Measures execution time for 4 and 9 threads.

### 4. Multiprocessing vs. Multithreading for List Operations
Compares the performance of multiprocessing and multithreading for large-scale list operations.

- **Key Function**:
  - `do_something(size, out_list)`: Appends the sum of indices to a list.
- **Metrics**: Measures and compares execution times.

### 5. Thread-Safe Bank Transactions
Simulates bank transactions (deposit and withdrawal) with thread-safe operations using `threading.Lock`.

- **Key Functions**:
  - `deposit(amount)`: Adds the specified amount to the balance.
  - `withdraw(amount)`: Subtracts the specified amount from the balance.
- **Metrics**: Tracks execution time for each transaction and overall.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/mahmed069/python-concurrency-.git
   ```

2. Navigate to the project directory:
   ```bash
   cd python-concurrency
   ```

3. Run each Python script:
   ```bash
   python <script_name>.py
   ```
   Replace `<script_name>` with the desired script, such as `gpu_vector_add.py` or `bank_transactions.py`.

## Outputs

### GPU Vector Addition
```plaintext
CUDA devices: <list of detected CUDA devices>
GPU computation successful!
```

### ThreadPoolExecutor vs. Threading
```plaintext
Task 1 executed
Task 2 executed
Execution time with ThreadPoolExecutor: 0.0001 seconds
Execution time with threading library: 0.0002 seconds
```

### Fibonacci Calculation with Threads
```plaintext
Execution time with 4 threads: 2.3456 seconds
Execution time with 9 threads: 5.6789 seconds
```

### Multiprocessing vs. Multithreading
```plaintext
List processing complete
Multiprocessing time = 2.3456 seconds
List processing complete
Multithreading time = 3.4567 seconds
```

### Thread-Safe Bank Transactions
```plaintext
Deposited: 50, New Balance: 150
Deposit Execution Time: 0.000123 seconds
Withdrawn: 30, New Balance: 120
Withdraw Execution Time: 0.000145 seconds
Final Balance: 120
Total Execution Time: 0.000500 seconds
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to improve this repository.

## Author

Developed by **Muhammad Ahmed**. Feel free to reach out for any questions or suggestions.
