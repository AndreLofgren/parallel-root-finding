# Newton-Raphson-parallel
This is a parallel C program for finding multiple roots in the interval [a, b] to the equation f(x) = 0.
In the src folder you will find two separate C programs; one implementing bisection, and one a hybrid
of bisection and Newton-Raphson. Parallelization was acheived with the OpenMP API.

# Compilation
A Makefile is included for compilation. Simply type 'make' or 'make all' in the command line to compile all source code.
The executables will be stored in the newly created folder bin.

# Run
./exec a b N T, where [a, b] is the interval to look for roots, N the number of subintervals and T the number of threads.

# Example runs
$ ./exec 0 100000 100000 2 <br />
Newton-bisection found 31831 zeros in 0.478851 s<br />
Bisection found 31831 zeros in 0.265927 s

$ ./exec 0 1000000 100000 2 <br />
Newton-bisection found 100000 zeros in 0.026027 s <br />
Bisection found 100000 zeros in 0.298974 s

