# Java_Basics
## Table of contents 
- [Chapter 1: Basic concepts](https://github.com/Cecilia-xu/CS_Notes/blob/master/Java/Java_basics.md#chapter-1-basic-concepts)
- [Chapter 2: OOP](https://github.com/Cecilia-xu/CS_Notes/blob/master/Java/Java_basics.md#chapter-2-object-oriented-programming-oop)
- [Chapter 3: Testing](https://github.com/Cecilia-xu/CS_Notes/blob/master/Java/Java_basics.md#chapter-3-testing)
- Chapter 4: Exception handling
- Chapter 5: Generics
- Chapter 6: Garbage collection
- Chapter 7: Concurrency
- Chapter 8: Parallelism
## Chapter 1: Basic concepts
1. Complier: a computer program to transform source code written in a programming language (the source language) into another computer language (the target language).
e.g. Java - high level programming language -> machine code
2. SDK (Software Development Kit) -> JDK
3. JRE/JVM (Java Runtime Environment aka Java Virtual Machine): allows program to run on multiple operating systems
4. IDE(Integrated Development Environment)
5. variables: a space in memory(RAM)
- RAM: Computer memory or random access memory (RAM) is your system’s short-term data storage; it stores the information your computer is actively using so that it can be accessed quickly. The more programs your system is running, the more memory you’ll need. 
6. Declaration
7. Initialization
8. Overflow: Storing a value that is too large for a declared type of variable will cause an overflow error
9. Primitive data type<br>
<img src = "https://s2.ax1x.com/2019/09/29/u3P6pQ.png" width = 80%></img>
- Note: String is not a primitive data type, but a reference type/class(which has methods)
<img src = "https://s2.ax1x.com/2019/09/29/u3Ph7V.png" width = 80%></img>
10. Naming conventions
- Variable names 
  - begin with a lettr 
  - single-word variable: lowercase letters
  - multi-word variabl: CamelCase notation
- Constant
  - keyword final
  - names: all letters are capitalized
  - multi-word name: words are separated with an underscore
- Method (Same as for variables)
11. Typecasting: to explicitly convert one data type to another e.g.(int)/(double)
12. Char
- MUST in Single quotation marks
- encoding
  - Unicode (Java): 16 bits
  - ASCII(subset of Unicode): 128 / +128 (Extended ASCII)/ 95 (printable ASCII)
  - Note: solving leetcode questions —— ask what is the character set they want? just letter: 26 * 2 = 52/ letter + number = 62/ All ASCII/+ Extended ASCII
  - Escape Sequence
13. Conditions(if/ switch)
- Compare
  - Numbers/chars: relational operators (< <= > >= == !=)
  - String: equals/compareTo(compares strings in lexicographic order)
  - Objects: ==(whether two object **references** are identical)/ equals(whether two object **contents** are identical) <br>
  Note: works correctly only if the implementors of the class have supplied it
  - Null: == null (Note: null - no reference v.s. "" - empty string)
- Combine conditions(Boolean operators)
  - && and || : short-circuit evaluation (As soon as the truth value is determined, no further conditions are evaluated.)
  - !
- Multiple alternatives (if ... else if ... else ...)v.s. Multiple conditions(if...if...if...)
- Switch statement<br>
<img src="https://s2.ax1x.com/2019/09/30/uG7PNn.png" width = 50%></img>
14. Loops (for loop/while loop)
- break statement: exit a while, for, or do loop/ switch
- continue statement(few programmer use): jumps to the end of the current iteration of the loop
15. semantics(language specs defines semantics) v.s. implementations(defines actual behavior of a progtames)<br>
Example:
- Senmantically:
```
int i = 0;
i ++;
````
- Implementation:
```
Set i to be 0
Read i, i = 0
Perform 0 + 1 = 1
Write new value 1 back to i 's memory location
```
##  Chapter 2: Object Oriented Programming (OOP)
1. Objects have
- fields (What things it maintains)
- methods (What it can do)
2. Instantiation: keyword "new" --> an object/an instance
3. Method
<img src="https://s2.ax1x.com/2019/09/29/u3PqXR.png" width = 50%></img>
- types
  - accessor methods: returns some information without changing the object
  - mutator methods: modify the internal data of an object
- return statement
- calling method
4. Constructor<br>
<img src="https://s2.ax1x.com/2019/09/29/u8pk4g.png" width = 90%></img>
5. UML diagram<br>
<img src="https://s2.ax1x.com/2019/09/29/u8pwVK.png" width = 40%></img>
6. The advantage of object oriented software development are:
- Modular development of code -> easy maintenance + modification
- Reusability
- reliability and flexibility
- increase understanding of code
7. 4 features:
### feature 1: encapsulation
- Refers to data hiding. In Java, there are three access modifiers: public, private and protected.
- Getter and setter methods used to access private fields
### feature 2: polymorphism
### feature 3: inheritance
### feature 4: abstraction
6. Constructors: the attributes are not initialized in the class, instead, they are unutualizaed in the constructors
- can verify and correct the values for the attributes and avoid weird or meaningless states!
- Overload: have more than 1 constructors, each of which has different parameters
  - differentiated by the number, the type, and the order of the arguments passed. 
7. reference: this（key word)/ dereferencing
8. Objects in real life: a list, a queue, an array, a program, a linked list node, etc.

## Chapter 3: Testing
1. Implement a testing program
- Provide a tester class.
- Supply a main method.
- Inside the main method, construct one or more objects. 4. Apply methods to the objects.
- Display the results of the method calls.
- Display the values that you expect to get.
- Black box testing: a testing method that does not take the structure of the implementation into account. If a program works perfectly on all inputs, then it surely does its job.
- White box testing: uses information about the structure of a program. Performing unit tests of each method is a part of white box testing.
- Code coverage: a measure of how many parts of a program have been tested. That means that you need to look at every if/else branch to see that each of them is reached by some test case.
- Boundary test cases are test cases that are at the boundary of acceptable inputs.
- It is a good idea to design test cases before implementing a program.
- Logging messages can be deactivated when testing is complete.



