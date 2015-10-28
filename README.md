# Matrix-Vector-Multiplication-Using-MPI
In this code matrix and vector are read from file by processor having rank 0 and rows of matrix are distributed among
the processors in a communicator and rank 0 processor sends vector to all other processors using mpi_bcast collective 
call.
So each processor does the job of multiplication of rows and given vector. And final multiplication result is gathered
to rank 0 proc using mpi_gatherv collective call.

This code will work for any dimension of matrix,vector and any no of processors.
