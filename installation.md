**What to actually install?**

There is a lot of uncertainties when it comes to installing tensorflow or pytorch.

The biggest question is how to install everything "properly" so that you feel "safe" you installed everything needed?

It turns out it mostly depends on what hardware you have. As of 12/05/2023 it is still complicated to "fully" install tensorflow or pytorch if you have anything else but intel + nvidia chips.

My laptop is AMD ryzen 5 with RADEON mobile 3500U gfx and according to the official ROCm page: https://rocm.docs.amd.com/en/latest/release/windows_support.html it is not supported.

However the problem that I was trying to solve was not entirely valid. 

I was trying to install everything properly meaning that I tried to install all the drivers and libs to work with cpu and gpu. 
It turns out that to work with tensorflow or pytorch (especially when you're a beginner) you don't
necessairly need **GPU**. And gpu is quite painfull to install and configure for anything else except nvidia even these days.

It was actually even worse. I was trying to install ROCm in a virtualbox! And I found out that it was impossible due to the nature of virtualbox hypervisor type.

So if you want to try tensorflow or pytorch and have few problems as possible during the installation, all you need to install is tensorflow but just for CPU.
It is same for pytorch. You need to find a version that works with CPU only.

INSTALLATION:

1) Install python (on Windows 10)

https://www.python.org/downloads/release/python-3120/

Find windows installer, download and install it.

Some notes to configure your windows 10:

https://docs.python.org/3/using/windows.html#removing-the-max-path-limitation

How to increase max path length:

a) Open command line and run gpedit.msc

b) Administrative templates->System->Filesystem

c) Enable Win32 long paths

2) You need pip manager, but if you installed python from the previous step it should be included automatically.

https://pip.pypa.io/en/stable/installation/

3) Just follow accurately the manual on the official page:

https://www.tensorflow.org/install/pip#windows-native

Remember, you can just use **tensorflow-cpu**

Later, if you have a need to use **GPU** you can start exploring if it is possible with your GPU and what you should install and configure for that. 
