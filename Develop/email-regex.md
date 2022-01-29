# Email Regex Tutorial

Regex, short for regular expression, is a string of text that allows you to create patterns that help match, locate, and manage text. The applications of regex include data validation, data scraping, data wrangling, data wrangling string parsing and more.

In this tutorial, I will be discussing the regex for an e-mail. I will be going in detail about the specific components/pattern needed for an email regex.

## Summary

```/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/```  is the string of text that makes up the regex of an email. 

The components that make up this regex that will be discussed is the following: anchors, quantifiers, character classes, flags, grouping and capturing, and bracket expression.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)

## Components of the Email Regex

Anchors: ```^ and $ ``` <br />
Quantifiers: ```* + ? and {} ``` <br />
Character classes: ``` \d \w \s and . ``` <br />
Grouping and Capturing: ``` () ``` <br />
Bracket Expressions: ``` [] ``` <br />

### Anchors
``` ^ ``` - Matches beginning of line || Example: ^abc || Matches: abc, abcd, abc123 <br />
``` $ ``` - Matches end of line || Example: abc$ || Matches: 123:abc, 234abc, hiabc <br />
``` ^ $ ``` - Exact string match || Example: ^abc$ || Matches: abc <br />

In the case of the email regex; the ```^``` indicates the beginning of the string while ```$``` indicates the end of the string

### Quantifiers
``` + ``` - Matches character before + one or more times || Example: a+c || Matches: ac, aac, aaac <br />

``` {} ``` - Matches a certain amount of times || Example: (abc){2} || Matches abcabc <br />

In the case of the email regex; the ``` + ```  matches the preceding characters in the bracket (will be covering brackets) that occur one or more times

In addition, the ``` ([a-z\.]{2,6}) ``` used in this expression matches any word characters between 2 and 6 times 

### Character Classes
``` \d ``` - Matches any numerical digit
``` \w ``` - Matches any word character 
``` . ``` - Matches any character

In the case of the email regex; the ``` \d ``` and ``` . ``` are used to match any digit character and any characters, respectfully.

### Flags
A regex usually comes within the form ```/abc/``` where the search pattern is between two slash characters. We can specify a flag at the end with these values:

``` g ``` (global) - looks for all matches, without it - only the first match is returned
``` m ``` (multi-line) - when enabled ^ and $ will match the start and end of a line, instead of the whole string
``` i ``` (insensitive) - makes the whole expression case-insensitive (example: /aBc/i would match AbC)

### Grouping and Capturing
```()``` - Capture anything matched || Example: (a)b(c)	|| 	Captures 'a' and 'c'

In the case of the email regex; the ``` ([a-z0-9_\.-]+) ``` used in this expression captures any word characters, numbers, "_", and "-". With the quantifier "+", it matches 1 or more of the preceding characters

### Bracket Expressions
``` [] ``` - Matches anything contained in the brackets || Example: [abc] || Matches: a, b, or c

In the case of the email regex; the ``` [a-z0-9_\.-] ```  used in this expression matches any characters in between the brackets. Therefore, all word characters, numbers, "_" and "-" will have a match

## Author

More from Michael Li:

I am aspiring software developer that loves to learn new skills and will hopefully make big changes in society, especially through coding.

My github can be found here: https://github.com/limichael97
