---
layout: assignment
due: 2022-10-04 23:59:59 -0800
permalink: assignments/lab04.html
title: Lab04 - Tic-Tac-Toe
github_url: https://classroom.github.com/a/Je3oHxb_
---

## Requirements

1. You will write a C program called `lab04` and provide a `Makefile` to implement a rudimentary Tic-Tac-Toe game
1. Your program will accept input from the command line specifying Row and Column inputs to the Tic-Tac-Toe board. 0 0 is the upper left and 2 2 is the lower right.
1. Your program will identify win and draw patterns on the board.

## Given

1. In lecture we will discuss the basics of the game, including alternating turns, making legal moves, and detecting a win.
1. We will learn several new C language features, including two-dimensional arrays, `typedef`, C library functions to accept input while your program is running.

## Example Output

```sh
$ ./lab04 _ _ _ _ _ _ _ _ _
 _ | _ | _
---+---+---
 _ | _ | _
---+---+---
 _ | _ | _

$ ./lab04 X X X X O X O X O
 X | X | X
---+---+---
 X | O | X
---+---+---
 O | X | O
X wins

$ ./lab04 X O X O X O O X O
 X | O | X
---+---+---
 O | X | O
---+---+---
 O | X | O
draw
```

## Rubric
1. Your score will be as indicated by the autograder