# Computer Science for Javascript: Regex Tutorial 
In this Regex Tutorial we will be learning about what Regular Expression or Regex is and what it actually does.  

## Summary
Regular Expression or Regex in short is a powerful searching tool used to find pattern within a text string. Two most common used for Regex is to validate text and search through text, one line of Regex can replace a whole dozen lines of codes. 


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
An achor limits a match to a particular location in the string. 
Special sequences which match an empty substring:
A caret (^) matches at the beginning of the target string "^The" 
A dollar sign ($) matches at the end of the target string "text$"
\b matches on a word boundary, i.e., the previous or subsequent character is not a word character

### Quantifiers
Quantifiers indicate numbers of characters or expressions to match.
Examples: 
*	Match zero or more times.
+	Match one or more times.
?	Match zero or one time.
{ n }	Match exactly n times.
{ n ,}	Match at least n times.
{ n , m }	Match from n to m times.

### Grouping Constructs

### Bracket Expressions
A bracket expression represents a character set via a list of characters enclosed by the square brackets: '[' and ']'. 
It normally matches the target string with any single character from the list. 
If the character list begins with '^', it matches any single character not from the rest of the list.
If two characters in the list are separated by '–', this is shorthand for the (inclusive) range of characters between those two. 
It is illegal for two ranges to share an endpoint, e.g. a-c-e. Ranges are collating-sequence dependent and should be avoided for portability.
Most special characters lose their special status and become literals within brackets. Additionally,
– is literal at the end or beginning of a bracket expression
^ is literal if not at the beginning of a bracket expression
\, retains its meaning in bracket expressions, permitting the usage of the special escape sequences: such as \n, \t, \w, \d, etc.

### Character Classes
[...]: Accept ANY ONE of the character within the square bracket, e.g., [aeiou] matches "a", "e", "i", "o" or "u".
[.-.] (Range Expression): Accept ANY ONE of the character in the range, e.g., [0-9] matches any digit;
[A-Za-z] matches any uppercase or lowercase letters.
[^...]: NOT ONE of the character, e.g.,
[^0-9] matches any non-digit.
Only these four characters require escape sequence inside the bracket list: ^, -, ], \.

### The OR Operator
 Alternation or "OR" is a vertical line character (|): 
 Examples: 
 E.g., the regex four|4 accepts strings "four" or "4".
 A|B|C means one of expressions A, B or C. 
 I love HTML|CSS matches I love HTML or CSS. 
 
### Flags
Flags are placed in the end of Regex, after the second slash there's difference ways it works or end a regex. 
There are 6 flags in Javascript: 
i - search is case-insensitive: no difference between A and a.
g - search looks for all matches, without it- only first match is returned.
m - multiline mode (mode of anchors ^$, flag "m"). 
s - "dotall" mode that allows a dot (.) to match a newline character \n 
u - unicode support. It allows correct processing of surrogate pairs. 
y - "sticky" searching at the exact point in text. 

### Character Escapes
A set of character that can  happen in a string to fufill a match. 
Examples: 
\\ - single backslash
\A - start of a string
\d - single digit [0-9]
\l - match a single lowercase letter [a-z]
\L - single character that is not lowercase [^a-z]
\Q - ignore escaped characters until 
\E - is found
\r - carriage return
\u - single uppercase character [A-Z]
\U - single character that is not uppercase [^A-Z]
\w - word character [a-zA-Z0-9_] 

## Author
Reycel Huffman is new to coding. I'm learning all about html, css, javascript, nodes, MYSQL. 
Here's my GitHub link:
https://github.com/reycelhuffman

