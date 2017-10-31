# README #

Project for "Data-driven Support for Cyber-physical Systems" course.

## What is this repository for? ##

Industrial Control Systems (ICS) manage critical infrastructure such as water supply systems,
nuclear and power plants. In the recent past coordinated attacks have been leveled against ICS
by adversaries with strong motivated intentions and if successful, these attacks have the
potential to cause catastrophic damages. As a result there is an urgent need for pragmatic tools
to detect cyber intrusions in ICS. Consequently, traditional anomaly-based network intrusion
detection techniques are a precious technology to protect ICS against coordinated attacks but are
not enough to detect and let alone protect ICS from cyber attacks perpetrated by strongly
motivated adversaries. In this project we study a model free approach called PASAD (Process-Aware
Stealthy-Attack Detection) as a choice to detect attacks by monitoring time series of sensor
measurements. In particular, we evaluate the performance of PASAD, by analyzing its efficiency in
physically constrained systems. Our main contribution is an efficient implementation of PASAD in
a low-level programming language and investigating its efficiency when deployed on limited-resource 
hardware. We also test the effectiveness of our approach, by evaluating the system against simulated
equipment and economic attacks.

## Compile and run ##

###/ids/ids.c (PASAD C implementation)###
* gcc ids.c -o ids
* ./ids

###/ids_lib/ids_lib.c (Optimized PASAD C implementation using GSL libraries)###
* gcc -Wall -o ids_lib ids_lib.c -lgsl -lgslcblas -lm
* ./ids_lib

###/pasad_matlab (PASAD simplified MATLAB implementation)###

###/pasad_matlab_output (Example output of MATLAB)###
* Both PASAD implementation in C take as input the files s.txt and U.txt.
* In this particular example N=2000, L=1000, r=29 and theta=0.0134.
