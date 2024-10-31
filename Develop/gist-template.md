# Title (replace with your title)

This is a Tutorial on regex expression and or regular expression.

## Summary

In this Tutorial we will be breaking down a regex expression for an email address.
This is the regex expression that we will be breaking down  /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

([a-z0-9_\.-]+): This is the first capturing group.
[a-z0-9_\.-]: This is a character class that matches any lowercase letter (a-z), digit (0-9), underscore (_), period (.), or hyphen (-).
+: This quantifier means "one or more" of the preceding character class. So, this part matches one or more characters that are valid in the username part of an email address.
@: This matches the literal @ symbol, which is a required part of an email address.


([\da-z\.-]+): This is the second capturing group.

[\da-z\.-]: This character class matches any digit (0-9), lowercase letter (a-z), period (.), or hyphen (-). The \d is a shorthand for digits.
+: Again, this means "one or more" of the preceding character class. This part matches the domain name of the email address.
\.: This matches a literal period (.). The backslash (\) is used to escape the period, as a period normally matches any character in regex.


([a-z\.]{2,6}): This is the third capturing group.

[a-z\.]: This character class matches any lowercase letter (a-z) or period (.).

{2,6}: This quantifier specifies that the preceding character class must occur between 2 and 6 times. This part matches the top-level domain (like .com, .org, etc.) of the email address.
    $: This asserts the end of a line. It means that the pattern must match until the end of the string.
    
    This regex pattern is designed to validate email addresses by ensuring they follow a specific structure: a valid username, followed by the @ symbol, a valid domain name, a period, and a valid top-level domain.





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
Anchors are used to specify the position of the pattern in relation to a line of text.
^ anchor signifies a string that begins with the characters that follow it

### Quantifiers
Quantifiers are used to quantify how many times a part of your regular expression should be repeated.

### OR Operator
An operator is a code element that performs an operation on one or more code elements that hold values. Value elements include variables, constants, literals, properties, returns from Function and Operator procedures, and expressions

### Character Classes
A character class is a special notation that matches any symbol from a certain set

### Flags
A flag is an optional parameter to a regex that modifies its behavior of searching

### Grouping and Capturing
Parentheses group the regex between them. They capture the text matched by the regex inside them into a numbered group that can be reused with a numbered backreference. They allow you to apply regex operators to the entire grouped regex.

### Bracket Expressions
A bracket expression is either a matching list expression or a non-matching list expression. It consists of one or more expressions: ordinary characters, collating elements, collating symbols, equivalence classes, character classes, or range expressions.
[] represent the exact number of characters in the string 

### Greedy and Lazy Match

Greedy: .* (matches as many characters as possible)
Lazy: .*? (matches as few characters as possible)

### Boundaries
Positions in a string where the character on the left differs from the character on the right in terms of whether they are word characters (a-z, A-Z, 0-9, _) or not. These positions are not actual characters but rather positions.

### Back-references
Regular expression commands which refer to a previous part of the matched regular expression

### Look-ahead and Look-behind
Will find only those matches for a pattern that are followed or preceded by another pattern.Also referredto as look around .

## Author

Anthony Black https://github.com/anthonyblack1992
