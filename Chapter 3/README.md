# Multiprocessing and Parallel Programming Examples

This repository contains various Python scripts that demonstrate multiprocessing, threading, and other parallel programming concepts. Each example highlights a specific use case or technique for parallelism.

## Table of Contents

1. [Process Management with Daemon Processes](#1-process-management-with-daemon-processes)
2. [Pipes for Inter-Process Communication](#2-pipes-for-inter-process-communication)
3. [Producer-Consumer Model](#3-producer-consumer-model)
4. [Process Lifecycle Management](#4-process-lifecycle-management)
5. [Using Barriers and Locks](#5-using-barriers-and-locks)
6. [Process Pools](#6-process-pools)
7. [Custom Process Class](#7-custom-process-class)
8. [Spawning Multiple Processes](#8-spawning-multiple-processes)

---

### 1. Process Management with Daemon Processes

**File**: `daemon_processes.py`  
**Description**: Demonstrates how to use daemon and non-daemon processes. Daemon processes terminate when the main program exits.

Key Features:
- Background and non-background process execution.
- Process-specific behaviors.

---

### 2. Pipes for Inter-Process Communication

**File**: `pipes_example.py`  
**Description**: Uses `multiprocessing.Pipe` to communicate between processes. A producer creates items, and a consumer multiplies them.

Key Features:
- Sending and receiving data via pipes.
- Multiple processes interacting through a shared communication channel.

---

### 3. Producer-Consumer Model

**File**: `producer_consumer.py`  
**Description**: Implements a producer-consumer model using a `Queue`. The producer adds items to the queue, and the consumer retrieves them.

Key Features:
- Synchronization between producer and consumer.
- Demonstrates the use of `multiprocessing.Queue`.

---

### 4. Process Lifecycle Management

**File**: `process_lifecycle.py`  
**Description**: Explores process lifecycle management, including starting, terminating, and joining processes.

Key Features:
- Monitoring process state.
- Handling process termination and exit codes.

---

### 5. Using Barriers and Locks

**File**: `barriers_and_locks.py`  
**Description**: Synchronizes processes using barriers and locks. Ensures processes wait for each other at a barrier point.

Key Features:
- Barrier synchronization.
- Serialized printing with locks.

---

### 6. Process Pools

**File**: `process_pools.py`  
**Description**: Demonstrates the use of `multiprocessing.Pool` to execute a function across multiple input values concurrently.

Key Features:
- Efficient parallel processing using pools.
- Map functionality for distributing tasks.

---

### 7. Custom Process Class

**File**: `custom_process_class.py`  
**Description**: Defines a custom process class by extending `multiprocessing.Process`.

Key Features:
- Custom behavior for processes.
- Demonstrates the `run` method in a custom process class.

---

### 8. Spawning Multiple Processes

**File**: `spawn_processes.py`  
**Description**: Spawns multiple processes to execute a function with different arguments.

Key Features:
- Dynamically starting and joining multiple processes.
- Demonstrates loop-based process creation.

---

## How to Run the Examples

1. Clone the repository:
   ```bash
   git clone https://github.com/mahmed069/multiprocessing-s.git
   cd multiprocessing



![image](https://github.com/user-attachments/assets/6f8f6e54-3a6f-4de3-a4a1-ec3cc9e457a0)

![image](https://github.com/user-attachments/assets/863a0e08-4cdb-4720-ba7c-2f011a3c2fa2)

![image](https://github.com/user-attachments/assets/67c0e1cf-0b80-4be9-a0cb-f0d067e4ba27)

![image](https://github.com/user-attachments/assets/2ded58ec-6143-4020-a250-b60ebde2b125)

![image](https://github.com/user-attachments/assets/5639ada3-5005-4a91-a643-e9251ed0b505)
