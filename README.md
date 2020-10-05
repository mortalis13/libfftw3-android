# libfftw3 for Android

Tested with [**Android NDK r16**](https://developer.android.com/ndk/downloads) on **Windows 10** and **Linux Mint**.  
Based on the following repository: https://github.com/Lauszus/fftw3-android.  
The [**fftw**](http://www.fftw.org) version used is [**3.3.8**](http://ftp.fftw.org/fftw-3.3.8.tar.gz), **ZIP** link: `ftp://ftp.fftw.org/pub/fftw/fftw-3.3.8.zip`.

## Building

- run `ndk-build` from the project directory

## Building another version

- download the [**fftw**](http://www.fftw.org) source from `ftp://ftp.fftw.org/pub/fftw`.
- extract the package to the `jni` folder
- copy the `config.h` from the original repository source and modify it for your needs (or run the `./configure` command from a **Linux** console to generate the `config.h` header from the source)
- on **Linux**, you can comment the `LOCAL_SHORT_COMMANDS` line for faster building
- run `ndk-build`
