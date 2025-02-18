# PHalstead

PHalstead is a tool to get Halstead's measures in parallel applications. Halstead evaluates applications based on the numbers of operators and operands (tokens) in the code:
- n1: number of operators 
- n2: number of operands
- N1: total occurrence of operatos
- N2: total occurrence of operands

Based on the number of tokens the following metrics are measured:
- Program length
- Program vocabulary
- Program volume in bits
- Programming difficulty
- Development effort
- Development time in seconds
- Development time in hours

The currently version allows the analysis of C++ code parallelized using the following parallel programming models:

- [Intel TBB](https://github.com/uxlfoundation/oneTBB)
- [FastFlow](https://github.com/fastflow/fastflow)
- [GrPPI](https://github.com/arcosuc3m/grppi)
- [SPar](https://github.com/GMAP/spar)
- [MPI](https://www.open-mpi.org)
- [DSParLib](https://github.com/GMAP/DSParLib)
- [MPR](https://github.com/GMAP/mpr)
- ResiFlow

In addition, the currently version allows the analysis of Java code parallelized using the following parallel programming models:

- Flink
- Storm

## How to install:

Python package is required to use PHalstead
- Tested on python3 

## How to cite:
- G. Andrade, D. Griebler, R. Santos, C. Kessler, A. Ernstsson, L. G. Fernandez "Analyzing Programming Effort Model Accuracy of High-Level Parallel Programs for Stream Processing." 2022 48th Euromicro Conference on Software Engineering and Advanced Applications (SEAA). IEEE, 2022.

## How to run:

`python3 parallel-halstead.py --api API file.cpp` 

Ex: `python3 parallel-halstead.py --api spar src/spar_video.cpp`

or

`python3 parallel-halstead.py -h` for more info
