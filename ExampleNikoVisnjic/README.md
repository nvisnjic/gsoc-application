Based on original code by Jason Kridner for the BeagleBoard GSoC applicaiton. 

1. Install an ARM cross-compiler
2. Edit Makefile to use your ARM cross-compiler of choice , if you got arm-linux-gnueabi-gcc, you're already set.


    * make <- build for Linux host with gcc; for local testing
    * make ARM=1 <- build for ARM with arm-linux-gnueabi-gcc

3. To test emulated, install qemu and run 
    * qemu-arm helloworld_arm

Tested on Arch Linux, 21/03/2015
