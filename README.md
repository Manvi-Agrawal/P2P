# Peer-To-Peer-Communication

## Overview
This project implements a peer-to-peer communication application using Inter-Process Communication (IPC) mechanisms: Sockets and FIFOs. The application consists of two processes, P1 and P2, which can communicate with each other using either mechanism.


### FIFO Communication
For FIFO communication, `main.c` file is used to create two FIFO pipes before starting processes P1 and P2. This is necessary because FIFOs are unidirectional, and creating the pipes beforehand prevents potential errors. The created FIFOs are used by P1 and P2 for communication.

## Socket Communication
Socket communication is bidirectional, eliminating the need for a separate `main.c` file to create pipes.

### Building and Running Locally

```bash
make clean
make all
make runF # Only for fifo, for pipe creation
make runP1
make runP2
```
