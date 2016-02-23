# libsonivox

This is the original Sonivox MIDI rendering (software synthesis) library 
used by Android. It is licensed under Apache license.

Its main advantages are small size and built-in wavetable, meaning you 
can get a MIDI player under 300kb - without external dependencies and 
without needing patches or an external soundfont!

The library is committed as-is from Android 6.0 source tree with a few 
minor changes made by George Yunaev (gyunaev@ulduzsoft.com):

* The library is merged together from several different places;
* Created Makefile and CMakefile;
* Added test application (heavily based on original eas_main.c and eas_wave.c patched for compatibility)
* Fixed 64-bit platform compatibility

Version: 3.6.10
License: Apache


PLATFORMS:

* Linux: Arch, Debian, Fedora, Ubuntu (player: ALSA, OSS, OpenAL output)
* Windows: x86 and x64
* OSX: x86, x64 and powerpc (in Xterm. player: OpenAL output)

BUILD FROM SOURCE:

Requirements:
* git
* qmake or regular make
* GCC or clang / Xcode / VisualStudio / MinGW or MinGW-w64

Original location in Android source tree: external/sonivox/