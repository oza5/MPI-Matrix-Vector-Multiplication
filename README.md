# MPI-Matrix-Vector-Multiplication
The code can be run using the following command:

$mpirun -n 4 python test.py

-argument following '-n' is a integerthat defines the number of parallel processors to run the code logic on.
-prints out thr runnig time of each node
-code consists of comments.

-Documentation:
We used various tutorials to first of all get a hang of the MPI syntax and working, we then used tutorials like MPI4py documentation to help us with implementing this simple parallel matrix-vector multiplication program, the number of processors are kept low for initial testing which also allows us to work on our local linux machines by installing the MPI4py package on our terminal, This allows us to not use Amazon aws for the meantime as small aounts of testing can be done on our computers.

The matrix vector multiplication works on the idea of allowing parallel processs to calculate different portions of the vector and then at the end gathering all these calculations to reach the correct answer. Each process when initialised starts a stopwatch that keeps track of the time taken by that specific process to calculate the result of the  portion of v alloted to it.  
