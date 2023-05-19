# Lesson 1. Hello, world!

You'd need a terminal window, a text editor, and a C compiler.

The example

```
#include <stdio.h>

int main() 
{
  printf("Hello, world!\n");
  return 0;
}
```

C is a compiled language, which means the output of the compiler is a platform-specific executable.

Programs are generated from text known as source files or source code files. Once compilation has been completed successfully, an executable file will be generated. 
Unless we provide an explicit name for it, the file will be named `a.out`.

To compile a program, type `cc program.c`.

To clarify the code you can use comments.

```
/* A single-line C-style comment */

/*
A multi-line
C-style comment
*/

// A C++ style comment
```

Experiment with code.
