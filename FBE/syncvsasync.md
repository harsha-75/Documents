## Synchronous vs Asynchronous

- can i do work while waiting ?

## Synchronous I/O

- Caller sends a requests and blocks
- Caller cannot execute any code meanwhile
- Recevier Responds , Caller Unblocks.
- Caller and receiver in sync

### Example of an OS Synchronous I/O

- Program asks os to read from the disk
- Program main thread is taken off of the CPU
- Read completes , Program can resume the execution
- 
  ```
      dowork();
      readfile("largefile.dat");
      doWork2()
  ```
 
 ## Asynchronous I/O

 - caller sends a request
 - Caller can work until it gets a response
 - Caller either : 

    1. checks if the responce is ready (epoll)
    2. Recevier calls back when it is done (io_uring)
    3. Spins up a new thread that blocks
- 

