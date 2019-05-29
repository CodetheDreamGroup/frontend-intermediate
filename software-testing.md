---
author: Jared Siirila
title: Software Testing
---

# Software Testing

---

## What is Testing?

The process of executing software to ensure that the results match
the specification.

--

It is usually impossible to completely test a piece of software for all possible inputs and outputs.  

Instead, testing usually focuses on a subset of possible inputs and outputs.

---

# Types of testing

--

## Black box testing

In black box testing, the tester has no visibility to the code (hence black box).  

--

This type of testing typically uses the *specification* for the software to test that
it produces the expected output given a set of inputs.  

Usually black box testing is done by somebody other than the developer who wrote the software.

When a defect is found with black box testing, the tester much report it back to the development 
team who can look at the code to try to fix the problem.

--

## White box testing

In white box testing the internal structure of the code is known

--

Since the structure of the code is known, tests can be written to test specific paths within the code.  

This can be useful to ensure that all the paths within the code get tested, 
where-as with black box testing you can't know if all paths in the code were tested.

---

# Testing levels

--

There are many different levels that software can be tested at, 
from individual functions all the way to an entire program or group of programs together.  

Here is one way to break them down.

--

![Testing Pyramid](/images/TestingTriangle.png)

--

### Unit tests

Test the smallest testable piece of an application.  

Typical units for testing are *functions* or *objects*.  

Uses *white box* testing because you need to know how the code is structured to test an individual unit.

Written by programmers; frequently by the same programmers who wrote the unit under test.

--

### Integration tests

Sit between end to end tests and unit tests.  

Tests the integration of multiple systems, such as classes, modules, functions, etc.  

Can be *white box* or *black box*, but more often these are *white box* tests.

--

### UI/ End 2 End (E2E) tests

Test a product as a whole.

Almost exclusively *black box* testing is used for E2E testing.

--

For this class, we will focus mostly on unit testing.

---

# Unit test example

--

The goal with unit testing is to test all of the specified behavior for a small unit of code.

For now, we will focus on a *function* as the unit to test.

--

Example: The zip function

The zip function takes two arrays and returns a new array with the items from each input array alternating.

e.g. given [1, 2] and ['a', 'b'] the zip function would return [1, 'a', 2, 'b']

* If the arrays are different lengths, zip stops as soon as the end of one of the arrays is reached

--

How would you write tests for this example.  

There are some good tools that can help us write tests that will cover most cases including.

* Include all known edge cases
* Include some simple cases
* Consider what could go wrong

---

# Let's try another

--

Array.sort

The sort() method sorts the elements of an array in place and returns the array.  

The default sort order is built upon converting the elements into strings, then comparing their sequences of UTF-16 code units values.

To keep it simple, we will only deal with string sorting in alphabetical order.

--


