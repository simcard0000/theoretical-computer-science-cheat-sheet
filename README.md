![active development](https://img.shields.io/badge/active%20dev-yes-brightgreen.svg)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/simcard0000/theoretical-computer-science-cheat-sheet.svg)
# theoretical-computer-science-cheat-sheet
🧮 An expanded version of Steve Seiden's Theoretical Computer Science Cheat Sheet.

### Table of Contents
1. [About + Credits](#about--credits)
2. [Contributing](#contributing)
3. [How do I unpack a TAR file in Windows?](#how-do-i-unpack-a-tar-file-in-windows)
4. [Theoretical Computer Science Cheat Sheet - Extended](#theoretical-computer-science-cheat-sheet---extended)
    1. [Definitions of Asymptotic Notation](#definitions-of-asymptotic-notation)

### About + Credits
Dr. Steven Seiden was an Associate Professor of Computer Science at Louisiana State University, and an alumnus of UC Irvine. He created the original "Theoretical Computer Science Cheat Sheet" - a condensed document of definitions, identities, and theorems that's been helpful in competitive programming events and courses like the University of Waterloo's [CS240](https://cs.uwaterloo.ca//current/courses/course_descriptions/cDescr/newCDescr/CS240) (yes, I have taken that class 💀). 

The purpose of this repository is to make the original PDF file (and the TeX files used to generate the PDF) more accessible; as well as to create a version in Markdown with extended information. The cheat sheet was originally available to download at: http://bit.csc.lsu.edu/~seiden/#cheat (the link is dead now). On this website were the following permissions from Dr. Steven Seiden:

> I grant permission for you to reproduce this cheat sheet, and redistribute it for educational purposes only. You may not reproduce it for profit. If you reproduce it, you must not alter or delete my copyright.

This cheat sheet was also submitted to the [TeX Showcase](https://www.tug.org/texshowcase/) on the TeX Users Group (TUG) site, by Martin Jansche. Here are his latest updates: 

> * GW 2003: I have been informed that it's author, Steve Seiden, died in 2002 as the result of an accident while riding his bike. As I cannot ask for permission anymore, I have taken the liberty of fixing errors reported to me. 
> * GW 2013: I have been informed by Raphael Reitzig of two errors, which have been fixed (notes in the `.tex` files)
> * GW 2016: The current distribution does not properly compile, Escher's Knot is missing. I include a fixed pdf, but the source still needs repairing. Help welcome. 

### Contributing
Feel free to raise an [issue](https://github.com/simcard0000/theoretical-computer-science-cheat-sheet/issues) if you find an error, if you would like to see something added to the extended notes, and if you have any fixes/optimizations to the `.tex` files for the cheat sheet.

### How do I unpack a TAR file in Windows?
TAR stands for "Tape ARchive", and `.tar` files are pretty common in Unix/Linux systems. Compressed `.tar` files can have `.tar.gz` or `.tar.bz2` extension names.
If you have [Cygwin](https://www.cygwin.com/) or [MinGW](https://www.mingw-w64.org/)/[MSYS](https://www.msys2.org/) installed, the basic unpacking commands are as follows:
```
  tar xvf  <.tar file>
  tar xzvf <.tar.gz file>
  tar xjvf <.tar.bz2 file>
```
For more information, [check out this page on the Haskell Language Wiki](https://wiki.haskell.org/How_to_unpack_a_tar_file_in_Windows).

### Theoretical Computer Science Cheat Sheet - Extended
This part is currently under construction!
#### Definitions of Asymptotic Notation
* big-O (big-"O"):  $f(n) = O(g(n)) \iff  \exists $ positive $c, n_0$ such that $0 \leq f(n) \leq cg(n)\,\forall n \geq n_0$
* big-Ω (big-"Omega"):  $f(n) = \Omega(g(n)) \iff  \exists $ positive $c, n_0$ such that $f(n) \geq cg(n) \geq 0\,\forall n \geq n_0$
* big-Θ (big-"Theta"): $f(n) = \Theta(g(n)) \iff f(n) = O(g(n))$ and $f(n) = \Omega(g(n))$

