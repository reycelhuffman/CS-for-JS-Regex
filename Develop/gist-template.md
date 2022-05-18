# Computer Science for Javascript: Regex Tutorial 

Introductory paragraph (replace this with your text)
In this Regex Tutorial we will be learning about what Regular Expression or Regex is and what it actually does.  

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.
Regular Expression or Regex in short is a powerful searching tool used to control and move text strings when it comes to processing text files. One line of Regex can replace a whole dozen lines of codes. 
Match Zip Codes (5 digit and 9 digit)
/^[0-9]{5}(-[0-9]{4})?$/
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
Special sequences which match an empty substring:
^ matches at the beginning of the target string
$ matches at the end of the target string
\b matches on a word boundary, i.e., the previous or subsequent character is not a word character
### Quantifiers
Quantifier	Description

*	Match zero or more times.
+	Match one or more times.
?	Match zero or one time.
{ n }	Match exactly n times.
{ n ,}	Match at least n times.
{ n , m }	Match from n to m times.
### Grouping Constructs

### Bracket Expressions
A bracket expression represents a character set via a list of characters enclosed by the square brackets: '[' and ']'. It normally matches the target string with any single character from the list. 
If the character list begins with '^', it matches any single character not from the rest of the list.

If two characters in the list are separated by '–', this is shorthand for the (inclusive) range of characters between those two. It is illegal for two ranges to share an endpoint, e.g. a-c-e. Ranges are collating-sequence dependent and should be avoided for portability.
Most special characters lose their special status and become literals within brackets. Additionally,
– is literal at the end or beginning of a bracket expression
^ is literal if not at the beginning of a bracket expression
\, retains its meaning in bracket expressions, permitting the usage of the special escape sequences: such as \n, \t, \w, \d, etc.
### Character Classes
[...]: Accept ANY ONE of the character within the square bracket, e.g., [aeiou] matches "a", "e", "i", "o" or "u".
[.-.] (Range Expression): Accept ANY ONE of the character in the range, e.g., [0-9] matches any digit; [A-Za-z] matches any uppercase or lowercase letters.
[^...]: NOT ONE of the character, e.g., [^0-9] matches any non-digit.
Only these four characters require escape sequence inside the bracket list: ^, -, ], \.

### The OR Operator
 (|): E.g., the regex four|4 accepts strings "four" or "4".
### Flags
XRegExp provides four new flags (n, s, x, A), which can be combined with native flags and arranged in any order. Unlike native flags, non-native flags do not show up as properties on regular expression objects. 
### Character Escapes
\\ - single backslash

\A - start of a string

\d - single digit [0-9]

\l - match a single lowercase letter [a-z]

\L - single character that is not lowercase [^a-z]

\Q - ignore escaped characters until \E is found

\r - carriage return

\u - single uppercase character [A-Z]

\U - single character that is not uppercase [^A-Z]

\w - word character [a-zA-Z0-9_] 

## Author
Regular expression for parsing an author string into an object following npm conventions.

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)

Reycel Huffman is new to coding. I'm learning all about html, css, javascript, nodes, MYSQL. 
Here's my GitHub link:
https://github.com/reycelhuffman

