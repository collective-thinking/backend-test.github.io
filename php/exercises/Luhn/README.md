# Luhn

Given a number determine whether or not it is valid per the Luhn formula.

The [Luhn algorithm](https://en.wikipedia.org/wiki/Luhn_algorithm) is
a simple checksum formula used to validate a variety of identification
numbers, such as credit card numbers and Canadian Social Insurance
Numbers.

**Your task is to implement the `isValid($str): bool` method. 
It should return `true` if the given string is valid and `false` otherwise.**

Validating a Number
------

Strings of length 1 or less are not valid. Spaces are allowed in the input,
but they should be stripped before checking. All other non-digit characters
are disallowed.

## Example 1: valid number

```text
4539 1488 0343 6467
```

The first step of the Luhn algorithm is to double every second digit,
starting from the right. We will be doubling

```text
4_3_ 1_8_ 0_4_ 6_6_
```

If doubling the number results in a number greater than 9 then subtract 9
from the product. The results of our doubling:

```text
8569 2478 0383 3437
```

Then sum all of the digits:

```text
8+5+6+9+2+4+7+8+0+3+8+3+3+4+3+7 = 80
```

If the sum is evenly divisible by 10, then the number is valid. This number is valid!

## Example 2: invalid number

```text
8273 1232 7352 0569
```

Double the second digits, starting from the right

```text
7253 2262 5312 0539
```

Sum the digits

```text
7+2+5+3+2+2+6+2+5+3+1+2+0+5+3+9 = 57
```

57 is not evenly divisible by 10, so this number is not valid.

## Example 3: valid and invalid characters

Valid strings should only contain numbers and spaces

Blank spaces should be ignored. `59` and `5 9` are both **valid**.

Strings containing other non numerical characters like the followings are considered **invalid** 

```text
5-9
$59
a59
```
