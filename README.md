# programming-challenges

**[WIP]**
My collection of programming challenges, covering many CS topics - made and curated by me.

## What's this?
This is meant to be a list of coding challenges for those who want to improve their skills. I have separated the problems by topic and put them in a increasing level of difficulty. Most of those were university assignments for me, but some of them I haven't solved yet.

If you want to improve your at coding, I suggest you try one of these, and if you have any suggestions on changes or things that can be added to this list, please open an issue. You're welcome to collaborate.

## How do I do this?

- search about the problem as much as you can. This is the part where you actually learn. Use Google, Wikipedia, Stack Overflow. Sometimes you're better off resorting to theoretical books, but there's plenty of free material online you can use;

- pick a language;

- implement it;

- be proud of it! yay

# Topics

## The essential

These are typically topics you'd be introduced to in the first or second year of a university computer science degree. That doesn't mean they're easier, it just means that they're foundational and have little to no prerequisites aside from elementary to high school math. If you're just starting, I recommend you pick these up first.

### Algorithms

- **Easy**: count how many times a character appears in a string. Bonus points for supporting unicode.

- **Easy**: Bubble Sort

- **Easy**: binary search

- **Average**: crack a DES-encrypted password (up to 6 characters) by brute forcing it

- **Average**: Quick Sort

- **Average**: Dijkstra's algorithm

- **Hard**: DFA-based string matching

- **Hard**: External Quicksort (use binary temporary files), test it with 100k+ elements

- **Hard**: Given a grid map with walls, empty spaces and portals with a given destination on the map, which disappear once you enter them, write a modified version of Dijkstra's algortihm to find the shortest path between two positions in the grid.

- **Extra**: External Quicksort, but multithreaded. Make some scheduling to make sure there are no race conditions.

### Computer Architecture

- **Easy**: use an HDL to design a chip that does addition and multiplication.

- **Easy**: use an HDL to design a chip that with an operation that decides if a number is prime or not (don't worry about complexity)

- **Average**: pick an assembly language and make an assembler for it. Ignore the memory load/store instructions, just work with immediates

- **Average**: design a CPU for your assembly language in an HDL

- **Hard**: add memory instructions and caching.

- **Hard**: make a parallel instruction pipeline for the your CPU (fetch -> decode -> execute -> write-back)

- **Extra**: make it multicore. Remember to enforce the cache coherence.

### Data Structures

- **Easy**: convert an array of numbers to a heap tree

- **Easy**: convert an array of numbers to a binary search tree (not necessarity balanced)

- **Average**: a tree-based dictionary that searches for words in a text and sees if they're being repeated. If one word is missing in the tree, add it iteratively

- **Average**: a program that stores strings in a way that would make them easy to search for. Use a hash and solve conflicts with arrays.

- **Hard**: same as above, but use a balanced binary tree to solve the conflicts instead, so the conflict search is O(log n)

- **Hard**: do the dictionary, but use radix trees instead

- **Extra**: manage files in a directory with a B-tree. Implement search, insertion and deletion

### Discrete Mathematics and Algebra

- **Easy**: iterative factorial function (don't use recursion)

- **Easy**: Euclid's algorithm (find the greatest common divisor of two integers)

- **Easy**: find out if a graph is connected

- **Average**: Hamiltonian path in a graph

- **Average**: find out if the input integer is prime using Fermat's little theorem

- **Average**: find out a given integer's N partitions. In other words, find out all combinations of N distinct integers that sum up to the input integer.

- **Hard**: RSA encoder and decoder (get key as input)

- **Hard**: solve a system of congruences with the Chinese remainder theorem

- **Hard**: first-order diophantine equation solver

- **Extra**: [Project Euler 651](https://projecteuler.net/problem=651)

### Linear Algebra

- **Easy**: vector lerp

- **Easy**: vector dot and cross product

- **Easy**: matrix multiplication

- **Average**: linear algebra library including the operations above, plus affine transformations (rotation, translation, scale)

- **Average**: matrix trace and determinants

- **Average**: linear system solver with Gaussian elimination

- **Hard**: SVD operator

- **Hard**: linear algebra library including the operations above, plus projective transformations

- **Hard**: conic section area calculator

- **Extra**: optimize matrix multiplication with concurrence

### Numerical Analysis

- **Easy**: linear interpolation for a set of points

- **Easy**: basic numerical integration (divide the function area in rectangles)

- **Easy**: linear regression

- **Average**: find the n-root of a number

- **Average**: LU factorization of a matrix

- **Average**: approximate the first 1000 digits of PI

- **Hard**: numerical integration using Simpson's rule

- **Hard**: Hermite interpolation for a set of points

- **Hard**: choose a numerical ODE method and implement it

- **Extra**: choose a numerical PDE method and implement it

### Probability and Statistics

### Theory of Computation and Formal Languages

## Advanced topics

Those are usually what you'd get in the mid-to-final years of the undergraduate studies. Those topics assume you have knowledge of the previous ones, and might be more convoluted than the foundations, as in, they require some more previous knowledge.

### Artificial Intelligence

Rec: Algorithms, Data Structures, Probability and Statistics

### Compilers and Programming Languages

Rec: Theory of Computation and Formal Languages

### Databases

Rec: Data Structures

### Graph Theory

Rec: Algorithms, Discrete Mathematics and Algebra

### Machine Learning

Rec: Linear Algebra, Numerical Analysis, Probability and Statistics

### Networking

Rec: Algorithms, Data Structures, Computer Architecture

### Operating Systems

Rec: Algorithms, Data Structures, Computer Architecture

### Optimization and Operations Research

Rec: Discrete Mathematics and Algebra, Linear Albegra

## Specializations

Those topics are usually opt-in. That means they're not for everyone and some of them may be interdisciplinary subjects or use very specific techniques. The pre-requisites for each one may vary drastically. I assume that if you're getting into one of these branches, you should know exactly what you need.

### Computer Geometry

### Computer Vision and Image Processing

### Emulation

### Games

### Graphics

### Heuristic Optimization and Meta-heuristics

### Information Theory

### Simulations

# Observations

I might have overlooked some topics that I'm not familiar with, but I'm open to suggestions. If you have any, just open an issue.
