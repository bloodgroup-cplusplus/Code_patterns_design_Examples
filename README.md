# Code_patterns_design_Examples
This repository includes few of the C++ Programming:Code patterns design
the original file is taken from https://en.wikibooks.org/wiki/C%2B%2B_Programming/Code/Design_Patterns

THE CODES ARE PRESENT IN THE REPOSITORY AS RESPECTIVE CPP FILES


Software design patterns are abstractions that help structure system designs. While not new, since the concept was already described by Christopher Alexander in its architectural theories, it only gathered some traction in programming due to the publication of Design Patterns: Elements of Reusable Object-Oriented Software book in October 1994 by Erich Gamma, Richard Helm, Ralph Johnson and John Vlissides, known as the Gang of Four (GoF), that identifies and describes 23 classic software design patterns.

A design pattern is neither a static solution, nor is it an algorithm. A pattern is a way to describe and address by name a repeatable solution or approach to a common design problem, that is, a common way to solve a generic problem (how generic or specific the pattern is depends on how restricted the target goal is). Patterns can emerge on their own or by design. This is why design patterns are useful as an abstraction over the implementation and a help at design stage. With this concept, an easier way to facilitate communication over a design choice as normalization technique is given so that every person can share the design concept.

Depending on the design problem they address, design patterns can be classified in different categories, of which the main categories are:

Creational Patterns
Structural Patterns
Behavioral Patterns.
Patterns are commonly found in objected-oriented programming languages like C++ or Java. They can be seen as a template for how to solve a problem that occurs in many different situations or applications. It is not code reuse, as it usually does not specify code, but code can be easily created from a design pattern. Object-oriented design patterns typically show relationships and interactions between classes or objects without specifying the final application classes or objects that are involved.

Each design pattern consists of the following parts:

Problem/requirement
To use a design pattern, we need to go through a mini analysis design that may be coded to test out the solution. This section states the requirements of the problem we want to solve. This is usually a common problem that will occur in more than one application.
Forces
This section states the technological boundaries, that helps and guides the creation of the solution.
Solution
This section describes how to write the code to solve the above problem. This is the design part of the design pattern. It may contain class diagrams, sequence diagrams, and or whatever is needed to describe how to code the solution.
Design patterns can be considered as a standardization of commonly agreed best practices to solve specific design problems. One should understand them as a way to implement good design patterns within applications. Doing so will reduce the use of inefficient and obscure solutions. Using design patterns speeds up your design and helps to communicate it to other programmers.

Creational Patterns
In software engineering, creational design patterns are design patterns that deal with object creation mechanisms, trying to create objects in a manner suitable to the situation. The basic form of object creation could result in design problems or added complexity to the design. Creational design patterns solve this problem by somehow controlling this object creation.

In this section we assume that the reader has enough familiarity with functions, global variables, stack vs. heap, classes, pointers, and static member functions as introduced before.

As we will see there are several creational design patterns, and all will deal with a specific implementation task, that will create a higher level of abstraction to the code base, we will now cover each one.

Builder
The Builder Creational Pattern is used to separate the construction of a complex object from its representation so that the same construction process can create different objects representations.

Problem
We want to construct a complex object, however we do not want to have a complex constructor member or one that would need many arguments.
Solution
Define an intermediate object whose member functions define the desired object part by part before the object is available to the client. Builder Pattern lets us defer the construction of the object until all the options for creation have been specified.


See creational_pattern_example (creational_pattern.cpp)
