# blhost
Modifications of NXP blhost to run on an iMX6UL and update a Kinetis microcontroller via UART only.

From the root of the repo, compile in a "build" directory with the following commands:

mkdir build

cd build

cmake -DCMAKE_TOOLCHAIN_FILE=<path to toolchainfile.cmake> ..
  
make

Output binary is then: build/blhost
