# Amicable

Write a program called `amicable.py` that prompts the user to input an upper bound (a positive integer). The program should then find and display all pairs of *amicable numbers* below that upper bound.

![embed](https://www.youtube.com/embed/fUSZBVYZdKY?si=3_01Crs-h7IcUhNc)

Two numbers are considered amicable if the sum of the proper divisors of the first number equals the second number, and the sum of the proper divisors of the second number equals the first number. Proper divisors of a number are all divisors excluding the number itself. For example, 220 and 284 are *amicable numbers* because the sum of the proper divisors of 284 is 1 + 2 + 4 + 71 + 142 = 220, and the sum of the proper divisors of 220 is 1 + 2 + 4 + 5 + 10 + 11 + 20 + 22 + 44 + 55 + 110 = 284

## Requirements:

1. Prompt the user to input an upper bound (`n`), and ensure the input is a positive integer. If the input is invalid or less than 1, keep asking the user for a valid number.
2. For every number less than `n`, calculate the sum of its proper divisors.
3. Find and print each pair of amicable numbers in the format.

### Example Usage:

    Enter an upper bound: 300
    220 is amicable with 284!
    284 is amicable with 220!

### Example Usage 2:

    Enter a upper bound: 5000
    220 is amicable with 284!
    284 is amicable with 220!
    1184 is amicable with 1210!
    1210 is amicable with 1184!
    2620 is amicable with 2924!
    2924 is amicable with 2620!

## Testing

To be sure test your program again using `checkpy`:

    checkpy amicable
