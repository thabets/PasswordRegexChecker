# Title (Password Validation Through Regex)

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
- [Author](#author)

## Regex Components
``
### Anchors
``
In a Regular Expression or more commonly known Regex anchors play a key role in identifying how the engine matches the string. A basic understanding of an anchors role is to tell the regex engine where they can begin and where to end. The anchors utilized in this regex example are `^` to begin and `$` to end.
``
### Quantifiers
``
Quantifiers come in many different forms but for this example there are three specific quantifiers we utilized. First is `?` quantifier which requires a single instance of a character to be available, the second is `*` quantifier which will require multiple instances of a character or condition. Although those are conditions for the quantifiers we utilize them in a manner to establish an at least condition.
``
`?=.*[a-z]` This block of code means that we would require at least one lower case letter. 
``
`?=.*[A-Z]` This block of code would require at least one Upper case letter.
``
The rest of the code follows this pattern to require either special characters or numbers.
``
But wait, we could see that there is another quantifier remaining that we need to emphasize on which is `{8,32}`. This functions as a different type of quantifying restriction for the regex expression. Instead of telling the engine to search the string for a specific type of information, it is setting a constraint that the string needs to be at least 8 characters long and not longer than 32 characters. We are also able to modify such constraints by for example `{8,}` as shown in the code which means that the min length of the password can not be lower than 8 characters but can be infinitely long.
``

### Flags
``
Although there are no Flags within this example the implementation of them are simple if we would like to establish a certain constraint. A flag functions a search pattern for the regex engine, which means that we can require a specific word to be included within the password and that is done by utilizing the `/` characteristic within regex. This ultimately means that we utilize regex to search for a specific string within those two slashes such as `/abc/`. 
``
### Grouping and Capturing
``
Within regex or basically any string of code we naturally utilize grouping and capturing without noticing it. The concept of grouping and capturing is simple, it is basically a way to treat multiple characters as a single unit utilizing parenthesis. Such as done with a function in a block of code. In our code we utilize this more than once as demonstrated below:
``
This block states at least one special character:
``
`(?=.*[!@#\$%\^&\*])`
``
This block states at least one number:
``
`(?=.*[0-9])`
``
As you can see we utilize this to identify what each characteristic should the regex search engine search for. It follows a similar methodical approach as the anchors but instead of looking through all the options it is specific to a single grouped parameter as a constraint.
``


## Author
``
Sallam Thabet is an Industrial Engineer with experience and emphasis on operational efficiency and excellency.
``
Github: thabets
