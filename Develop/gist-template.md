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

Regex for an emailaddress

/^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/ *Structure of an email address: The structure of a basic email address is split up into 3 main parts: the "user-name" and "domain-name" separated by an @ "At sign", then a . "dot" followed by the "domain-extension". The final address structure will look like this: (user-name)@(domain-name).(domain-extension) We'll reference these 3 parts throughout this tutorial.