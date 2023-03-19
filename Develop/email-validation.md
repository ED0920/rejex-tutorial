# Email Address Validation - Regex

This tutorial outlines regex search patterns on email addresses, validating and matching user inputs using the expression `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`. This is a useful tool when validating emails in applications.


## Summary

Regex, short for Regular Expressions, is a sequence of characters that describes search patterns. It is used a tool to search and manipulate text, making it a very valuable tool in data process and analysis. We will be analysing email expression `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)


## Regex Components

### Anchors
There are 2 characters  `^` and `$` considered to be anchors.

In our regex `^` is used to indicated the begining of the string and `$` is used to signify the end of the string, th

### Quantifiers

Quantifiers are set limits of a string that a regex matches. They include the minimum and maximum number of characters that a regex is looking for. In this case it is `{2,6}` in our expression allowing a match range between 2-6 charachers for the character set of `[a-z]`.

Another quantifiers in this regex is `+` operator, which connects the users email name + email service + .com.

### Character Classes

To define a set of characters in regex we use character classes.

The character class in our expression is `\d`. This will match any Arabic numeral digit which is equivalent to `[0-9]`.

### Grouping and Capturing

In order to group sections of a regex, we use parentheses `()`. Each section within `()` is known as a subexpression. In our expression, the subexpression are as followed:
- `([a-z0-9_\.-]+)` matches the user email address
- `([\da-z\.-]+)` matches the email service
- `([a-z\.]{2,6})` captures the '.com'

### Bracket Expressions
Characters in square brackets `[]` represent a range the we want to match. These are known as bracket expressions and positive character group as they outline the characters we want to include. Our expression contains the following bracket expressions:

`-` is used between alphanumeric character (letters and numbers only) to represent a range of possible characters. 

`[a-z]` allows for any lower case letter between a-z and will only look for lowercase characters only. 

`[0-9]` allows the string to contain any nuymber bewtween 0-9

`[_-]` allows the string  to contain an underscore or hyphen. These are considersed special characters.

### Greedy and Lazy Match

Quantifiers are inherently greedy, meaning they match as many occurrences of particular patterns as possible. 

In our regex expression a  `+` qunatifier will mached as many times as possible. Another quantifier used in our regex is 
`{}` when matcheing `{2,6}` in our last sub expression. 

Each of quantifier can be made lazy by adding the `?` symbol after it, meaning it will match as few occurrences as possible.


## Author

Please see my projects at https://github.com/ED0920 

