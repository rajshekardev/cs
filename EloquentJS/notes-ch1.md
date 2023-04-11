# EloquentJS

## Chapter 1

- Values, Types & Operators

### Numbers

- Javascript uses 64 bits to make numbers.
  [ ] with N decimal digits you can represent 10^N numbers
  [ ] given 64 binary digits you are limited to 2^64
  about 18 quintillion(18 with 18 zeroes)

  - the first bit denotes sign of the number.
  - some bits are used to store decimal position
  - the actual maximum is like 9 quadrillion(15 zeroes)

  fractions are written with a dot.

  for large numbers you use scientific notation
    which is written as 2.998e9 = 2.998 x 10^8

- whole number smaller than 9 quadrillion are always precise
- calculations with fractional numbers are generally nor precise.

pi cannot be represented with precise decimal value similarly
other decimals cannot be represented with precise values because
of 64bit constraint.

TLDR: fractional values not precise

### Arithmetic - ArthaShastra

JS Arithmetic Operators
  
 "+ , - , * , / , % (Follows BODMAS rule) "
  
special numbers
  Infinity , -Infinity , NaN

    0/0 = NaN
    Infinity - Infinity = NaN
    NaN != NaN

### String
  
  'Down on the sea' - Single quote
  "Lie on the Ocean" - double quotes
  `Float on the Ocean` - backtics

  things to escape

- "\n" - new line
- "\t" - tab

  JS uses unicode text so every character is represented using 16bit number
  JS is limited by 16 bit for characters so emojis which are represented with
  numbers higher than 16bit in unicode spec are represented with 2 characters

  a letter is represented by 16 bit number
  a emoji takes 2 character positions.

 String cannot be divided, multiplied or subtracted.
 "+" Operator works on string and concatenates them together

 string values have a few functions built into them. discussed in chapter 4

### Strings enclosed in backticks are String Literals

    they can embed compute statements with ${} syntax.
    they are able to span to multiple lines.


    ``` JS
    let a = 10
    `half of 100 is ${100 / 2}`
    
    `a value is ${a}`

    ```

### Operator types

#### Unary Operators

    - Operators that work on one value
  "  - (minus) , typeof() , !(not) "

  minus Operator makes a value negative
  typeof Operator returns the data type of the value
  not Operator inverses the value

#### Binary Operators

  Work on two values such as all.
  Arithmetic Operators, &&, ||,<,>,<=,>= etc.

  all require two values to operate on so they are called binary operators

## Boolean Value

boolean value holds either true or false.

<, > and <= , >= all produce boolean values.

- Strings are orderd alphabetically
- Uppercase is lower than lowercase so "Z" < "a" is true
- Non alphabetic characters are also included in the ordering.

### Logical operators

&& , || and ! are logical operators

#### Ternary operator

operates on 3 values

    ```
    console.log(true ? 1 : 2);
    ```

#### Empty Values

null and undefined are empty values.
  Bad design led to their creation.
  they are both same most of the time.

## Automatic Type conversion

JS converts types when neccessary

    ```
     console.log(8 * null) // 0
     console.log("5" - 1) // 4
     console.log("five")  // NaN
     console.log(false == 0) // true
    ```

when an operator is applied to wrong type of value. JS does
convert the values and try to make sense using a set of rules.

This is called type coercion
