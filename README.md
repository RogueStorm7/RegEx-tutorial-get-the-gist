# RegEx Tutorial Get The Gist

The objective of this tutorial is to explain a specific regex of *matching a simple email validation* and how it works. To understand the search pattern and what the regex defines. A good example that everyone can understand is an email. 

## Summary
To begin we must first understand what RegEx is.
Putting it plainly, it stands for *regular expression* it is a tool commonly used as a search pattern for matching one or more character's in string data. 
There are a series of symbols and characters that are used and we will dive into those throughout the tutorial. Below you will find the code I will be referring to.
 
String of a matching email. The average person never sees an email written like this.

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

Usually, it is written as the example below:
- "mynameis@gmail.com" or "contactme@yahoo.com"


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
We will call them *groups*. We are only looking at the *beginning* and *end* right now. 

In this *group* it contains: a-z, 0-9 an underscore, hyphen or a period.
`^([a-z0-9_\.-]+)`   at the __beginning__ is the `^` .

In this *group* it contains:
`.([a-z\.]{2,6})$`  at the __end__ of this group we see the `$`.

These are the parameters to get a match. **NOTE** the period (also known as an *escape character* at the end) must have a backward slash to be a match.

We will get to the **middle** _group_ shortly.
### Quantifiers
In order for there to be a match. 
The *Qualifiers* indicate how many times a specific character or group thereof is present. An example would be `abc+`.
In the string there will be a match as long as there is `ab` but has to have a **minimum** of one `c` to get that match. If not there is no match. **NOTE** the `+` means one of these characters **must** be included to match.
### OR Operator
The `#` has to be present and identifies a matching hex code.
**NOTE** this is not the string for an email match. We will get back to that for now... 

Take a look at this code: `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

 Breaking this down: `/^#?([a-f0-9]{6}`. We see the `#` comes first. The `a-f`, `0-9`,`{6}` means a match will include a `6` character string; containing `a-f` alphabets and `0-9` numerics. **NOTE** I left the brackets out of the example to help you see the details I was explaining they must be included in order to match. 
 
 In this string of code it is saying find the above named example 6 characters that include: the `#`, `a-f`, and `0-9`. **OR**

 The `|` is a symbol that signifies **OR** (a boolean value) match this `[a-f0-9]{3})$/`. A string of 3 characters that include:`a-f`, and `0-9`.
 ### Character Classes
Back to the original 
### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author
My name is, Mianta McKnight, and I created this tutorial. 
It has been a interesting process to understand RegEx.
I hope it was helpful.
Here is a link to my GitHub profile @ [RogueStorm](git@github.com:RogueStorm7/RegEx-tutorial-get-the-gist.git)


