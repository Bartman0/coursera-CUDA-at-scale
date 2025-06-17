# Image Rotation using NVIDIA NPP with CUDA

## Overview

This project demonstrates the use of NVIDIA Performance Primitives (NPP) library with CUDA to perform image rotation. The goal is to utilize GPU acceleration to efficiently rotate a given image by a specified angle, leveraging the computational power of modern GPUs. The project is a part of the CUDA at Scale for the Enterprise course and serves as a template for understanding how to implement basic image processing operations using CUDA and NPP.

## Code Organization

`bin/`
This folder should hold all binary/executable code that is built automatically or manually. Executable code should have use the .exe extension or programming language-specific extension.

`data/`
This folder should hold all example data in any format. If the original data is rather large or can be brought in via scripts, this can be left blank in the respository, so that it doesn't require major downloads when all that is desired is the code/structure.

`lib/`
Any libraries that are not installed via the Operating System-specific package manager should be placed here, so that it is easier for inclusion/linking.

`src/`
The source code should be placed here in a hierarchical fashion, as appropriate.

`INSTALL`
This file holds the human-readable set of instructions for installing the code so that it can be executed.

`Makefile`
Configuration file for make.

`run.sh`
A script used to run your executable code, either with or without command-line arguments.

## Supported OSes

Linux

## Supported CPU Architecture

x86_64

## Prerequisites

Download and install the [CUDA Toolkit 11.4](https://developer.nvidia.com/cuda-downloads) for your corresponding platform.
Make sure the dependencies mentioned in [Dependencies]() section above are installed.

## Build and Run

### Linux

To build use the make:

```
$ make
```

## Running the Program

After building the project, you can run the program using the following command:

```bash
make run
```

This command will execute the compiled binary, rotating the input image (Lena.png) by 45 degrees, and save the result as Lena_rotated.png in the data/ directory.

If you wish to run the binary directly with custom input/output files, you can use:

```bash
./bin/imageEdgeDetection --input data/Lena.pgm --output data/Lena_edge.pgm
```

- Cleaning Up
  To clean up the compiled binaries and other generated files, run:

```bash
make clean
```

This will remove all files in the bin/ directory.
