---
author: Jared Siirila
title: NPM Packages
---

# NPM

--

## What is NPM

--

A JavaScript software package registry

and
<!-- .element: class="fragment" -->

A command line tool to install and use packages from the registry
<!-- .element: class="fragment" -->


--

The registry is at http://www.npmjs.com

---

## Installing NPM packages

--

Use the command `npm install <package name> --save` to install an npm package in a project

--

When this command is run, the specified package is downloaded form the npm registry and 
installed in the *node_modules* folder within the directory the command was run

--

The *save* portion of the command tells npm to save the information about what was installed 
in a *package.json* file in the same folder

We will take a look at one of these files in a few minutes

--

When you install a package, it installs all of the other packages that the original package depends on

This can quickly grow to hundreds of packages in the node_modules folder, even if you only installed a few packages

--

How does it know which packages the installed package depends on?

It uses the *package.json* for the installed package to determine that information

---

## Types of packages are on NPM

--

The npm registry contains all kinds of different packages including

--

Small packages containing one or just a few functions

* [Dedupe](https://www.npmjs.com/package/dedupe) - removes duplicate values from an array
* [Uuid](https://www.npmjs.com/package/uuid) - get a unique identifier
* [Better title case](https://www.npmjs.com/package/better-title-case) - convert a string to title case

--

Libraries that contain many functions and methods that work well together

* [lodash](https://www.npmjs.com/package/lodash) - A ton of useful functions for working with data
* [jQuery](https://www.npmjs.com/package/jquery) - The library for browser DOM operations
* [Mathjs](https://www.npmjs.com/package/mathjs) - An extensive math library

--

Command line tools

* [Vaca](https://www.npmjs.com/package/vaca) - ASCII cow
* [Http-server](https://www.npmjs.com/package/http-server) - A super simple HTTP server
* 

--

Frameworks for development

* [React](https://www.npmjs.com/package/react) - A framework for web development
* [Ember](https://www.npmjs.com/package/ember) - Another web development framework
* 
