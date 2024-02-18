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

   - `essential`: Verify the student used a switch statement.
     Would be nice if we could give different feedback depending on what the student used instead.
     If it was if-else, comment that switch is better suited for so many different variants.
     If an object was used, comment that this is nice but the goal is to practice switch.
   - `essential`: Verify that there are 5 cases and a default case in the switch statement to make sure the student did not tailor their code for the test cases (e.g., used more cases instead of default).
   - `actionable`: If the student used `break`, comment to use early `return`s instead to avoid assigning to a helper variable first and then returning that variable.
   - `celebratory`: Comment something nice when a student used grouped case statements.
     ```javascript
     case 'Energizer':
     case 'Green Garden':
        return 1.5;
     ```

2. Task 2: Describe a destination

   - A solution that uses `if (limes.length < 0) break;` instead of combining the conditions should be considered equally correct to the exemplar solution.
     The version in the exemplar file is shorter but the break version emphasizes that there is a special edge case.
   - `essential`: Verify that `while` was used.
   - `essential`: If a helper function was used for the switch statement, check that is was not exported.
   - `actionable`: If the student wrote `if (limes.length < 0) return limesCut`, comment that the duplication of `return limesCut` can be avoided by using break there instead of return.
   - `actionable`: Tell the student to use a helper function to wrap the switch statement for readability if he/she did not do that.
   - `informative`: If the student used a counter to iterate over the array, show a comment about about `shift`.
   - `informative`: Remind the student about `++` if it was not used to increment the lime counter.
   - `informative`: Check whether a shorthand assignment `+=` was used to increase the loop counter.
   - `informative`: If `default` was included in the switch statement, remind the student that it is optional and not needed in the scope of the task.
   - `celebratory`: Make a positive remark if the student used a helper function to wrap the switch statement.
   - `celebratory`: Celebrate if the student used `++` and `+=`.

3. Task 3: Describe the travel method

   - `essential`: Verify that do-while was used.
     If while was used instead, say that do-while is a better fit because there is always at least one iteration (because `timeLeft` is always > 0) and the condition can best be checked after running the code.
   - `essential`: Verify `timeToMixJuice` was reused instead of duplicating the code.
   - Most of the points from task 2 also apply here.
     Check what can be reused.

4. Task 4: Describe a character traveling to a destination

   - `essential`: Verify that do-while was used.
     If while was used instead, say that do-while is a better fit because there is always at least one iteration (because `timeLeft` is always > 0) and the condition can best be checked after running the code.
   - `essential`: Verify `timeToMixJuice` was reused instead of duplicating the code.
   - Most of the points from task 2 also apply here.
     Check what can be reused.

5. Task 5: Describe a character traveling to a destination without specifying the travel method.

   - `essential`: Verify that do-while was used.
     If while was used instead, say that do-while is a better fit because there is always at least one iteration (because `timeLeft` is always > 0) and the condition can best be checked after running the code.
   - `essential`: Verify `timeToMixJuice` was reused instead of duplicating the code.
   - Most of the points from task 2 also apply here.
     Check what can be reused.

[representer-java]: https://github.com/exercism/java-representer
[analyzer-java]: https://github.com/exercism/java-analyzer
