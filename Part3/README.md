# Reasons for concurrency and parallelism


To complete this exercise you will have to use git. Create one or several commits that adds answers to the following questions and push it to your groups repository to complete the task.

When answering the questions, remember to use all the resources at your disposal. Asking the internet isn't a form of "cheating", it's a way of learning.

 ### What is concurrency? What is parallelism? What's the difference?
 > Concurrency: The ability to run different parts of a program at the same time, these parts can comunicate with eachother, threads. 
   Parallelism: Deviding a program into smaller parts and solving these parts in parallell. 
   Difference: With parallelism you are solving lots of similar problems, with concurrency the tasks can be different and comunicate with eachother.
 ### Why have machines become increasingly multicore in the past decade?
 > Lots of tasks can be solved in parallel and we have reached the maximum level of frequency in our machines. 
 
 ### What kinds of problems motivates the need for concurrent execution?
 (Or phrased differently: What problems do concurrency help in solving?)
 > Operating systems,controll systems, 
 
 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > *Your answer here*
 
 ### What are the differences between processes, threads, green threads, and coroutines?
 > Processes and threads are managed by th OS. Threads exists within a process, the threads within the same process are able to comunicate with eachother.
   Green threads are threads that are managed by a virtual machine. Coroutines are threads that can be activated by multiple inputs.
 
 ### Which one of these do `pthread_create()` (C/POSIX), `threading.Thread()` (Python), `go` (Go) create?
 > pthread_create(): thread
   threading.Thread(): green thread
   go: process
 
 ### How does pythons Global Interpreter Lock (GIL) influence the way a python Thread behaves?
 > GIL makes sure that only one thread can use the python interpreter at once. This means that only one thread can run at any time.
 
 ### With this in mind: What is the workaround for the GIL (Hint: it's another module)?
 > Cython
 
 ### What does `func GOMAXPROCS(n int) int` change? 
 > Changes the maximum amount of CPUs that can operate at any time.
