---
title: solvataire
date: 2024-03-03T22:03:09-04:00
description: a brute-force solver for the game Peg Solitaire in Rust. 
summary: a brute-force solver for the game Peg Solitaire in Rust. 
tags: ['rust']
author: kyle Kincer
toc: false
readTime: true
autonumber: false
---
### a peg solitaire solver
if you're anything like me, you've been called an [**eg-no-ra-moose**](https://blog.crackerbarrel.com/2021/08/13/how-to-beat-the-cracker-barrel-peg-game/) by that silly peg game at Cracker Barrel one too many times. i'd had enough.

Solvataire is a brute-force solver for the game [Peg Solitaire](https://en.wikipedia.org/wiki/Peg_solitaire), written in Rust. it uses a recursive depth-first search to solve the game. it's currently only implemented for the triangle board commonly found at Cracker Barrel™️  restaurants, but i plan to support the English boards at some point. 

### links
- [GitHub](https://github.com/KyleKincer/solvataire)

## implementation
### algorithm
the solver uses a recursive backtracking algorithm to find the shortest sequence of moves to solve the game. it starts with an initial board state and explores all possible moves from that state, recursively searching until it finds a solution. 

### performance
the solver is multithreaded, using Rust's `rayon` library to parallelize the search. 
