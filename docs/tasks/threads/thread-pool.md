---
layout: default
title: Thread Pool
parent: Threads
grand_parent: Tasks
nav_order: 2
---

# The thread pool implementation

### Requirements 

- Create a C++ library (shared object) that implements a simple thread pool 
- Thread pool should be implemented as a class called "parallel_scheduler" 
- Thread pool takes a **capacity** argument in the constructor as a a maximum number of threads in the pool.
- Thread pool defines a method **run** that takes as an input two arguments **function** and the **argument**. 
- All the functions given to the "run" method are enqueued and the thread pool should execute them as soon as any of its threads gets time.
- Next, another executable application is implemented to demonstrate the usage of the thread pool library.
- The demonstration application should enqueue various functions for the execution (more than the capacity).
- The module "parallel_scheduler" should be compiled as a shared library (parallel_scheduler.so) and should be linked with the demo application.

### Expected result

The resulting application should be able to build and execute from command line as follows:

```sh
make
./demo-application
```

The final solution should contain a **Makefile** for the multi-stage build. The Makefile should also contain targets **all** and **clean**. It's recommended to have compiler and compiler flags to be declared as a Makefile variables. Alternatively, **cmake** could also be used instead of make. 
