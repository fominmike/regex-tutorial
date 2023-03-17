 # Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/

The regex expression that I'll be summarizing today is an expression used to examine and verify a given email address. To shortly go over, this expression looks for a word or numbers, followed by a '@', then another word, followed by a period, ending with one more word 2-6 characters in length.


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
^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/

The two anchors we'll be examining is the ^ anchor and the $ anchor. These two anchors typically look for the start and end of a string. ^ - this anchor loks for the start of the string to match the given criteria, $ - so as this anchor makes sure the end of the string matches the criteria.


### Quantifiers
^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/

Quantifiers are characters within the expression that indicate number of characters or expressions to match. In our exapmle, we identify two quantifiers which is the + and the {} brackets. The + in our example means that there should be one or more of the given criteria characters used before the @ sign. Also, we see {2, 6}, which means that the length of this group should be no less than 2 and no more than 6

### Character Classes
By using character classes, we tell the regex engine to use to match only one out of several characters. For example, if we want to check for the word grey or gray to both match, we can use the expression gr[ea]y.

### Grouping and Capturing
Grouping and capturing is done by placing a certain part of an expression into parantheses or round brackets. In the example we're breaking down, grouping is used 3 times. ([a-z0-9_.-]+) this examines a certain group that can contain lowercase letters, numbers, and alos underscore, hyphen or period.

### Bracket Expressions
Bracket Expressions use [] to examine the the user input to match the certain characters inside the brackets. For example [hHiI] will match with hi, hI, Hi, HI. [a-z] Here we look at this bracket expression that matches any letter to be lowercased.

### Greedy and Lazy Match
When looking at our givin example, we use a greedy regex expression. We use the + quantifier. It allows the engine to match one or more of the token it quantifies.

## Author
Michael Fomin is the author of this tutorial. Github https://github.com/fominmike/regex-tutorial
