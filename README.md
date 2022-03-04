# RegEx Tutorial Get The Gist

The objective of this tutorial is to explain a specific regex of *matching a simple email validation* and how it works. To understand the search pattern and what the regex defines. A good example that everyone can understand is an email. 

## Summary
To begin we must first understand what RegEx is.
Putting it plainly, it stands for *regular expression* it is a tool commonly used as a search pattern for matching one or more character's in string data. 
There are a series of symbols and characters that are used and we will dive into those throughout the tutorial. Below you will find the code I will be referring to.

Matching Email-

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`


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
In the Matching Email code the **Anchor** is the regular expressions beginning and end. In this string the '^' and '$'. 

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

Which indicates to the computer to search for something that looks like those two symbols, and **must** be included to find the match. 
If these symbols are missing there will not be a match.
Breaking down the string will help us better understand it.
We will call them *groups*.

`^([a-z0-9_\.-]+)`   at the __beginning__ is the '^'.

`.([a-z\.]{2,6})$`  at the __end__ of this group we see the '$'.

This is the first *group* it contains a-z,0-9 an underscore, hyphen or a period. These are the parameters to get a match. **NOTE** the period (also known as an *escape character* at the end) must have a backward slash "\" in or to be a match.

### Quantifiers

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

This has been a interesting process to understand RegEx.
I hope it was helpful.
Here is a link to my GitHub profile[RogueStorm](git@github.com:RogueStorm7/RegEx-tutorial-get-the-gist.git)
