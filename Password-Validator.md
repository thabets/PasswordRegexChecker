# Title (Password Validation Through Regex)

Introductory paragraph (replace this with your text)
Regular Expressions also known as Regex is an important and very valuable tool that developers use in all forms of coding. It is simply defined as a sequence of characters that are utilized to search for specific patterns. One might inquire as to the type of patterns that could be beneficial in making this an important tool. From personal experience, one of the most important aspect we could encounter on our daily use is the relationship between the user of software and the software itself. When developers utilize Regex, it is to clearly set acceptable parameters towards the utilization of a certain interactive system that means that the developer attempt to set certain parameters around the information that is acceptable for a user to input into a website, game or productivity software. Now imagine a database that would return a spreadsheet to management regarding expenditures, this software has three inputs. First input is the amount in $, the second input is the purpose and lastly the third input is the email associated with the account of the user who utilized such expenditures. In the case of Regex we would like to validate the input, the user is supposed to enter is accurate and acceptable to the database to proceed. Regex could be used in this case, first to validate the input to the third field was indeed an email, an input to the purpose was a string and an input to the monetary field was indeed a number with only two decimal places or the nearest hundredth. As you can see regex can be used in many different forms but the most utilized form is determining a password meets a certain criteria also the strength of a password.

## Summary

For this project we will look as to how to utilize regex in validating a password with certain constraints as well as future possibilities and changes as towards the parameters of such password. Also how to utilize regex in determining the strength of a password.

^(?=.*[a-z])(?=.*[A-Z])(?=.*[0-9])(?=.*[!@#\$%\^&\*])(?=.{8,})$

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

In a Regular Expression or more commonly known Regex anchors play a key role in identifying how the engine matches the string. A basic understanding of an anchors role is to tell the regex engine where they can begin and where to end. The anchors utilized in this regex example are `^` to begin and `$` to end.

### Quantifiers

There are

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