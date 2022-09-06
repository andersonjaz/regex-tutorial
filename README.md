# Regex Tutorial

# Let Me Show You How to Regex

This is a short summary of how to use Regex. 

## Summary

This is a short summary of how to use Regex. /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/ is the code snippet I will explain. 

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

There are two anchors. "^" denotes the start of a string and "$" denotes the end of a string.

### Quantifiers

Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found.

* *? Match zero or more times.
+ +? Match one or more times.
? ?? Match zero or one time.
{ n } { n }? Match exactly n times.
{ n ,} { n ,}? Match at least n times.
{ n , m } { n , m }? Match from n to m times.
Quantifiers in this regex includes the + operator, which will connect the users email name + email service + .com. Another quantifier for this regex includes {2,6}, which will allow a match range of 2-6 characters for the character set of [a-z.].

### OR Operator

There is no OR operator in this string.

### Character Classes

[a-f] - any alphabetic letters between a through f. Lower case a, b, c, d, e, and or f. [0-9] - any digit or numeric number between 0 and 9. 0, 1, 2, 3, 4, 5, 6, 7, 8, and or 9. In any arrangemenet.

### Flags

There are no flags.

### Grouping and Capturing

There are three groups in this piece of regex. The first capturing group is ([a-z0-9_\.-]+)which is capturing the user name of the email, which can have letters, numbers, an underscore or a dash.
the second capturing group is for the email site which is ([\da-z\.-]+). This one can have numbers or letters or a dash.
The third capturing group is ([a-z\.]{2,6}), which is the final part of the email which can be only letters and a period, like .cn or .net.

### Bracket Expressions

Brackets indicate a set of characters to match.
In the email, we want to check to see if the email is made of letters and numbers and underscores so we put these into brackets to check [a-z0-9] like so. If I wanted an email composed entirely of 1234 and "a" and "f", then I would put ^([af1234]+)@([0-9a-z]+)\.([a-z\.]{2,6})$

### Greedy and Lazy Match

Any thing that matches as many times as needed is greedy and anything that matches with as few as things as possible is lazy.


### Boundaries

The boundaries in this regex are the 's, the ones before the ^ and after the .

## Author

Laura J. Anderson