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

