# REGEX EXPLAINED



## Summary
The replaceAll() method returns a new string with all matches of a pattern replaced with something else.The pattern can be a string or a RegExp and the replacement can be a string or a function to be called for each match.

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
^The matches any string that starts with The 

end$ matches a string that ends with end

^The end$  exact string match (starts and ends with The end)

roarmatches any string that has the text roar in it

### Quantifiers
abc* matches a string that has ab followed by zero or more c 

abc+  matches a string that has ab followed by one or more c

abc?   matches a string that has ab followed by zero or one c

abc{2}  matches a string that has ab followed by 2 c

abc{2,}  matches a string that has ab followed by 2 or more c

abc{2,5}  matches a string that has ab followed by 2 up to 5 c

a(bc)*   matches a string that has a followed by zero or more copies of the sequence bc

a(bc){2,5}  matches a string that has a followed by 2 up to 5 copies of the sequence bc

### Grouping Constructs

x|y   Matches either "x" or "y". For example, /green|red/ matches "green" in "green apple" and "red" in "red apple".

[xyz] and [a-c] A character class. Matches any one of the enclosed characters. You can specify a range of characters by using a hyphen, but if the hyphen appears as the first or last character enclosed in the square brackets it is taken as a literal hyphen to be included in the character class as a normal character.

[^xyz] and [^a-c] A negated or complemented character class. That is, it matches anything that is not enclosed in the brackets. You can specify a range of characters by using a hyphen, but if the hyphen appears as the first or last character enclosed in the square brackets it is taken as a literal hyphen to be included in the character class as a normal character.


(x) Matches x and remembers the match.

\n Where "n" is a positive integer. A back reference to the last substring matching the n parenthetical in the regular expression (counting left parentheses).

\k<Name> A back reference to the last substring matching the Named capture group specified by <Name>.

(?<Name>x) Matches "x" and stores it on the groups property of the returned matches under the name specified by <Name>. The angle brackets (< and >) are required for group name.


### Bracket Expressions
[abc] a or b or c

[^abc] any character _except_ a, b, or c (negation)

[a-zA-Z]  a through z or A through Z, inclusive (range)

### Character Classes
Square brackets [ ] — means exactly one character

A leading ^ negates, a non-leading, non-terminal - defines a range:

### The OR Operator

a(b|c) matches a string that has a followed by b or c (and captures b or c)

a[bc]      same as previous, but without capturing b or c

### Flags

### Character Escapes

## Author

https://github.com/Maneira3232