## CODE 1: Thread Synchronization with Queue

### Description:
- A producer-consumer model where:
  - **Producer** creates random items and puts them in a shared queue.
  - **Consumers** take items from the queue and process them.

### Working:
1. Producer creates 5 random items and adds them to the queue.
2. Logs a message for each addition.
3. Consumers continuously take items from the queue.
4. Ensures only one thread processes an item at a time.
5. Creates one producer and three consumers sharing the same queue.
6. All threads work together to process the queue.

### Summary:
The producer adds items to the queue, while multiple consumers process them concurrently without interference.

---

## CODE 2: Custom Thread Class

### Description:
- Demonstrates creating and running threads using a custom thread class.

### Working:
1. Defines a custom thread class `MyThreadClass`.
2. Creates two threads using the custom class.
3. Threads print a message and their name.
4. Ensures the program waits for threads to complete before printing "End".

### Summary:
Two threads run simultaneously, each printing a message, and the program ends after both threads finish.

---

## CODE 3: Multiple Tasks Using Threads

### Description:
- Runs three independent tasks (functions) simultaneously using threads.

### Working:
1. Defines three functions: `function_A`, `function_B`, and `function_C`.
2. Each function prints a starting message, waits for 2 seconds, then prints an exiting message.
3. Creates three threads, one for each function, and starts them.
4. Ensures the program waits for all tasks to finish.

### Summary:
Three tasks run concurrently, each taking 2 seconds, and the program ends after all tasks are done.

---

## CODE 4: Sequential Thread Execution

### Description:
- Demonstrates sequential thread execution using `join()`.

### Working:
1. Defines a function `my_func` to print the thread number.
2. A loop creates 10 threads, each running `my_func` with its number.
3. Each thread starts and completes before the next one begins due to `join()`.

### Summary:
Threads execute one after another, not simultaneously, as the program waits for each thread to complete before creating the next.

---

## CODE 5: Producer-Consumer with Semaphore

### Description:
- Uses a semaphore to synchronize a producer and a consumer.

### Working:
1. The producer waits 3 seconds, creates a random item, and signals the consumer.
2. The consumer waits until signaled by the producer, then processes the item.
3. Repeats this process 10 times using threads.

### Summary:
The producer creates items, and the consumer processes them, ensuring synchronization using a semaphore.

---

## CODE 6: Adding and Removing Items with RLock

### Description:
- Simulates adding and removing items from a shared resource (box) using threads and a reentrant lock (RLock).

### Working:
1. `Box` class manages a total count of items with an RLock to ensure thread safety.
2. `Adder` thread adds random items to the box.
3. `Remover` thread removes random items from the box.
4. Both actions occur concurrently without interference.

### Summary:
Two threads add and remove items from a shared resource safely, demonstrating the use of RLock for synchronization.

---

## How to Run
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```
2. Run each Python file individually to see the threading examples in action:
   ```bash
   python code1.py
   python code2.py
   # ...and so on
   ```

Code 7: Basic Multi-threading

Functionality:

Creates and starts nine threads.

Each thread performs the following tasks:

Prints its name.

Displays the process ID.

Sleeps for a random duration between 1 to 10 seconds.

Prints when it finishes.

Working:

Thread Creation: Nine threads are created with random durations.

Thread Execution: Threads start simultaneously using start().

Thread Synchronization: The program waits for each thread to finish using join().

Execution Time: The total execution time is calculated and displayed.

Result:

Threads run in parallel with random durations.

The program outputs thread details and total execution time.

Code 8: Multi-threading with Locks

Functionality:

Introduces a lock to synchronize threads.

Ensures only one thread can print at a time.

Working:

A threading.Lock is used to control access to the printing operation.

Threads acquire the lock before printing and release it after printing.

The rest of the execution is similar to Code 7.

Result:

Threads run one by one for printing, ensuring no overlap in output.

Total execution time is displayed.

Code 9: Lock with Independent Execution

Functionality:

Threads acquire a lock to print their details but release it immediately for parallel execution.

Working:

Each thread acquires a lock to print its name and process ID, then releases the lock.

After releasing the lock, the thread sleeps for a random duration and prints its completion message.

The rest of the flow is similar to Code 7.

Result:

Threads execute in parallel but take turns for printing.

Outputs thread details and total execution time.

Code 10: Producer-Consumer Using Events

Functionality:

Implements producer-consumer synchronization using threading.Event.

The producer generates items, and the consumer removes them.

Working:

Producer:

Generates random numbers and appends them to a list.

Signals the consumer using event.set().

Clears the event after signaling.

Consumer:

Waits for the event signal.

Pops an item from the list when notified.

Synchronization is managed through events to ensure smooth communication.

Result:

The producer adds items, and the consumer removes them in a synchronized manner.

Logs each action and ensures proper coordination.

Code 11: Producer-Consumer Using Condition Variables

Functionality:

Implements producer-consumer synchronization using threading.Condition.

Working:

Producer:

Adds items to a list until the limit of 10 is reached.

Waits when the list is full.

Consumer:

Removes items from the list.

Waits when the list is empty.

Both threads use condition.notify() to wake each other when appropriate.

Result:

Ensures the producer does not exceed the limit and the consumer does not act on an empty list.

Logs the producer-consumer interaction with precise synchronization.

Code 12: Barrier Synchronization

Functionality:

Simulates a race with three runners using a threading.Barrier.

All runners must reach a barrier before proceeding.

Working:

A Barrier is set for three runners.

Each runner:

Sleeps for a random duration.

Prints its arrival at the barrier.

The barrier waits until all runners arrive.

After crossing the barrier, the program concludes the race.

Result:

Threads synchronize at the barrier before continuing.

Simulates a race with synchronized execution.

Summary

Code 7-9: Demonstrate thread creation, execution, and synchronization using locks.

Code 10: Explores event-based synchronization for producer-consumer problems.

Code 11: Implements condition variables for producer-consumer coordination.

Code 12: Uses barriers for thread synchronization in a race simulation.

These programs provide a comprehensive introduction to multi-threading concepts in Python, demonstrating their use in real-world scenarios.

How to Run

Clone the repository:

git clone <repository-url>
cd <repository-folder>

Run each Python file individually to see the threading examples in action:

python code7.py
python code8.py
# ...and so on

License

This repository is open-source and available under the MIT License.
