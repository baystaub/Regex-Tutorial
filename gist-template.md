# Regex Tutorial (Regular Expression's)

This tutorial is to choose a regular expression (Regex) and breakdown the structure of it. each regular expression is composed of meta-characters and literal characters. Regex is used to search for patters occurring in a set of code and sort through the data. These can be very helpful is using to perform tons of different functions and make our lives easier.

## Summary

In this tutorial i will be summarizing how to match hex values: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

For the examples, I will be using the components of the matching hex values expression.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors
There are two Anchors that Regex uses. One being the caret "^", and the other being the dollar sign "$". The caret is used to identify the start of an expression while the dollar sign is used to identify the end.

ex: /^ start, $/ end

### Quantifiers
Quantifiers are classified as either greedy, or lazy. They are used to specify the amount of times a character, group, or character class must be present in the input to find a match.

ex: ? match zero, {6} match exactly 6 times,{3} match exactly 3 times

### Grouping Constructs
Grouping constructs delineate subexpressions of regular expression and capture the substrings of an input string. They are used to match subexpressions that are repeated in an input string, apply quantifiers to a subexpression that has multiple regex elements, Include subexpressions in strings, and retrieve single subexpressions from the Match.Groups prorerty and preocess the seperately fro the matched text as a whole.

ex: ([a-f0-9]{6}|[a-f0-9]{3}), what is in the parenthesis is the group that seperates the subexpression from the regular expression.

### Bracket Expressions
Bracket expression is a matching list expression or non-matching list expression. It consisits of one or more of the following expressions: ordinary characters, collating elements, collating symbols, equivalence classes, character classes, or range expressions.

ex: [a-f0-9] will match a range of characters a through f and zero through nine as specified within the brackets.

### Character Classes
Character classes distinguish kinds of characters for example, letters and digits.

ex: a-f0-9, there are the defined characters to match in the regex expression

### The OR Operator
OR operators are used to provide as many terms desired as long as they have "|" seperating each term. the "|" seperates each term contained within a group "(...)".

ex: | , this is used in the regex expression to say match [a-f0-9]{6} OR [a-f0-9]{3}. 

### Flags
Regex has flags that allow for functionality like global and case insensitive searching. Flags can be used together or seperately in any order.

### Character Escapes
character escapes are done by using a backslash in front of special characters. For example, to search for "a" followed by "*" followed by "b", you'd use 
'/a\*b/' 

## Author

Hello, My name is Bailey. I am a learning developer and this is my tutorial of regualr expressions.
https://github.com/baystaub?tab=repositories