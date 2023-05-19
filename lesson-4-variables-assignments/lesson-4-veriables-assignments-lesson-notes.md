# Lesson 4. Variables and Assignments

A variable is a location in memory that holds a value of a specified type that can vary over the life of the variable, identified by its name.

The following components are essential
- A unique identifier or name
- A type
- A value

```
int var;
int var2 = 12;
```

Identifier or name is a sequence of capital and small letters, digits, and the underscore character. An identifier may not begin with a digit.

```
int id1;
int id2;

or

int id1, id2;
```


```
int id1 = 11;
int id2 = 12;

or

int id1 = 11, id2 = 12;
```

Literal constants
- integer constants: 65, 1024
- double constants: 3.5, -0.7
- character constants: 'A', '6'

- octal integers: 07, 011
- unsigned octals: 07u, 011u
- long octals: 07L
- hex integers: 0x4
- unsigned hex: 0x4u
- long hex: ox4L
- float literals: 0.5f
- double literals: 0.5
- long-double: 0.5L

Defined values
- you can use #define to predefine some value (literal)

It's better to use explicitly typed constants
```
const int size = 12;
```

Assignment
```
regular assignment 
int x = 4;

foo(12); // assigning by passing it to the function

int ret = foo(); // assigning from a function return value
```
