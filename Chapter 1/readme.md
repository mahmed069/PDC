Question1: MultiThreading Vs MultiProcessing
Input Size 1: 100000
Multiprocessing time = 1.1094443798065186
Multithreading time = 0.7600803375244141
Input Size 2: 300000
Multiprocessing time = 1.6197483539581299
Multithreading time = 1.6941444873809814
Analyses:
Multithreading is faster than Multiprocessing because threading works parallelily.
As increasing the tinput size, The execution time increases. 

Question 2:
Execution time with 4 threads: 16.7771 seconds
Execution time with 9 threads: 34.2173 seconds
Analyses:
As increasing the threads execution time also increses this time because of Fabunacci Algo runs as whole at same time not parallily works.

Question 3:
 Leveraging parallelism for large datasets to significantly reduce computation time. It efficiently assigns threads to elements, providing faster execution than sequential CPU processing.

Question 4:
Execution time with ThreadPoolExecutor: 0.0000 seconds
Execution time without ThreadPoolExecutor : 0.0156 seconds
Reason:
ThreadPoolExecutor libraray performs both tasks parallelily thats why it runs faster than without using libraray.

Question 5:
A lock allows only on e thread to access a resource at a time, while a semaphore can allow a specified number of threads to access a resource concurrently.
Withdraw Execution Time: 0.000000 seconds
Final Balance: 120
Total Execution Time: 0.000000 seconds