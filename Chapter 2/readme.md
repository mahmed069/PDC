## CODE 1: Thread Synchronization with Queue
Description:

    A producer-consumer model where:
        Producer creates random items and puts them in a shared queue.
        Consumers take items from the queue and process them.

Working:

    Producer creates 5 random items and adds them to the queue.
    Logs a message for each addition.
    Consumers continuously take items from the queue.
    Ensures only one thread processes an item at a time.
    Creates one producer and three consumers sharing the same queue.
    All threads work together to process the queue.

Summary:

The producer adds items to the queue, while multiple consumers process them concurrently without interference.

## CODE 2: Custom Thread Class
Description:

    Demonstrates creating and running threads using a custom thread class.

Working:

    Defines a custom thread class MyThreadClass.
    Creates two threads using the custom class.
    Threads print a message and their name.
    Ensures the program waits for threads to complete before printing "End".

Summary:

Two threads run simultaneously, each printing a message, and the program ends after both threads finish.

## CODE 3: Multiple Tasks Using Threads
Description:

    Runs three independent tasks (functions) simultaneously using threads.

Working:

    Defines three functions: function_A, function_B, and function_C.
    Each function prints a starting message, waits for 2 seconds, then prints an exiting message.
    Creates three threads, one for each function, and starts them.
    Ensures the program waits for all tasks to finish.

Summary:

Three tasks run concurrently, each taking 2 seconds, and the program ends after all tasks are done.
## CODE 4: Sequential Thread Execution
Description:

    Demonstrates sequential thread execution using join().

Working:

    Defines a function my_func to print the thread number.
    A loop creates 10 threads, each running my_func with its number.
    Each thread starts and completes before the next one begins due to join().

Summary:

Threads execute one after another, not simultaneously, as the program waits for each thread to complete before creating the next.
## CODE 5: Producer-Consumer with Semaphore
Description:

    Uses a semaphore to synchronize a producer and a consumer.

Working:

    The producer waits 3 seconds, creates a random item, and signals the consumer.
    The consumer waits until signaled by the producer, then processes the item.
    Repeats this process 10 times using threads.

Summary:

The producer creates items, and the consumer processes them, ensuring synchronization using a semaphore.
## CODE 6: Adding and Removing Items with RLock
Description:

    Simulates adding and removing items from a shared resource (box) using threads and a reentrant lock (RLock).

Working:

    Box class manages a total count of items with an RLock to ensure thread safety.
    Adder thread adds random items to the box.
    Remover thread removes random items from the box.
    Both actions occur concurrently without interference.

Summary:

Two threads add and remove items from a shared resource safely, demonstrating the use of RLock for synchronization.

## Code 7: Basic Multithreading

Working

Thread Class: Extends the Thread class and defines the run method.

Thread Behavior:

Prints the thread name and process ID (os.getpid()).

Sleeps for a random duration (1-10 seconds).

Prints a completion message.

Execution:

Creates nine threads with random durations.

Starts all threads using start().

Waits for all threads to finish using join().

Result

All threads run simultaneously with random durations.

Total execution time is printed after all threads complete.

Summary

This program demonstrates how to create and run multiple threads simultaneously and measure the total execution time.

## Code 8: Multithreading with Locks

Working

Lock Usage:

Threads acquire a lock (threadLock) before printing and release it after finishing.

Thread Behavior:

Prints the thread name and process ID after acquiring the lock.

Sleeps for a random duration (1-10 seconds).

Releases the lock after finishing.

Execution:

Creates and starts nine threads.

Ensures only one thread prints at a time using the lock.

Result

Threads execute one at a time for printing but run independently for other tasks.

Total execution time is printed.

Summary

This program ensures synchronized output by using locks to control access to shared resources (printing).

## Code 9: Mixed Lock Management

Working

Modified Lock Usage:

Threads acquire a lock only for printing and release it immediately after.

The sleep operation is independent of the lock.

Thread Behavior:

Acquires the lock to print its details.

Sleeps for a random duration (1-10 seconds).

Releases the lock after printing.

Result

Threads print their details sequentially but run independently for other tasks.

Total execution time is printed.

Summary

This program uses locks to control access to printing while allowing threads to run independently for other operations.

## Code 10: Producer-Consumer with Events

Working

Producer:

Generates random items and adds them to a shared list.

Signals the consumer using an event after adding each item.

Clears the event after signaling.

Consumer:

Waits for the event to be set by the producer.

Pops an item from the list after the event is set.

Execution:

Both threads run and coordinate using the Event object.

Result

Producer adds items to the list, and the consumer removes them in a synchronized manner.

Both threads work together using events to manage coordination.

Summary

This program demonstrates producer-consumer synchronization using the Event class.

## Code 11: Producer-Consumer with Conditions

Working

Condition Object:

Ensures proper synchronization between the producer and consumer.

Producer:

Adds items to a shared list up to a limit (10 items).

Waits if the list is full.

Consumer:

Removes items from the shared list.

Waits if the list is empty.

Coordination:

Uses condition.wait() and condition.notify() for synchronization.

Result

Producer and consumer operate without conflicts.

Producer pauses when the list is full, and the consumer waits when the list is empty.

Summary

This program implements producer-consumer synchronization using a condition variable to manage shared resources.

## Code 12: Race Simulation with Barriers

Working

Barrier:

Ensures all threads (runners) reach the barrier before proceeding.

Runner:

Each runner sleeps for a random time (2-5 seconds).

Prints a message upon reaching the barrier.

Execution:

Creates threads for runners.

Waits for all runners to reach the barrier before continuing.

Result

All runners wait at the barrier until everyone arrives.

The race finishes after all runners proceed past the barrier.

Summary

This program demonstrates thread synchronization using a Barrier to coordinate the progress of multiple threads
