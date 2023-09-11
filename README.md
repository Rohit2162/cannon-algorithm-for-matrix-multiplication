# cannon-algorithm-for-matrix-multiplication
# Parallel-Matrix-Matrix-Multiplication-with-MPI-using-Cannon-s-Algorithm

## How to install MPI on Ubuntu / Linux
## 1. Fedora
Command to install package:
sudo dnf upgrade
sudo dnf install apt
sudo apt install libopenmpi-dev

## 2. Ubuntu
sudo apt-get update
sudo apt-get install libopenmpi-dev

-> To check the version of the MPI downloaded, type the following command:
mpicc --showme:version

There are chances of getting an error if your system has anaconda installed.So run the below command line and then try to install the MPI
1. deactivate conda

Minimum Hardware Requirements:
1. RAM = 4GB
2. HDD = 10GB

Operating System used: Ubuntu

Language: C++


## Cannon's Matrix MAtrix Multiplication
The Matrix-Matrix of Cannon In order to swiftly multiply two huge matrices, multiplication is a parallel approach that distributes the work over a number of processors or cores. In particular, distributed memory systems like networked computers are a good fit for the method. It entails breaking the matrices up into blocks and distributing them across the processors in a grid-like arrangement. Then, a coordinated set of local matrix multiplications and cyclic shifts are used to calculate the outcome. Cannon's approach is a helpful tool for high-performance computing applications since it has a reduced communication cost when compared to other parallel matrix multiplication methods.

## MPI (Message Passing Interface)
The message-passing interface (MPI) is a standardized means of exchanging messages between multiple computers running a parallel program across distributed memory.

## Cannon's Matrix MAtrix Multiplication using MPI
1. Create a text file named A.txt,
   Write the NxN Matrix of your choice
2. Create a text file named B.text,
   Write the NxN Matrix of your choice
3. Create the .c file and write code provided in cannon.c

## How to compile and run the cannon.c file
_If anaconda is installed, then deactivate the enviroment by **conda deactivate**, then only run and compile the file._
1. mpicc -o filename filename.c
2. mpirun -np 4 ./filename
3. If 2. command is giving error, then run the below command
4. mpirun --oversubscribe -np 16 ./filename -quiet


## References:
1. https://iq.opengenus.org/cannon-algorithm-distributed-matrix-multiplication/#:~:text=Cannon's%20algorithm%20is%20a%20distributed,been%20shown%20to%20be%20difficult.
2. https://www.comrevo.com/2020/11/cannons-algorithm-for-matrix-multiplication.html
3. https://www.techtarget.com/searchenterprisedesktop/definition/message-passing-interface-MPI
4. OpenAI GPT-3.5 (https://www.openai.com)
