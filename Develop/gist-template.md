# Email Address Validation - Regex

This document outlines regex search patterns on email addresses, validating and matching user inputs using the /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/


## Summary

Regex, short for Regular Expressions, is a sequence of characters that describes search patterns. It is used a tool to search and manipulate text, making it a very valuable tool in data process and analysis.


Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

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
There are 2 characters considered to be anchors, which are '^' and '$'.

The character '^' is used to indicated the begining of the string and to signify the end of the string, the '$' is used.



### Quantifiers

Quantifiers are set limits of a string that a regex matches. They include the minimum and maximum number of characters that a regex is looking for. In this case it's

Another quantifiers in this regex is '+' operator, which connects the users emailname + email service + .com.

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions
Characters in square brackets '[]' represent a range the we want to match. These are known as bracket expressions and positive character group as they outline the characters we want to include. 

A '-' is used between alphanumeric character (letters and numbers only) to represent a range of possible characters. 

'[a-z]' can contain any lower case letter between a-z and will only look for lowercase characters only. 

'[A-Z]' can contain uppercase letters between a-z and will only look for uppercase charachers. In order to look for both uppercase and lowercase, [a-zA-Z] will need to be used. 

'[0-9]' allows the string to contain any nuymber bewtween 0-9

'[_-]' The string can contain an underscore or hyphen. These are considersed special characters.

### Greedy and Lazy Match

Quantifiers are inherently greedy, meaning they match as many occurrences of particular patterns as possible. They include the following:

*—Matches the pattern zero or more times

+—Matches the pattern one or more times

?—Matches the pattern zero or one time

{}—Curly brackets can provide three different ways to set limits for a match:

{ n }—Matches the pattern exactly n number of times

{ n, }—Matches the pattern at least n number of times

{ n, x }—Matches the pattern from a minimum of n number of times to a maximum of x number of times

Each of these quantifiers can be made lazy by adding the ? symbol after it, meaning it will match as few occurrences as possible.

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
