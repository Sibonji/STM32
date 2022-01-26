Update the system (optional step):

sudo apt-get update
sudo apt upgrade

Installation git:

sudo apt-get install git

Installation libusb:

sudo apt-get install libusb-1.0-0-dev

Installation cmake:

sudo apt-get install cmake

Linux 20.04 and above. Download GNU Embedded Toolchain from the website.

Unpack the tarball to the install directory, like this:

    cd ${install_dir} && tar xjf gcc-arm-none-eabi-_version_-linux.tar.bz2

${install_dir} is directory where you downloaded your file. _version_ is version of arm toolchain.

After set path like this:

    ${install_dir}/gcc-arm-none-eabi-*/bin/arm-none-eabi-gcc

Or this:
    export PATH=$PATH:${install_dir}/gcc-arm-none-eabi-*/bin
    arm-none-eabi-gcc --version

${install_dir} is directory where you saved unpacked file. Instead of * write full name of directory (version of gnu arm toolchain).