---
author: Jared Siirila
title: Writing Unit Tests and Test Driven Development
---

# Unit Tests and Test Driven Development

---

## Unit Tests

--

Test the smallest testable piece of an application

--

Unit tests are also code. Code that executes the other code and verifies that it gets the expected results

--

Written by programmers; frequently by the same programmers who wrote the unit under test

--

They can be written at any time when developing, but when doing *Test Driven Development* they should be written before writing the code they are testing.

--

![Confused](/images/confused-coder.jpg)

---

## Test Driven Development

--

Is not really about testing

It is about design and development
<!-- .element: class="fragment" -->

It is about developing incrementally
<!-- .element: class="fragment" -->

--

### 3 steps to TDD

1. Write a failing unit test
<!-- .element: class="fragment" -->

2. Write the code that makes the unit test pass
<!-- .element: class="fragment" -->

3. Refactor as needed, making sure all tests still pass
<!-- .element: class="fragment" -->

4. Repeat with another test case as needed
<!-- .element: class="fragment" -->

--

## Writing Unit Tests and TDD

--

We will use the zip method that we created test cases for in the previous class

These are the test cases we wrote for the zip method (I added some additional ones)

--

* Should return an array

--

* Should return a single array containing all items from two equal length arrays
    * [1, 2] and ['a', 'b'] returns [1, 'a', 2, 'b']
    * [1] and ['a'] returns [1, 'a']

--

* When the first array is longer than the second array, return the correct zipped array that contains all elements from the second array
    * [1, 2] and ['a'] return [1, 'a']

--

* When the first array is shorter than the second array, return the correct zipped array that contains all elements from the first array
    * ['hello', 'world] and [3, 5, 7, 11, 13] returns ['hello', 3, 'world' 5]

--

* When the first argument is an empty array, returns an empty array
    * [] and [1] returns []

--

* When the second argument is an empty array, returns an empty array
    * [1, 2, 3] and [] returns []

--

* Works with arrays of mixed types
    * [1, 'hello', [42, 100]] and [2, 'world', [24, 13]] returns [1, 2, 'hello', 'world', [42, 100], [24, 13]]

--

* Throws an error when the first parameter is not an array
    * 'hello' and [1, 3] throws a TypeError

--

* Throws an error when the second parameter is not an array
    * ['hello'] and 3 throws a TypeError

--

* The items should be zipped correctly, the items in the first array should come before the items in the second array
    * [1, 2] and ['hello', 'world] returns [1, 'hello', 2, 'world'] not ['hello', 1, 'world', 2]

--

