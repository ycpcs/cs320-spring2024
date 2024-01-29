---
layout: default
title: Course Overview, OOP
---

Introduction
============

What is the course about?

-   The *practice* of software development
-   All the things you need to know to

    -   Figure out what a system should do (requirements)
    -   Define and analyze the problem (analysis)
    -   Design a system to solve the problem (design)
    -   Implement the design (implementation)
    -   Ensure the quality of the implementation (testing, code review)
    -   Work in a collaborative team environment
	-	Share code (version control - shared code base and issue tracking)
    -   Planning and estimation (how long will it take?)

The course will focus on *object-oriented* software development

-   The techniques can be adapted for non object-oriented languages

Course will emphasize *agile* software development

-   Agile software development is an *incremental* development process
-   Develop the system a little bit at a time
-   The idea is to make steady progress
-   The system is stable and functional at all times
-   Don't wait until the end of the project to "see if it works"

[Here's how we're going to do that.](./lecture00.html)


Object-Oriented Programming (OOP)
---------------------------------

The course will focus on object-oriented software construction using an object-oriented language.

"Object-oriented" means that the software is a collection of objects that interact with each other.

In esence, identify the physical real-world objects that make up the project problem statement, and then translate those objects into prgrammatic classes that interact with each other, much as they would do in the real world.

An *object* is an instance of a class.

A class is a user-defined data type: like a struct in C.

A class defines

> **fields** (member variables): a collection of variables that each object that is an instance of the class will possess

> **methods** (member functions): define the behavior of the objects that are instances of the class

The key to developing good object-oriented software is figuring out what objects/classes you need, and what the *behavior* of those objects/classes should be!

> In other words, the important thing is WHAT objects do, not HOW they do it

This is the distinction between *design* and *implementation*:

> Design is figuring out WHAT the objects should do &mdash; their behavior

> Implementation is taking the desired behavior and figuring out HOW the behavior should be accomplished

This course focuses on both the design (the WHAT), and the implementation (the HOW). You will be learning WHAT the WHAT is while also learning HOW to do the HOW!