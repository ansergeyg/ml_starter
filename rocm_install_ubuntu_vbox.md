dkms - https://en.wikipedia.org/wiki/Dynamic_Kernel_Module_Support 

An essential feature of DKMS is that it automatically recompiles all DKMS modules if a new kernel version is installed. This allows drivers and devices outside of the mainline kernel to continue working after a Linux kernel upgrade


Install dkms

sudo apt -y install dkms

Unistall dkms

sudo apt-get remove dkms

Remove dkms Configurations and Data

sudo apt-get -y purge dkms


Some good points about dkms:

Why don't we make DKMS packages the default packages for proprietary hw driver modules? 

Because prebuilt modules in the repos are updated in lockstep with the kernel package, so you actually can't have a situation where the module version doesn't match the kernel unless you do a partial upgrade. 

https://www.reddit.com/r/archlinux/comments/bib65t/why_dont_we_make_dkms_packages_the_default/
