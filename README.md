# blhost
Modifications of NXP blhost to run on an iMX6UL and update the Kinetis microcontroller via UART only.

Compile in a separate directory with the following commands:

mkdir build

cd build

cmake -DCMAKE_TOOLCHAIN_FILE=<path to toolchainfile.cmake> ..
  
make

Output binary is then: build/blhost
