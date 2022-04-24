# Regex tutorial 

This is a walkthrough example of how Regex works. Regex is short for Regular Expression, it's used for many things, like making a function that validates a criteria the coder is wishing to create. For this tutorial, Regex will be used to match emails. 
## Summary
The code presented below will be used as an example of how Regex is used. This code is used for formatting emails. It means that it must follow these Regex criterias or the email will be invalid

```text
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)

## Regex Components

### Anchors
```text
^ , $
```
  Anchors starts and ends regular expressions.
 - Everything between the ^ and $ symbols are defined and the user must match the guidelines of the anchors. 
### Quantifiers
- Quantifiers are a group of expressions that user can use to  further specify a criteria . In our case it will be :

```text
([a-z0-9_\.-]+)
```
- This means that the string that sent contain the letters a-z, numbers through 0-9, and symbols _, .,  or -. The + is an order command, it has to follow these orders or it may cause an error.

### OR Operator
- This is particular expression does not contain a OR operator, but we will look at the code that makes it so, and how it operates in the functions.
```text
x(y|z)
```
 - the | in the expressions means OR in simple terms. This means the string MUST have an x that is followed by y or z.

### Character Classes
- An example of Character Classes in this code is /d, in the ([\da-z\.-]+).

- it ensures that the expessions after the @ symbol, that a letter is picked and not a number.

### Flags
- Flags are used to give more guidelines to validate the code.

- Flags are not used in this code, but formally users can find them between the slashes where a flag indicator will be found. 

- For example:
 g means "global" and makes the regex in to match everything within the string.

 m means "multiline" and it means every line will be matched seperately, every expression will be read one by one between the anchors.

 i means "insensitive" it means that the expression will not be picky betweeen capitals and lowercase so it will pass the matching.

### Grouping and Capturing
- The grouping  and capturing of an expression are done by parasenthesis.
- In this code there is:
```text
([a-z0-9_\.-]+)
```
 - as you can see it is surrounded by parasenthesis and it is also done in order. The user response must be true before it moves to the next group ([\da-z\.-]+), and this expression must be match before it validates to the other group in our expression ([a-z\.]{2,6}) 


### Bracket Expressions
- As name suggests, to use this is the coder has to use brackets. These are templates for matching the expressions.

For example :
```text
[a-z0-9_\.-]
```
- As explained earlier, this code means the response must have letters a-z, numbers 0-9, ., ., or _, and it is set in a bracket because it must be true for validation to go through.

## Author
Tutorial created by Edmer Valencia.
- Email: edmer_franciz@yahoo.com
- Github:  https://github.com/edm1001
- Gist Link: 
