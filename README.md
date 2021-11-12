# OpenCLTutorial

Hey there! This is the repository with the code I used in the OpenCL tutorial video on my channel. Check it out here:

# How to build

1. Download the repo in whichever way you like.
2. Install the OpenCL binaries on your system. You can get them for AMD: http://developer.amd.com/tools-and-sdks/heterogeneous-computing/amd-accelerated-parallel-processing-app-sdk/downloads/ , for Intel: http://software.intel.com/en-us/vcsource/tools/opencl-sdk , or for Nvidia: https://developer.nvidia.com/cuda-downloads.
3. Open the repo in Visual Studio 2019 or above.
4. Go into the project properties -> Linker -> General -> Additional library directories, and add the directory containing your OpenCL binaries.
5. Then go to project properties -> Linker -> Input -> Additional dependencies, and add the OpenCL binary. (usually 'OpenCL.lib')
6. Make sure that project properties -> C/C++ -> General -> Additional include directories, still contains the lib\OpenCL\Include folder.
7. Build/Run the program like normal in VS.
8. You can also build this project without VS. Just make sure that you link/include OpenCL properly, and that vectorsum.cl is in the same directory as your executable.
