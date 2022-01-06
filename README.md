# model3-RPi4
Files required to run Supermodel the Sega Model 3 emulator under Batocera Linux.

For some reason I cannot build Supermodel on an x86 machine for the Raspberry Pi 4.
You can however build it on the RPi4 directly.
This is the resulting binary & associated files built on a RPI4 running Ubuntu 21.04.

Batocera will now grab these files to install during their RPi4 build process.

Note: The binary is modified to run specifically with Batocera Linux v33 or later.
      The Rules file is changed also to optimise for the RPi4.
      
To build yourself - here are the instructions for an Ubuntu 21.04 system:

1. sudo apt install git build-essential libsdl2-dev libsdl2-net-dev libglew-dev zlib1g-dev
2. git clone https://github.com/dmanlfc/model3-RPi4.git
3. cd model3-RPi4
4. make -j4

This creates the Batocera binary

I appreciate the developers of this great emulator.
The original source code is available here:
https://sourceforge.net/p/model3emu/code/HEAD/tree/trunk/
