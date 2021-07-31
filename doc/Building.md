# Building Notepad Next

To build Notepad Next you will need a compatible C++ compiler, the Qt libraries, and the Notepad Next source code.

This document specifically describes how to build Notepad Next using Microsoft's Visual Studio 2019 compiler. Other compilers and operating systems have not been tested, but should be possible with minor changes to the project files and source code.

## Installing Visual Studio 2019

1. Download the installer for [Visual Studio 2019 Community](https://visualstudio.microsoft.com/) (other versions should work if you have those installed already).
1. Run the installer
1. Select the 'Desktop development with C++'
1. Complete the installation

## Installing Qt Libraries

1. Download the [Qt installer](https://www.qt.io/download-qt-installer)
1. Run the installer.
1. Select 'custom installation'
1. Install (at a minimum):
  * Qt 5.15.2 > MSVC 2019 64-bit
  * Developer and Design Tools > Qt Creator CDB Debugger Support
  * Developer and Design Tools > Debugging Tools for Windows
  * Developer and Design Tools > Qt Installer framework (optional if you want to build the installer)

# Cloning the Notepad Next Repository

1. In a command prompt (or git shell, powershell, etc) run:
1. `git clone --recurse-submodules https://github.com/dail8859/NotepadNext.git`
1. `cd NotepadNext`
1. `git checkout dev`


# Building/Running Notepad Next

1. Open `src/NotepadNext.pro` with Qt Creator
1. Configure the project for 'Desktop Qt 5.15.2 MSVC2019 64bit'
1. Press `Ctrl+R`
1. Qt Creator will build and run the project.