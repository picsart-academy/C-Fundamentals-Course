# Lesson 2. Understanding Program Structure

A **digraph** in C is a two-character sequence, which means something more than either of the characters alone. For example, \n digraph, which represents the <newline> character to be output to the console.

Digraphs that appear in strings are also called **escape sequences** (they escape from the normal meaning of every single character).

- \a Alert
- \b Backspace
- \f Form feed (page advance)
- \n Newline
- \r Carriage return
- \t Horizontal tab
- \v Vertical tab
- \' Single quote
- \" Double quote
- \? Question mark
- \\ Backslash itself
  
```
"Hello, world without a new line"
"Hello, world with a new line\n"
"A string with \"quoted text\" inside of it"
"Tabbed\tColumn\tHeadings"
"A line of text that\nspans three lines\nand completes the
line\n"
```

Delimiters are characters that are used to separate tokens. When a token is predefined by C, it cannot be used except in a prescribed way. While int, return, and include are keywords, main is not a keyword. Every C program must have a single function named main() as the entry point for the program.

```
#include <stdio.h>

int main() {
    printf("Hello, world!\n");
    return 0;
}
```

Delimiters in the code above
- single delimiters: ; and <space>
- paired, symmetric delimiters: <>, (), {}, and ""
- Asymmetric delimiters that begin with one character and end with another: # and <newline> and // and <newline>

The code could be rewritten like this
```
#include <stdio.h>
int main(){printf("Hello, world!\n");return 0;}
```

List of delimiters
- <space>, basic token separator or whitespace
- <newline>, terminating delimiter for preprocessor directives and C++-style comments or whitespace
- ;, statement terminator
- //, beginning of a comment
- #, beginning of a preprocessor directive (octothorp)
- < >, filename delimiters are used in a preprocessor directive when used in pairs
- { }, block delimiters
- ( ), function parameter delimiters. Also used for expression grouping
- " ", string delimiters or filename delimiters in preprocessor directives for multiple characters
- ' ', character delimiters for single characters
- [], array notation

Some of these punctuation marks have different meanings when used in different contexts.

Statements
- simple statements: end with ;. return 0; is a simple statement.
- block statements: begin with { and end with }. 
- complex statements: consist of a keyword, a parenthetical expression, and one or more block statements. main() {...} is a complex statement.
- compound statements: made up of simple statements and/or complex statements that consist of multiple statements. The body of the program above is an example of a compound statement.

some of the examples in the program above
- preprocessor directive: begins with # and ends with <newline>
- function definition statement: the main() function is a function definition.
- function call statement: calling a function.

other statements
- control statement: these include if, else, goto, break, continue. The return statement is also a control statement.
- looping statement: while, do while, for.
- expression statement: simple statements that evaluate expressions and return some kind of result or value.


