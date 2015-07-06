# Internship2015
Intro challenges for the 2015 Internship

When solving you should focus on producing clear, easy to understand code. If you have questions, don't hesitate to ask. You should try to create efficient solutions, but main goal is readability. 

## Problem 1:
Write a program that generates all two-word (from the attached wordlist.txt) anagrams of the string "documenting". [wordlist.txt](https://github.com/Recognos/Internship2015/blob/master/wordlist-problem1.txt) 

## Problem  2:
Write a program that solves word-chain puzzles. There’s a type of puzzle where the challenge is to build a chain of words, starting with one particular word and ending with another.
Successive entries in the chain must all be real words, and each can differ from the previous word by just one letter. For example, you can get from “cat” to “dog” using the following chain: "cat" - "cot" - "cog" - "dog".
[wordlist2.txt](https://github.com/Recognos/Internship2015/blob/master/wordlist-problem2.txt)

## Problem 3:
Convert a numeric string to integer (of float) without using any builtin conversion functions

## Problem 4:
Given a file containing one word per line, print out all the combinations of words that are anagrams; each line in the output contains all the words from the input that are anagrams of each other.

## Problem 5:
 
I call it the “word break” problem and describe it as follows:
 
Given an input string and a dictionary of words,
segment the input string into a space-separated
sequence of dictionary words if possible. For
example, if the input string is "applepie" and
dictionary contains a standard set of English words,
then we would return the string "apple pie" as output.
 
## Problem 6:
Converting Arabic to Roman: We would like to be able to convert Arabic numbers into their Roman numeral equivalents. We just need some kind of program that can accept a numeric input and output the Roman numeral for the input number.


## Problem 7:
Create a tool that will allow you to preview an image file at the command-line in pure text.
Your program will need to read in an image, in whatever format you want to support, and respond with a text representation of the image that fits in the terminal.
For example, given the image:
Ducky
Your program might respond with something like:
```
........--**####**::::::::::::........
......--##oooooo\\**::::::::..........
......**oo==oooo\\\\::::..............
....--\\oooooooo\\$$**::..............
....**&&$$oooo\\$$$$%%................
....**\\oooo\\<<<<$$##................
....!!<<<<<<<<<<\\\\##..........::::::
....::%%<<<<<<<<\\$$^^....::**++**....
....^^%%<<<<<<<<$$$$##**""==++++==****
....**oo<<<<<<$$<<<<\\oo==++++++==""""
..!!==oo<<<<<<<<$$$$oo====++++==oo####
^^====oo\\<<$$\\oooooo==++======oo****
**++++====oooo====++++======oooo\\^^^^
++====++++========++======oooooo**....
""====++++==========oooooooooo##--....
""==================oooooooooo^^......
!!oo==oo======oooooooooo\\##^^::......
..""oooooooooooooooo\\oo""^^..........
..::**====oooooooooo==**::............
....::^^**""""""""!!..--::............
....::^^**""""""""!!..--::............
```
Go for as much accuracy as you can possibly squeeze out of it.

## Problem 8

#### Source: https://mindcoding.ro/pb/printf

You are given n _variable declaration_s and a _printf instruction_. You must display the output of the instruction.
 A _variable declaration_ is a string of the form `name=value`, where `name` is a single lowercase letter of the latin alphabet.
 The _printf instruction_ is a greatly simplified version of the homonymous C function. For this problem:

A _printf instruction_ is a string of the form `_format_string_, arg1, arg2, ...` (with 0 or more arguments)
 A _format_string_ is a sequence of words, separated by spaces (exactly one space between each two consecutive words). The words which start with a `%` are special; they are called format specifiers. The `i`th format specifier will be replaced with the value of the `i`th variable, formatted according to these rules:

*   If the format specifier is `%s`, the value is a string which should be printed directly
*   If the format specifier is `%WIDTHd`, the value is an integer which should be padded with spaces until it is WIDTH characters long, then printed. Thus:
    *   If the value is 5 and the format string is `%3d`, print `" 5"` (without the quotes).
    *   If the value is 100 and the format string is `%3d`, print `"100"` (without the quotes).
*   If the format specifier is `%.PRECISIONf`, the value is a decimal number which should be rounded to PRECISION digits after the decimal point, then printed. Thus:
    *   If the value is 5.31 and the format string is `%.2f`, print `"5.3"` (without the quotes).
    *   If the value is 3.14159 and the format string is `%.4f`, print `"3.1416"` (without the quotes).
    *   If the value is 1.1 and the format string is `%.5f`, print `"1.10000"` (without the quotes)
*   All other words (those not starting with `%`) should be printed literally

## Input

`N`, the number of variables, will be on the first line. The next N lines will contain variable declarations (`variable_name=value`, with no spaces next to the `=`).
 The printf instruction (`format,variable_name<sub>1</sub>,variable_name<sub>2</sub>,...,variable_name<sub>n</sub>`, with one comma between each two arguments) will be on the last line.

## Output

The output of the instruction will be on solely one line.

## Constraints

The names of the variables are made up of one letter.
 The format string will **not** contain the character `,`.
`1 ≤ WIDTH, PRECISION ≤ 5`
`1 < N < 10`
 All lines in the input contain less than 100 characters.
 For the `%WIDTHd` format specifier, the integer is at most `WIDTH` digits long.

## Example

| Input | Output |
| --- | --- |
| 2
|o=widgets
|p=13.365
|Buy %s @ %.2f each,o,p | Buy widgets @ 13.37 each |
| 3
|a=1
|b=10
|c=100
|The first three powers of %s are %4d %4d %4d,a,a,b,c | The first three powers of 1 are    1   10  100 |
| 2
|b=3
|a=Ana
|%s are %s mere,a,b| Ana are 3 mere |

## Problem 9:
Implement a Secret Santa selection program.
Given a file where each line looks like this :
FIRST_NAME space FAMILY_NAME space <EMAIL_ADDRESS> newline
your program should then choose a Secret Santa for every name in the list, and print in the console the results.
Obviously, a person cannot be their own Secret Santa.
(Optionally: the program will not allow people in the same family to be Santas for each other.)
