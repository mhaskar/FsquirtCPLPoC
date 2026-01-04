`Fsquirt.exe` Windows binary attempts to load a Control Panel applet (CPL) called `bthprops.cpl` from its current working directory.
When `bthprops.cpl` is present alongside `fsquirt.exe`, the binary loads it and executes a MessageBox from DLLMain.

This PoC code generates a malicious `bthprops.cpl` file that can be loaded by `fsquirt.exe`. The included `build.sh` script compiles the CPL module for you.

![Fsquirt.exe PoC screenshot](screenshot.png)
