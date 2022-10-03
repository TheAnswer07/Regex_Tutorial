# Regex Email Tutorial

In this project, I'm creating a tutorial that explains how a specific regular expression, or regex, functions by breaking down each part of the expression and describing what it does.

## Summary

The following regex pattern is the one that we'll analyze. It matches an email with the format of name@domain.extension:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Character Escapes](#character-escapes)



## Regex Components


### Anchors

The beginning and the end of this expression are respectively denoted by the two (2) anchors "^" and "$".

### Quantifiers

The "+" and "{2,6}" represent the quantifiers in this expression denoting the quantities to match. There's no limit on the amount of characters before the "+". 

In this case, "([a-z0-9_\.-]+)" which is the name in "name@domain.extension", has unlimited amount of characters. The same goes for ([\da-z\.-]+) which is the "domain" section in the email format "name@domain.extension".

The "{2,6}" quantifier means that there can be a minimum of 2 and maximum of 6 characters in the extension section of the email format "([a-z\.]".

### Character Classes

This regex only has one Character Class which is the "\d" within the Grouping/Capturing construct ([\da-z\.-]+).

The "\d" refers to a Class of Character meaning any digits.

### Grouping and Capturing

The parenthesis "()" represent the Grouping/Capturing constructs in this regex, allowing the characters inside to be taken as a subset.

We have 3 Grouping/Capturing constructs in this regex and they're as follows:

([a-z0-9_\.-]+) for the "name",

([\da-z\.-]+) for the "domain", and

([a-z\.]{2,6}) for the "extension".

### Bracket Expressions

The bracket expressions [a-z0-9_\.-], [\da-z\.-] and [a-z\.] represent the match for one character for each of these sections.

Based on this regex's quantifiers, it allows for multiple matches of the characters in the bracket expressions.

### Character Escapes

The Character Escape in this regex is the "\." and it specifies that we're actually looking for a dot ".", instead of the normal/simple dot "." which would represent/mean matching any character.

## Author

This Regex Email Tutoril has been created by myself, Full Stack Developer Moussa D. You can access my GitHub page via the following link:

[GitHub Profile](https://github.com/TheAnswer07)
