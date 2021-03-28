# ARCVM V1

Moved from the BrandonKi/ARCANE

Has a different instruction set than ARCVM-V2 https://github.com/BrandonKi/ARCVM-V2

A minimal bytecode virtual machine written in C++

has a seperate instruction set from BrandonKi/ARCVM-V2

This is the back-end for a programming language called ARCANE (https://github.com/BrandonKi/ARCANE)

However the front-end is currently being rewritten

full instruction set documented below

https://docs.google.com/spreadsheets/d/1RJZBzq33wgM4W4Zc3TOtNXXqJP57WYDpCWftLpLdmg8/edit?usp=sharing

bytecode file format described below

#@TODO ADD FILE FORMAT DESCRIPTION#

# HOW TO BUILD

install and run Cmake with the compiler of your choice
```
cmake .
```

then run with that compiler and pass in the 
name of your bytecode file as a command line argument

# NOTES 

replace reintrpret cast with safe version (memcpy or bitcast(c++20))
