# Thousand and one primes

The first prime number is 2, the third prime number is 5, the 1001st prime number is 7927. Implement a program called `1001-primes.py`, that generates the $$n$$-th prime number, where $$n$$ is a user provided value.

    Which prime number are you looking for? 1001
    7927

## Background

As previously mentioned, a computer is a great tool for quickly executing a series of "dumb", or simple, actions. An example of what a computer does a lot better (and quicker!) than humans, is calculating prime numbers. The definition of a prime number is not too complicated. But determining how many divisors a number has could take an enormous amount of time. Python to the rescue!

## Specification

* Prompt the user for the rank (how many-th) of the prime number that they want. This has to be a whole, positive number.

* If the user provides an invalid rank, prompt the user for a new rank. Keep asking the user for a rank until they provide a valid input. Since it is not known how often you'll have to repeat the question, a `while`-loop seems perfect!

* You can however assume the user only provides whole numbers (integers). That means you don't have to take decimal numbers into considerations.

* Once the rank of the prime is established, have your program calculate the correct prime and report it back to the user.

* Make sure that your program does not output anything other and the prime number, just like in the example above!

### Constraints

The same as before:

* You are only allowed to use the concepts that are discussed in this module.
* You are *not* allowed to use the `break`-statement.
* You are *not* allowed to use the `import`-statement.

## Problem analysis

As always, take a couple of minutes of time, before any coding, to draw the problem with **pen and paper**. How would you divide the problem into smaller and simpler steps.

In this assignment, we'll guide you through some of the steps.

## Step 1: use previous solutions.

You're not starting from scratch, beacause you already wrote `check-prime.py`. Copy that solution as a starting point for this problem.

## Step 2: check all numbers smaller than 100

Let's take it a step further. We can reuse our code from before and for *each* number smaller than 100 determine whether it is a prime number or not.

Create an extra `for`-loop to check each number smaller than 100 and determine for each of these "candidate primes" whether it is or isn't a prime number. For each number you'll have to determine the divisors individually, so you'll be needing two `for`-loops inside of one another (*nested loops*).

Implement aforementioned procedure and make sure it works correctly. Next we'll want to expand the procedure by `print`ing each found prime number. So after each conclusion of whether a number is a prime, we'll need a `print`-statement.

Is your answer correct? Verify on the web!

## Step 3: the umpteenth prime

Now let's get back to the assignment: finding the n-th prime number. We'll assist you a bit in the strategy for the program:

* You cannot simply loop with a `for`-loop til `n`. Since we ant the `n`-th prime number; we don't want to know if `n` is a prime number (see the difference with step 2?). So you'll have to keep count *how many* prime numbers you've already found. Use a variable for this.

* Start out small. Make sure your program works for the first 10 prime numbers before you start looking at 10 thousand numbers. Ten is just large enough to test most of the programs functions and small enough that it should be easy to fix mistakes.

* Errors? Print for every candidate-prime some information, so you know what calculation your program is at, than see if your intended strategy is working correctly.

> Maybe it is weird or annoying to write a program, after which you find out that it doesn't work correctly. That is a programmers fate: it's just incredibly difficult to precisely formulate an algorithm and instantly convert it into functioning code. Sometimes you've forgotten an exception or edge case, but just as easily you've made a typo somewhere. Keep in mind even the best programmers have to deal with this!

## Hints

* You only need the Python elements you've learned up until now to correctly implement this program!

## Testing

To be sure test your program again using `checkpy`:

    checkpy 1001-primes
