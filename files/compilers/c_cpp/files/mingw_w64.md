
[https://www.mingw-w64.org/](https://www.mingw-w64.org/)

[https://www.msys2.org/](https://www.msys2.org/)


example: `msys2-x86_64-20250622.exe`


Installation
- Download the installer:
  - example: `msys2-x86_64-20250622.exe`

##### (Optional) For more information on the installer, like command line options, or how to verify the checksum and signature of the installer, see the installer guide.

- Run the installer. Installing MSYS2 requires 64 bit Windows 10 or newer.

- Enter your desired Installation Folder (short ASCII-only path on a NTFS volume, no accents, no spaces, no symlinks, no subst or network drives, no FAT).

![alt text](1.png)

- When done, click Finish.

![alt text](2.png)

- Now MSYS2 is ready for you and a terminal for the UCRT64 environment will launch.

![Empty MSYS2 terminal window](3.png)

- **You will probably want to install some tools like the mingw-w64 GCC to start compiling projects. Run the following command:**

```bash
pacman -S mingw-w64-ucrt-x86_64-gcc
```
Note : also install this in the same way if you wanna use "MinGW Makefiles" generator with cmake ==> `mingw-w64-ucrt-x86_64-make`

- The terminal window will show the output as below. Press 'Enter' to continue:

```bash
resolving dependencies...
looking for conflicting packages...

Packages (15) mingw-w64-ucrt-x86_64-binutils-2.41-2
            mingw-w64-ucrt-x86_64-crt-git-11.0.0.r216.gffe883434-1
            mingw-w64-ucrt-x86_64-gcc-libs-13.2.0-2  mingw-w64-ucrt-x86_64-gmp-6.3.0-2
            mingw-w64-ucrt-x86_64-headers-git-11.0.0.r216.gffe883434-1
            mingw-w64-ucrt-x86_64-isl-0.26-1  mingw-w64-ucrt-x86_64-libiconv-1.17-3
            mingw-w64-ucrt-x86_64-libwinpthread-git-11.0.0.r216.gffe883434-1
            mingw-w64-ucrt-x86_64-mpc-1.3.1-2  mingw-w64-ucrt-x86_64-mpfr-4.2.1-2
            mingw-w64-ucrt-x86_64-windows-default-manifest-6.4-4
            mingw-w64-ucrt-x86_64-winpthreads-git-11.0.0.r216.gffe883434-1
            mingw-w64-ucrt-x86_64-zlib-1.3-1  mingw-w64-ucrt-x86_64-zstd-1.5.5-1
            mingw-w64-ucrt-x86_64-gcc-13.2.0-2

Total Download Size:    49.38 MiB
Total Installed Size:  418.82 MiB

:: Proceed with installation? [Y/n]
[... downloading and installation continues ...]
```

- Now you can call `gcc` to build software for Windows.
```bash
gcc --version
```



---
#### **After installing MSYS2 it will update itself via pacman, see the update guide for more information.**
