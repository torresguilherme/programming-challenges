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

- **Easy**: calculate the mean, median, variance and standard deviation for a given array of samples

- **Easy**: combinatorial probability calculator

- **Easy**: given a function, find out numerically if it's a PDF (probability density function)

- **Average**: Poisson distribution calculator

- **Average**: make a tiny US election poll simulator, given a number of N states where x% are republicans and y% are democrats, given a random K people sample for each state, output the probability of each state having the most republicans

- **Average**: given a shape in a given rectangular area, use a Monte Carlo method to determine the approximate area of this shape

- **Hard**: given a distribution, calculate the Bayes estimator

- **Hard**: general regression analysis software

- **Hard**: graphical conditional probability calculator. Insert nodes with given probabilities and calculate the probability of a given ocurrence

- **Extra**: make a US election poll simulator. Assume that each state has 10 million votes, "interview" K voters from each state and find out if they're democrats or republicans. Calculate the estimated chance of a democrat or republican victory. Use your disk to help with the large volume of data. 

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

### Cryptography and Security

### Exact Exponential Algorithms and Parametrized Complexity

- **Easy**: solve the Travelling Salesman Problem with a non-combinatorial algorithm

- **Easy**: knapsack problem with dynamic programming

- **Average**: implement an algorithm that solves graph coloring with a complexity lesser than O(2^n) (yes, it's possible. remember that unless NP = P, the complexity must be exponential, but the basis can be a number k such that 1 < k < 2)

- **Average**: given a vertex covering problem instance, find the complexity of the kernel and solve it with an FPT algorithm

- **Hard**: solve the d-hitting set with a sunflower-based kernel

- **Hard**: pick an NP-hard problem of choice and implement a treewidth-based FPT algorithm for it

- **Extra**: develop a randomized algorithm for the vertex cover problem. You should use a FPT transformation and calculate a number of executions such that the probability of your algorithm failing is less than the probability of a meteor destroying your computer during the execution (you can assume that number is, say, 0.000001). tip: use the property: 1 + x <= exp(x) for every x >= 0.

### Games

### Graphics

- **Easy**: a triangle in your graphics API of choice. When you click the screen, rotate the triangle clock-wise around the cursor

- **Easy**: spinning 3D cube. Shading is optional

- **Easy**: render a teapot in a scene with a point light. Use a Phong BRDF, with specular reflection. Bonus: use both flat, Gouraud and Phong shading, and compare the results

- **Average**: animate a character with shape interpolation

- **Average**: brute-force CPU ray tracer. Make ray-sphere and ray-triangle intersection (note: this is embarassingly parallel, and if you don't make it concurrent, your program will be orders of magnitude slower)

- **Average**: PBR shader. Bonus: add ambient occlusion

- **Hard**: pick a real-time global illumination method of choice and render a scene with it

- **Hard**: space-optimized GPU ray tracer.

- **Hard**: real-time terrain editor. Use an implicit modelling algorithm like dual contouring

- **Extra**: GPU path tracer

### Metaheuristics

- **Easy**: find a "decent" solution to the Travellng Salesman Problem by searching the space for local minima

- **Easy**: given a set of input vectors A_i and scalars b_i, use a genetic algorithm to estimate a function f such that f(A_i) ~= b_i. Use as many operators as you please.

- **Average**: approximation algorithm of Christofides and Serdyukov for the Travelling Salesman Problem

- **Average**: solve graph coloring with a Taboo search

- **Hard**: general simulated annealing solver 

- **Hard**: pick a multiobjective optimization problem and a metaheurisic of choice, implement it from scratch

- **Extra**: general heuristic multiobjective solver

### Information Theory

### Simulations

- **Easy**: make a 2D breakout game, brute force collisions

- **Easy**: space-optimized raycast. 

- **Easy**: Conway's Game of Life

- **Average**: 2D Noita-style particle simulator using cellular automata

- **Average**: Foucault pendulum

- **Average**: FLIP fluid simulation without incompressibility

- **Hard**: FLIP with incompressibility

- **Hard**: full real-time physics engine. Simulate bouncy materials, elastic properties and mechanical energy

- **Hard**: a simple molecular dynamics simulator 

- **Extra**: celestial mechanics engine

# Observations

I might have overlooked some topics that I'm not familiar with, but I'm open to suggestions. If you have any, just open an issue.
