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


