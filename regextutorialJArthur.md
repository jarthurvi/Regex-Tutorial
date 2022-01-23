# Title Ultimate Regex Tutorial

Introductory paragraph  Regular expressions, or regex for short, are a series of special characters that define a search pattern.

## Summary
Here are some regex examples.

* Matching a Hex Value: `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`
 Checks to see if a string fulfills the requirements for a hex value.
 
* Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
Checks to see if a string fulfills the requirements for a matching email.

* Matching a URL: `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`
Checks to see if a string fulfills the requirements for a matching URL.

* Matching an HTML Tag: `/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/`
Checks to see if a string fulfills the requirements for a matching HTML tag.


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

Signifies a string that begins with the characters that follow it. 

`/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/`

"^" and "$" are anchors.
    
### Quantifiers
Quantifiers set the limits of the string that your regex matches (or an individual section of the string). They frequently include the minimum and maximum number of characters that your regex is looking for.

    *—Matches the pattern zero or more times

    +—Matches the pattern one or more times

    ?—Matches the pattern zero or one time
    
   Adding a "?" symbol to any search will return the fewest amount of possible matches.
   
   
EXAMPLE STRING : `/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/` : Here we see this string has several quantifiers.

### Grouping Constructs
`/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/`

Checks multiple parts of a string to determine that different sections fulfill different requirements.
For Example: (?:>(.*)
They look for exact matches so if (abc):(xzy) were seen this would not match even though all the right letters are there but they 
are not in the same order so they will not be seen as a match.

### Bracket Expressions
A bracket expression is either a matching list expression or a non-matching list expression enclosed by two brackets [].
 `/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/`
ex. [a-z]

### Character Classes
Character classes exist within bracket expressions often as multiple within each expression. Each character class designates a set of characters equivalent to the corresponding standard. ex. alpha, digit, etc.
`/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/`
ex. "." (Matches any character except the newline character (\n))
### The OR Operator
Returns the boolean value true if either or both operands is true and returns false otherwise.
`/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/`
ex. "|" <\/\1>|\s+\/>

### Flags
Flags are tokens that modify its behavior of searching.
`/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/`
ex. "s" |\s+\/>)$/`

### Character Escapes
The backslash (\) in a regex escapes a character that otherwise would be interpreted literally.
`/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/`
ex. `/^<([a-z]+)


## Author

Joseph Arthur is new to the world of coding and web development but really enjoying this new experience. 
GitHub Page Link: https://github.com/jarthurvi
