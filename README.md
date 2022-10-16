# rocm_dummy_packages
Dummy packages to resolve some dependencies to assist in installation of ROCM

See https://github.com/RadeonOpenCompute/ROCm/issues/1713#issuecomment-1256420167

Did only work with kernel version 5.15.0-50-generic, NOT 6.0.0 and above

## ROCm fails to install due to dependency issues for **rocm-llvm**

Just download and install these dummy packages. They don't contain any binaries, just tells apt that you have the packages installed that it requires
for **rocm-llvm**

No warranties implied. This worked for me on Ubuntu 22.04
I did install **libstd++-10-dev** manually.

You may need to uninstall the python-is-python3 package to install the python dummy package. But it is trivial to just create the symlink yourself.
