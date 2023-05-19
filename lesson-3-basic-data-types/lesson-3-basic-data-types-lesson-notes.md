# Lesson 3. Basic Data Types

C is a strongly typed language. Every value must have a type associated with it. C also does automatic, or implicit, conversions from one type into another.

We can also perform manual, or explicit, conversions with type casting. Type casting is an operation that we might need to do to a value.

The basic data value in C is a byte or a sequence of 8 bits. The set of values a byte can represent is 256.

## Numbers

When negative numbers are needed, we specify them with the **signed** keyword.

Basic integer types
- char
- signed char
- unsigned char
- short, same as signed short, short int, or signed short int
- int
- unsigned, same as unsigned int
- long, same as signed long, long int, or signed long int
- unsigned long, same as unsigned long int
- long long, same as signed long long or signed long long int
- unsigned long long, same as unsigned long long int

When signed/unsigned is not specified, the default might be signed.

The short is guaranteed to be at least 2 bytes but might be longer depending upon the machine.

The int, unsigned, long, and unsigned long types are guaranteed to be at least 4 bytes but might be longer.

The long long and unsigned long long types are guaranteed to be at least 8 bytes but might be longer.

C99 added integer types that specify the exact width, the fastest width, and the minimum width of integer values.
- The `int<n>_t or uint<n>_t` forms for exact width integer types
- The `int_least<n>_t or uint_least<n>_t` forms for the smallest width of an integer (might be larger).
- The `int_fast<n>_t or uint_fast<n>_t` forms for the fastest width for an integer in that implementation.

<n> is either 8, 16, 32, or 64.

These types are defined in stdint.h and inttypes.h files.

Fractional numbers
- float, 4 bytes
- double, 8 bytes
- long double, 16 bytes

## Characters

Summarizing ASCII's organization
- 0..31, control characters for printing and device communication
- 32..63, punctuation and numbers
- 64..95, uppercase alphabet plus miscellaneous punctuation
- 96..127, lowercase alphabet plus miscellaneous punctuation
- 128..255, not used

## Boolean

Before C99, there was no explicit type for a Boolean. A value of any type that is 0 is considered as also evaluating to a Boolean false. Any value other than 0 will evaluate to a Boolean value of true. 

Since C99, a `_Bool` type was added, which, when evaluated, will always evalute to only 0 or 1. When we include stdbool.h file, we are able to use the bool type as well. Also, in stdbool.h, true and false are defined. 

## Size and range

The sizeof() operator a builtin function that takes a C data type a its parameter and returns the number of bytes for that data type. 
The return type of sizeof() is `size_t`, analogous to unsigned long. 

Ranges for each data type are defined in limits.h and float.h for real number limits.
- SCHAR_MIN, SCHAR_MAX - int8_t
- SHRT_MIN, SHRT_MAX - int16_t
- INT_MIN, INT_MAX - int32_t
- LLONG_MIN, LLONG_MAX - int64_t
- UCHAR_MAX - uint_8_t
- USHRT_MAX - uint_16_t
- UINT_MAX - uint32_t
- ULLONG_MAX - uint64_t
- FLT_MIN, FLT_MAX - float
- DBL_MIN, DBL_MAX - double
- LDBL_MIN, LDBL_MAX - long double


