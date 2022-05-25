## Exercise 2.12: Prime numbers

The program in Example 2.8 is not a very efficient way of calculating prime numbers: it checks each number to see if it is 
divisible by any number less than it. We can develop a much faster program for prime numbers by making use of the following observations:

a) A number $n$ is prime if it has no prime factors less than n. Hence we only need to check if it is divisible by other primes.

b) If a number $n$ is non-prime, having a factor r, then $n = rs$, where $s$ is also a factor. 
If $r \geq \sqrt{n}$ then $n = rs \geq \sqrt{ns}$, which implies thats $s \leq \sqrt{n}$. 
In other words, any non-prime must have factors, and hence also prime factors, less than or
equal to $\sqrt{n}$. Thus to determine if a number is prime we have to check its prime factors
only up to and including $\sqrt{n}$-if there are none then the number is prime.

c) If we find even a single prime factor less than $\sqrt{n}$ then we know that the number
is non-prime, and hence there is no need to check any further-we can abandon this number and move on to something else.


Write a Python program that finds all the primes up to ten thousand. Create a list to store the
primes, which starts out with just the one prime number 2 in it. Then for each number n from 3 to 10000 
check whether the number is divisible by any of the primes in the list up to and including $\sqrt{n}$. 
As soon as you find a single prime factor you can stop checking the rest of them-you know n is not a prime.
If you find no prime factors $\sqrt{n}$ or less then n is prime and you should add it to the list. 
You can print out the list all in one go at the end of the program, or you can print out the individual
numbers as you find them.
