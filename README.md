ThinkDSP
========

LaTeX source and Python code for _Think DSP: Digital Signal Processing in Python_, by Allen B. Downey.

The premise of this book (and the other books in the _Think X_ series) is that if you know how to program,
you can use that skill to learn other things.  I am writing this book because I think the conventional
approach to digital signal processing is backward: most books (and the classes that use them) present
the material bottom-up, starting with mathematical abstractions like phasors.

With a programming-based approach, I can go top-down, which means I can present the most important
ideas right away.  By the end of the first chapter, you can
break down a sound into its harmonics, modify the harmonics, and generate new sounds.

### Run the code for this book on Binder: [![Binder](http://mybinder.org/badge.svg)](http://mybinder.org/repo/AllenDowney/ThinkDSP)

This is a work in progress, so comments are welcome.

The book is under a Creative Commons license:

Attribution-NonCommercial-ShareAlike 3.0 Unported 
http://creativecommons.org/licenses/by-nc-sa/3.0/

The code is under the GNU GPL:
GNU GPLv3 http://www.gnu.org/licenses/gpl.html

### Code dependencies

Including IPython notebook through jupyter:

```
virtualenv venv
source venv\bin\activate
pip install numpy scipy matplotlib pandas jupyter
```

As on ArchLinux with AUR:

```
yaourt -S --needed python-numpy python-scipy python-matplotlib python-pandas jupyter
```

On Windows it's harder to install scipy. Install the others first. Download from [Unofficial Windows Binaries for Python Extension Packages](http://www.lfd.uci.edu/~gohlke/pythonlibs/#scipy) according to the environment, rename the downloaded .zip to .whl then install:

```
pip install numpy matplotlib pandas jupyter
pip install scipy-0.16.1-cp35-none-win_amd64.whl
```

### Book dependencies

As on ArchLinux with AUR:

```
yaourt -S --needed texlive-most texlive-lang hevea evince
```
