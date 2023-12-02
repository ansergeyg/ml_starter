dkms - https://en.wikipedia.org/wiki/Dynamic_Kernel_Module_Support 

An essential feature of DKMS is that it automatically recompiles all DKMS modules if a new kernel version is installed. This allows drivers and devices outside of the mainline kernel to continue working after a Linux kernel upgrade


Install dkms

sudo apt -y install dkms

Unistall dkms

sudo apt-get remove dkms

Remove dkms Configurations and Data

sudo apt-get -y purge dkms
