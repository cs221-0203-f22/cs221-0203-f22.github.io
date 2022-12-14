---
layout: assignment
due: 2022-09-20 23:59:59 -0800
permalink: assignments/lab03.html
title: Lab03 - Files, error handling
github_url: https://classroom.github.com/a/qiE0w-Re
---

## Background

In C, it's very important to be careful when allocating memory, copying data between buffers, and working with files. In this lab, we will explore some common error handling techniques.

## Requirements

1. You will develop a C program named `lab03` which 
    1. takes a filename and the name and quantity of a product for stock-keeping
    1. writes a comma-separated list of the data out to the file.
1. Each product will have a name (at most 15 chars and a NUL) and quantity (an integer), and you will keep those in one or more C `struct`. It's possible to generate the output without structures but please learn to use structures
1. You will use the C file management functions to open, write, and close the CSV file
1. You will handle error conditions **exactly** as shown in the example output
1. You will provide a `Makefile` and test your project with the `grade` script

## Given

1. I will discuss and demo the C file management functions in lecture.

## Example Output
```sh
phpeterson@vlab20:lab03 $ ./lab03 lab03.csv
usage: lab03 filename 'name qty' ['name qty']

phpeterson@vlab20:lab03 $ ./lab03 lab03.csv 'apples 20' 'oranges 10'
phpeterson@vlab20:lab03 $ cat lab03.csv
name,quantity
apples,20
oranges,10

phpeterson@vlab20:lab03 $ ./lab03 lab03.csv 'apples 20' 'oranges asdf'
not a number: asdf

phpeterson@vlab20:lab03 $ ./lab03 lab03.csv "cinnamonapplessauce 10"
string overflow: cinnamonapplessauce 10

phpeterson@vlab20:lab03 $ ./lab03 /usr/bin/lab03.csv 'apples 20' 'oranges 10'
failed to open: /usr/bin/lab03.csv
```

## Rubric
1. Your lab will receive the score shown by the autograder
1. Deductions may be made if your code does not meet the above requirements
