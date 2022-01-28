# Email Regex Tutorial

Regex, short for regular expression, is a string of text that allows you to create patterns that help match, locate, and manage text. The applications of regex include data validation, data scraping, data wrangling, data wrangling string parsing and more.

In this tutorial, I will be discussing the regex for an e-mail. I will be going in detail about the specific components/pattern needed for an email regex.

## Summary

```/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/```  is the string of text that makes up the regix of an email. 

The components that make up this regex that will be discussed is the following: anchors, quantifiers, OR operators, character classes, flags, grouping and capturing, bracket expression, greedy and lazy match, boundaries, back-references, look-ahead and look-behind.

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

## Components of the Email Regex

Anchors: ```^ and $ ``` <br />
Quantifiers: ```* + ? and {} ``` <br />
OR operator: ``` | or [] ``` <br />
Character classes: ``` \d \w \s and . ``` <br />
Grouping and Capturing: ``` () ``` <br />
Bracket Expressions: ``` [] ``` <br />

### Anchors
``` ^ ``` - Matches beginning of line || Example: ^abc || Matches: abc, abcd, abc123 <br />
``` $ ``` - Matches end of line || Example: abc$ || Matches: 123:abc, 234abc, hiabc <br />
``` ^ $ ``` - Exact string match || Example: ^abc$ || Matches: ^abc$ <br />

In the case of the email regex; the ```^ ``` indicates the beginning of the string while ```$``` indicates the end of the string

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

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
