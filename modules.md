---
author: Jared Siirila
title: Modules
---

# Modules

---

Keeping all of your code in a single file get confusing really quickly

--

Which section of the file contains which piece of functionality?

--

It makes it hard to collaborate since everyone is editing the same file?

--

How would you run different pieces of functionality by themselves to test themselves?

--

How do you run tests independent of the code they are testing?

--

JavaScript modules to the rescue...

---

## Benefits of Modules

--

### Encapsulation  

Hide access to module internals such as variables

--

## Abstraction

Hide details so you can work at a higher level

--

## Reusability

Reuse modules repeatedly in a project

Reuse modules between projects

--

## Separation of Concerns

Different teams/people can work on different modules

Teams can share code between each other with modules

---

## One Problem

--

JavaScript didn't have a module system originally...

--

Code could be split up between files to load multiple files in a webpage

--

but everything in those files lived in the same global scope

--

So if two different files both declared variables with the same name,
whichever one was ran second would 'win'

---

## Enter JS Module systems

--

The JS community recognized this problem, and created solutions for it

* Immediately Invoked Function Expressions (IIFEs)
* Asynchronous Module Definition (AMD)
* CommonJS modules

--

But the different module systems created didn't work with each other

--

And none of them worked in the browser without additional JS files to run them

--

Eventually with the introduction of ES6 (a newer version of JavaScript),
the language defined it's own module system

* ES6 modules

--

**Yay**

...
<!-- .element: class="fragment" -->

...
<!-- .element: class="fragment" -->

--

Except, the Cloud 9 system you are working on uses an older version of Node JS that only supports CommonJS modules

So that is what we will use today

--

Later we will go over ES6 modules, but the concepts between the two are pretty much the same

---

## CommonJS

--

In CommonJS, and ES6 modules also, each file is a separate module.

By default, anything declared in a file is only accessible in that file.

--

The two basic elements of CommonJS modules are

* `require` - Used to include other modules in a file
* `exports` - Used to export code from a module to require in another file

---

## Examples
