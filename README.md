# README #

Project for "DAT300 - Data-driven Support for Cyber-physical Systems" course.

## What is this repository for? ##

Read more about the project [here](https://vtaxiarchis.wordpress.com/projects-ids).

## Compile and run ##

### /ids/ids.c (C implementation) ###
```
gcc ids.c -o ids
./ids
```

### /ids_lib/ids_lib.c (Optimized C implementation using GSL libraries) ###
```
gcc -Wall -o ids_lib ids_lib.c -lgsl -lgslcblas -lm
./ids_lib
```

### /matlab (Simplified MATLAB implementation) ###
* train_phase.m (MATLAB code for training phase) -> generates s.txt and U.txt
* test_phase.m (MATLAB code for testing phase)

### /matlab_output (Example output of MATLAB) ###
* Both implementations in C take as input the files s.txt and U.txt generated by MATLAB.
* Example output files for N=2000, L=1000, r=29 and theta=0.0134.
