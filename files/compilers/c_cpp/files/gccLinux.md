# GCC (GNU Compiler Collection) on Linux

[visit this (easier path)](cl2.md)

## About
- **GCC** = GNU Compiler Collection → includes `gcc` (C) and `g++` (C++).
- On Linux, installing **GCC** automatically installs support for both C and C++.
- Works out-of-the-box since Linux has a standardized system header + library layout.

---

## Installation (Debian/Ubuntu)

>### Step 1: Update your system
>```bash
>sudo apt update
>sudo apt upgrade -y
>```
>
>### Step 2: Install GCC + development tools
>```
>sudo apt install build-essential -y
>```


## This installs:

>- gcc → C compiler
>- g++ → C++ compiler
>- make → build tool
>- core headers/libraries → (libc6-dev, etc.)

## Verification

>### Check versions:
>
>```bash
>gcc --version
>g++ --version
>```