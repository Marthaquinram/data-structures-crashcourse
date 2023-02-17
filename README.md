# Data Structures crash course

In the context of interviews from Algoexpert.io

## What are Data Structures?

- a collection of data values, the relationship among them, and the functions and operations that can be applied to the data.
  - 1 -> 2 -> 3 -> 4
  - [ foo, interview, coding, practice ]

## Complexity Analysis

- The process of determining how efficient an algorthm is. Complexity analysis usually involves find both the **time complexity** and **space complexity** of an algorithm. Complexity analysis is effectively used to determine how "good" an algorithm is and whether its "better" than another one.

- What makes a solution better than another?
  - The complexity
    - Time Complexity - measure how fast an algorith or a solution runs. Its expressed using Big O
    - Space Complexity - measure of how much memory or space an algorithm uses up. Its expressed using Big O
- The faster the algorithm runs the better the time complexity is, the less memory and space the better the space complexity is.

## Memory

- Memory is the founational layer of computing, where all data is sorted.

Bit

- Short for binary digit, a nit is a fundamental unit of information in Computer Science that represents a state with one of two values, typically 0 and 1.
  Any data stored in a computer is, at the most basic level, represented in bits.

Byte

- A group of eight bits. For example, 01101000 is a byte.
  A signle byte can represent up to 256 data values (2^8).
  Since a binary number is a number expressed with only two symbols, like 0 and 1, a byte can effectively represent all of the numbers between 0 and 255, inclusive, in binary format.
  - 1: 0000 0001
  - 2: 0000 0010
  - 3: 0000 0011
  - 4: 0000 0100

## Big O Notation

The notation used to describe the **time complexity** and **space complexity** of algorithms.
Variables used in Big O notation denote the sizes of inputs to algorithms. For example, **O(n)** might be the complexity of the algorithm that traverses through an array of length n; similarly, **O(n + m)** might be the complexity of the algorithm that traverses through an array of length **n** and through a string of lengthn **m**.
Examples of common complexities and their Big O notation, ordered from fastest to slowest:

- **Constant:** O(1)
- **Logarithmic:** O(log(n))
- **Linear:** O(n)
- **Log-linear:** O(nlog(n))
- **Quadratice:** O(n^2)
- **Cubic:** O(n^3)
- **Exponential:** O(2^n)
- **Factorial:** O(n!)

![bigO](./assets/BigO.jpeg)
From: <https://www.freecodecamp.org>

- In the context of coding interviews, Big O notation is usually understood to descrive the **worst-case** complxity of an algorithm, even though the worst-case complexity might differ from the **average-case** complexity.

Some sorting algorithms have different time complexities depending on the layout of elements in their input array. In rare cases, their time complexity will be much worse than in more common cases. Similarly , an algorithm that takes in a string and performs special operations on uppercase characters might have different time complexity when run on an input string of only uppercase characters vs. on an input string with just a few uppercase characters.
When describing the time complexity of an algorithm, it can sometimes be helpful to specify whether the time complexity refers to the average case or to the worset case (e.g, "this algorithm runs in O(nlog(n)) time on average and in O(n^2) time in the worse case").

## Logarithm

If an algorithm has a logarithmic time complexity(O(log(n))), where n is the size of the input) then whenever the algorithms input doubles in size (i.e whenever n doubles), the number of operations needed to complete the algorithm only increases by one unit. Conversely, an algorithm with a linear time complexity would see its number of operations double if its input size doubled.

## Arrays

Accessing a value at a given index: O(1)
Updating a value at a given index: O(1)
Inserting a value at a given beginning: O(n)
Inserting a value in the middle: O(n)
Inserting a value at the end:

- amortized O(1) when dealing with a dynamic array
- O(n) when dealing with a static array
  Removing a value at the beginning: O(n)
  Removing a value in th emiddle: O(n)
  Removing a value at the end: O(1)
  copying the array: O(n)

get => i.e array[2] => O(1)
set => i.e, array[2]= 5 => O(1)
