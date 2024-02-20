# Design

## Goal

The goal of this exercise is to teach the student the basics of the Concept of `Method Overloading` in Java.

## Learning objectives

- Know what method overloading is.
- Know how to overload a method with different number of parameters
- Know how to overload a method with different argument types

## Concepts

- `method-overloading`

## Prerequisites

This exercise's prerequisites Concepts are:

- `classes`
- `strings`
- `enums`

## Representer

This exercise does not require any specific representation logic to be added to the [representer][representer-java].

## Analyzer

This exercise could benefit from the following rules in the [analyzer][analyzer-java].
The comment types mentioned below only serve as a proposal.

1. Task 1: Describe a character

   - `informative`: If the student used String Concatenation, inform them about String Formatting but do not suggest that it is a better option.

2. Task 2: Describe a destination

   - `informative`: If the student used String Concatenation, inform them about String Formatting but do not suggest that it is a better option.

3. Task 3: Describe the travel method

   - `informative`: If the student used if-else, inform them about Ternary Operators but do not suggest that it is a better option.
   - `informative`: If the student used String Concatenation, inform them about String Formatting but do not suggest that it is a better option.

4. Task 4: Describe a character traveling to a destination

   - `essential`: Verify that `describe` methods for Tasks 1, 2 and 3 were reused instead of duplicating the code.
   - Points from Task 3 also apply here. Check what can be reused.

5. Task 5: Describe a character traveling to a destination without specifying the travel method.

   - `essential`: Verify that `describe` method for Task 4 was reused instead of duplicating the code.
   - Points from Task 3 also apply here. Check what can be reused.

[representer-java]: https://github.com/exercism/java-representer
[analyzer-java]: https://github.com/exercism/java-analyzer
