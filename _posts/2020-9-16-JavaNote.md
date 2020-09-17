---
title: Reading notes on Core Java 7th edition. Volume I
date: 2020-09-16 10:41:53
category: 
- Reading Notes
tags:
- Java
---
# Reading notes on Core Java 7th edition. Volume I

Here I will post some important information in the book.   

## Chapter 1, 2
(No important content)  

## chapter 3
Data types
- Like C/C++, Java use `""` for strings.  
- number notation: suffix `L/l` for long integer, prefix `0` for octal number, `0x/0X` for hexadecimal, `0b/0B` for binary(after Java 7).
- cannot convert between integers and boolean values. So C-style snippets such as `int x = 1; if(x) {...}` is not supported.

Variables and Constants
- java use `final` keyword for *constant variables*.

Operators
- integer division by 0 raises an exception, whereas floating-point division by 0 yields an infinite or NaN result.
- a cast (auto promote) will happen implicitly when carry out a binary operation such as `+`.
- Don't use `==` to test equality of two Strings (and surely any Objects, as we will see later)

Arrays
- simply assign an array to another will lead two variable point to same array object. Use `Array.copyOf()` instead.
- Use `System.out.println(Arrays.deepToString(arr));` to print a nested array (an array with 2 or more dimensions)

## chapter 4
Introduction to Object-Oriented Programming
- Try to minimize the number of classes that depend on each other. In software engineering terminology, minimize the *coupling* between classes.
