# Regex tutorial

This is a walthrough example of how Regex works. Regex is short for Regular Expression, it's used for many things, like making a function that validates a criteria the coder is wishing to create. For this tutorial, Regex will be used to match emails. 
## Summary
The code presented below will be used as an example of how Regex is used. This code is used for formatting emails. It means that it must follow these Regex criterias or the email will be invalid

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
^, $:Anchors starts and ends regular expressions.
-Everything in parathneses are defined and the user must match the guidelines of the anchors. 
### Quantifiers
-Quantifiers are a group that user can use to  further specify a criteria . In our case it will be :

([a-z0-9_\.-]+)

-this means that the string that sent contain the letters a-z, numbers through 0-9, and symbols _, .,  or -. The + is an order command, it has to follow these orders or it may cause an error

### OR Operator
-This is particular expression does not contain a OR operator, but we will look at the code that makes it so, and how it operates in the functions.


### Character Classes
An example of Character Classes in this code is /d.

-it ensures that the expessions after the @ symbol, that a letter is picked and not a number.

### Flags

### Grouping and Capturing
The grouping  and capturing of an expression are done by parasenthesis.
In this code there is:
([a-z0-9_\.-]+) - as you can see it is surrounded by parasenthesis and it is also done in order. The user response must be true before it moves to the next group ([\da-z\.-]+), and this expression must be match before it validates to the other group in our expression ([a-z\.]{2,6}) 


### Bracket Expressions
As name suggests, to use this is the coder has to use brackets. These are templates for matching the expressions.

For example :
[a-z0-9_\.-]
As explained earlier, this code means the response must have letters a-z, numbers 0-9, ., ., or _, and it is set in a bracket because it must be true for validation to go through.
### Greedy and Lazy Match
-The example code does  not have greedy or lazy match.
### Boundaries
The example code does not contain Boundaries.
-Boundaries are used to look for specific words in a string.
### Back-references
The example code does not contain Back-references.
### Look-ahead and Look-behind
The example code does not contain any Look-ahead or Look-behind expressions

## Author
Tutorial created by Edmer Valencia.
