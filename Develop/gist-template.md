Regular Expression Tutorial

This tutorial will be a foundational reference guide for anyone learning regular expressions.
 I'll be referencing one partiucular regex throughout this tutorial which can be used to search 
 for an email address that follows this structure "email@gmail.com" and return a match if the 
 email matches the criteria specified in the regex. We'll break down each component of our email 
 regex and learning about the functionality of each part. By the end of this tutorial you will 
 know what a regular expression is, when to use them and how to utilize each component.

## Summary
A regular expression or "regex" is a statement that describes a specific pattern of characters 
that can be searched for in a file or directory, matched and then returned to be utilized by a 
user or program to serve various use cases. The goal of each regex is to return a match 
for a continuous series of characters. The type of characters, number characters and order of 
characters can all be specified and modified inside the regex statement.

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
The caret (^) anchor: Matches the beginning of the string. For example, if you want to match any string that starts with "Hello", you can use the regex pattern "^Hello".

The dollar sign ($) anchor: Matches the end of the string. For example, if you want to match any string that ends with "world", you can use the regex pattern "world$".
### Quantifiers
The asterisk (*) quantifier: Matches zero or more occurrences of the preceding pattern. For example, the regex pattern /abc/ matches "ac", "abc", "abbc", "abbbc", and so on.

The plus sign (+) quantifier: Matches one or more occurrences of the preceding pattern. For example, the regex pattern /ab+c/ matches "abc", "abbc", "abbbc", and so on, but not "ac".

The question mark (?) quantifier: Matches zero or one occurrence of the preceding pattern. For example, the regex pattern /ab?c/ matches "ac" and "abc", but not "abbc".

The curly braces ({}) quantifier: Matches a specific number of occurrences of the preceding pattern. For example, the regex pattern /a{3}/ matches "aaa", but not "aa" or "aaaa".
### OR Operator
The OR operator in regex allows you to match a pattern if it matches any one of several alternatives. The OR operator is denoted by the vertical bar (|) character.

For example, if you want to match a string that contains either "cat" or "dog", you can use the regex pattern /cat|dog/. This pattern matches "cat", "dog", and any string that contains either "cat" or "dog", such as "the cat and the dog".
### Character Classes
character classes and their meanings:

[0-9]: Matches any digit
[a-z]: Matches any lowercase letter
[A-Z]: Matches any uppercase letter
[a-zA-Z]: Matches any letter, uppercase or lowercase
[ \t\n\r\f\v]: Matches any whitespace character (space, tab, newline, carriage return, form feed, or vertical tab)
### Flags
The Flags and their meanings.

g (global): Matches all occurrences of the pattern in the string, not just the first one. Without this flag, the regex will stop after the first match.
i (case-insensitive): Matches the pattern regardless of case. For example, the pattern /hello/i will match "hello", "Hello", "HELLO", and so on.
m (multiline): Matches the pattern across multiple lines, rather than just within a single line. This flag affects the behavior of the caret (^) and dollar sign ($) anchors.
s (dotall): Matches any character, including newline characters (\n), with the dot (.) character. Without this flag, the dot only matches non-newline characters.
u (unicode): Enables full Unicode support for the pattern, including matching Unicode characters and using Unicode property escapes.
y (sticky): Matches the pattern only at the index specified by the lastIndex property of the regex object. This flag is used in conjunction with the lastIndex property for more advanced string matching.

### Grouping and Capturing
When grouping a section of regex, you break the regex into different parts, each of with has their own paramemters. Regex are grouped with ().
### Bracket Expressions
[abc] Matches the characters with in the brackets. [^abc]Excludes the characters in the brackets.

### Greedy and Lazy Match
Along side with quantifiers, quantifiers can be greedy or lazy. Greedy means they must macth as many times as possible. Lazy means it matches the least times possible.

*— Matches the pattern zero or more times

+— Matches the pattern one or more times

?— Matches the pattern zero or one time
### Boundaries
Boundries anchor the regex to a begining and end of a string. Using Anchors explained above, we can se tthe boundries for a regex.
### Back-references
A backreference in regex is a way to refer to a previously captured group within the same regex pattern. This allows you to match a string that contains a repeated sequence of characters.

Backreferences are indicated using the backslash () character followed by a number that corresponds to the numbered capture group you want to reference. The number is the same as the order in which the capture group appears in the pattern, starting with 1.

## Author

Kaylon Myers is an aspiring software engineer in Houston, TX. GitHub: https://github.com/kaylonm17