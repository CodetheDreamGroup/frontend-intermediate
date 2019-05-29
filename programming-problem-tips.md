---
author: Jared Siirila
title: Programming problem tips and tools
---

# Tips for solving programming problems

---

# Similarity to math word problems

--

Solving programming problems is a lot like solving math word problems

--

Many of the same strategies can be used

--

Lets revisit math word problems for a moment

--

![Billy Madison](/images/billy-madison.jpeg)

---

# Word problem tools

--

Read it carefully

What is being asked?
<!-- .element: class="fragment" -->

Mark up the relevant information (ignore irrelevant information)
<!-- .element: class="fragment" -->

Break it down in to the individual steps
<!-- .element: class="fragment" -->

---

# Example Word problems

--

There was a nest of fish eggs in Brookfield River; 302 of the eggs hatched and 114 of them didn't. How many eggs were there in total?

total suggests addition
<!-- .element: class="fragment" -->

Relevant numbers are 302 and 114
<!-- .element: class="fragment" -->


--

Newberry Publishing needs to ship 48 new math textbooks to a high school. If each box can hold 8 textbooks, how many boxes will the publisher need?

Relevant values are 8 and 48
<!-- .element: class="fragment" -->

Each could mean multiplication or division, it requires careful reading to determine it is division in this case
<!-- .element: class="fragment" -->

--

Erik saved $21 in March. He saved $19 in April and $30 in May. Then Erik spent $38 on a keyboard. How much money does Erik have left?

spent and left suggest subtraction
<!-- .element: class="fragment" -->

saved suggest addition
<!-- .element: class="fragment" -->

relevant numbers are $21, $19, $30, and $38
<!-- .element: class="fragment" -->

---

# Programming problems

--

Programming problems tend to follow the same rules for how to solve them

--

Read them carefully
<!-- .element: class="fragment" -->

What is being asked?
<!-- .element: class="fragment" -->

What information is relevant?
<!-- .element: class="fragment" -->

What information is irrelevant or misleading?
<!-- .element: class="fragment" -->

Identify the tools you might use to solve the problem
<!-- .element: class="fragment" -->

---

# Tips for identifying tools

--

* each
* every
* iterate
* count
* all
* list

All of these words tend to indicate that some form of **iteration** will need to be used
<!-- .element: class="fragment" -->

That could be a for loop, a while loop, the foreach method, or something else
<!-- .element: class="fragment" -->

--

* compare
* if
* only
* when
* tests

These tend to indicate some sort of **comparison**
<!-- .element: class="fragment" -->

Usually, that is an *if/else* statement, but it could be a the condition for a loop or some other comparison
<!-- .element: class="fragment" -->

--

* returns
* outputs
* input
* takes
* arguments

These tend to indicate use of a **function** or **method**
<!-- .element: class="fragment" -->


--

# Practice problems

--

Given a list of numbers, return the largest number in the list

--

Given two numbers, return true if they have the same value and false otherwise

--

Given a list of prices, compute the total of all of the prices

--

Given a number, return an array of each digit in the number

--

Given two lists, return a new list that has all of the items from each list alternated

e.g. [1, 2, 3] and ['a', 'b', 'c'] would return [1, 'a', 2, 'b', 3, 'c']


---