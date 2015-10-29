# YouCompleteMe Windows Installation Guide

## Instructions for compiling YCM with Clang support
 - Install Cmake and add it to system Path variable
 - CD to this directory: <USERFOLDER>\vimfiles\bundle\YouCompleteMe\third_party\ycmd\cpp
 - Run the following at the console: 
    cmake -G "Visual Studio 12" -DPATH_TO_LLVM_ROOT=C:\LLVM
 - Run the following at the console: 
    msbuild /t:ycm_core;ycm_client_support /property:configuration=Release YouCompleteMe.sln
 - Remove cmake/bin from the system Path variable
