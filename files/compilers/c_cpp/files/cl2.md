# Clang on Linux

## About
- **Clang** is part of the LLVM project.
- It supports both C and C++.
- On Linux, Clang reuses **GCC’s standard libraries and headers** → so you need GCC’s [dev packages](gccLinux.md) too.
- Installing Clang is as easy as using your package manager.

---

## Installation (Debian/Ubuntu)

### Step 1: Update your system
```bash
sudo apt update
sudo apt upgrade -y
```
### Step 2: Install Clang
```bash
sudo apt install clang -y
```
This installs:

- clang → C compiler
- clang++ → C++ compile
- LLVM tooling (e.g., lldb if available)

## Verification
### Check versions:

```bash
clang --version
clang++ --version
```