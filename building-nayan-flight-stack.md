# Building Nayan Flight Stack



#### Toolchain Installation

1. Fetch relevant toolchain from [here](https://launchpad.net/gcc-arm-embedded/4.9/4.9-2015-q3-update).

2. Extract toolchain and add `<path-to-toolchain>/bin` to PATH environment variable.

3. Run `arm-none-eabi-gcc --version` and make sure the following output is shown: 

    ```
arm-none-eabi-gcc (GNU Tools for ARM Embedded Processors) 4.9.3 20150529 (release) [ARM/embedded-4_9-branch revision 227977]
Copyright (C) 2014 Free Software Foundation, Inc.
TThis is free software; see the source for copying conditions.  There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
    ``` 
4. For Ubuntu Linux machines with previous arm-none-eabi-gcc installation remove them by executing following commands:
    ```
    sudo apt-get remove gcc-arm-none-eabi gdb-arm-none-eabi binutils-arm-none-eabi gcc-arm-embedded
    sudo add-apt-repository --remove ppa:team-gcc-arm-embedded/ppa
    ``` 

 #### Installing Pre-requisites
 For Mac users:
 
 1. Install [homebrew](http://brew.sh/) into your system.
 
 2. Execute following list of commands from your shell:
     ```
     brew tap PX4/homebrew-px4
     brew update
     brew install git bash-completion genromfs kconfig-frontends
     brew install astyle cmake ninja
     sudo easy_install pip
     sudo pip install pyserial empy
     ```
 
 
 For Linux users:
 
 1. Execute following command in your terminal:
     ```
     sudo apt-get install python-serial openocd \
     flex bison libncurses5-dev autoconf texinfo build-essential \
     libftdi-dev libtool zlib1g-dev \
     python-empy  -y
     ```
 
