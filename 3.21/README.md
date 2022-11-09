# Question-3.21
.
The Collatz conjecture concerns what happens when we take any positive integer n and apply the following algorithm:

  n =  n ∕ 2, if n is even
 
    =  3 * n + 1, if n is odd
The conjecture states that when this algorithm is continually applied, all positive integers will eventually reach 1. For example, if n = 35, the sequence is

35, 106, 53, 160, 80, 40, 20, 10, 5, 16, 8, 4, 2, 1

Write a C program using the fork() system call that generates this sequence in the child process. The starting number will be provided from the command line. For example, if 8 is passed as a parameter on the command line, the child process will output 8, 4, 2, 1. Because the parent and child processes have their own copies of the data, it will be necessary for the child to output the sequence. Have the parent invoke the wait() call to wait for the child process to complete before exiting the program. Perform necessary error checking to ensure that a positive integer is passed on the command line.

# References for the Source Code

The base for the solution [Code.c](https://github.com/Kashish-0106/Question-3.21/blob/main/code.c) was obtained from the source code in [UCM Assignments](http://ucmassignments.blogspot.com/2016/06/a-collatz-conjecture-collatz-conjecture.html) and [this link](https://github.com/VibaRUdupa/CS252-OS/blob/main/Question%203.21/Code.c).

NOTE: No license was found on their website. The author does not intend any copyright infringement.


# Results

The fork() function works only on Linux OS. Specific header files are to be loaded for operations related to processes that can not be done on Windows OS. To run this code, either use a Linux OS (by using a Virtual environment or dual booting) or this could also be executed on some of the online compilers like [Online GDB](https://www.onlinegdb.com/)

Output console:

![result](/3.21/result-screenshot.png)
