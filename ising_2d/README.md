Worm algorithm for the two-dimensional Ising model
(implementation based on http://mcwa.csi.cuny.edu/umass/izing/Ising_text.pdf).

### python version (worm_ising_2d.py)
Written in pure Python, so that it can be run through pypy.

### C version (worm_ising_2d.cpp)
Requires mt19937ar.c, and has to be compiled via

    make worm_ising_2d


### Known bugs:
* the C code does not run for large L (you can move some declarations outside the main) a preliminary bugfix (not on this repository yet) has troubles with the bond/nbr arrays.

### To-do
* add correlation function measure (which also gives access to magnetic susceptibility),
* add magnetization measure (how?),
* find a smarter way of labelling bonds (in the C version).
