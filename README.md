# CUDA-programming
CUDA (Compute Unified Device Architecture) is a parallel computing platform and application
programming interface (API) model created by Nvidia for general computing on its own GPU (Graphics
Processing Unit). It enables developers to speed up compute-intensive applications by harnessing the
power of GPUs for the parallelizable part of the computation. The CUDA platform is designed to work
with programming languages such as C, C++, and Fortran.
How To Run CUDA C or C++ on Google Colab
Step 1: Go to https://colab.research.google.com in Browser and Click on New Python 3 Notebook
Step 2: Click to Runtime > Change > Hardware Accelerator GPU
Step 3: Refresh the Cloud Instance of CUDA On Server [write code in a Separate code Block and Run]
Step 4: Install CUDA Version 9 [write code in a Separate code Block and Run]
Step 5: Check version of CUDA by running the command: !nvcc –version
Step 6 : Execute the command below to install a small extension to run nvcc from Notebook cells [write
code in a Separate code Block and Run]
!pip install git+git://github.com/andreinechaev/nvcc4jupyter.git
Step 7: Load the extension using the code: %load_ext nvcc_plugin
How does a CUDA program run?
Basic Steps:
• Initialize CPU arrays
• Allocate memory on GPU memory for these arrays
• Transfer arrays from CPU (Host) memory to GPU (Device) memory
• Create Threads
• Launch the GPU function
• Transfer the results from Device to Host
• Print/Save results
• Deallocate GPU memory
