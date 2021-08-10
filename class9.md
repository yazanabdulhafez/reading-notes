# FUNCTIONAL PROGRAMMING

## Functional Programming Concepts

1. What is functional programming?
**is a programming paradigm where programs are constructed by applying and composing functions.**
2. What is a pure function and how do we know if something is a pure function?
**pure functions have no side-effects or hidden I/O, programs built using functional paradigm are easy to debug. Moreover, pure functions make writing concurrent applications easier.**
3. What are the benefits of a pure function?
**When the code is written using the functional programming style, a capable compiler is able to:**

* Memorize the results
* Parallelize the instructions
* Wait for evaluating results

4. What is immutability?
**Variables are immutable i.e. it isn’t possible to modify a variable once it has been initialized. Though we can create a new variable, modifying existing variables is not allowed.**
5. What is Referential transparency?
**an expression, in a program, may be replaced by its value (or anything having the same value) without changing the result of the program. This implies that methods should always return the same value for a given argument, without having any other effect.**

## Modules and require()

1. What is a module?
**Its ajavascript file contain a certain function**
2. What does the word ‘require’ do?
**The require() method is used to load and cache JavaScript modules**
3. How do we bring another module into the file the we are working in?
**we need to import the module. we will use the require keyword at the top of the file.The result of require is then stored in a variable which is used to invoke the functions using the dot notation.**
4. What do we have to do to make a module available?
**we need to export the module to be available to other files.**

## Things I want to know more about

1. The modules and how to deal with them. 

## Resources used in this reading

1. <https://hackr.io/blog/functional-programming>
2. <https://www.sitepoint.com/what-is-referential-transparency/>
3. <https://www.youtube.com/watch?v=xHLd36QoS4k>