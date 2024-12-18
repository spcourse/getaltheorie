# Eratosthenes

Write a program called `eratosthenes.py` that uses the **Sieve of Eratosthenes** to calculate the number of prime numbers below a given number.

![embed](https://www.youtube.com/embed/klcIklsWzrY?si=60GPtxiA_gjVAtIK)

Beware, implementing this algorithm correctly in Python might be trickier than it seems!

## Requirements:

1. Prompt the user to enter an integer (`n`) and ensure that the input is at least 3. If the input is invalid or less than 3, continue asking the user for a valid number.
2. Use the **Sieve of Eratosthenes** to efficiently count all prime numbers below `n`
3. Efficiency is important! A correctly implemented sieve should be able to count all prime numbers up to 10,000,000 within a few seconds. (On a reasonably fast computer even primes up to 100,000,000 shouldn't take much more than about 10 seconds.)

### Example Usage 1:

    Count primes below: 10
    There are 4 prime numbers below 10.

### Example Usage 1:

    Count primes below: 10000000
    There are 664579 prime numbers below 10000000.

## Testing

To be sure test your program again using `checkpy`:

    checkpy eratosthenes
