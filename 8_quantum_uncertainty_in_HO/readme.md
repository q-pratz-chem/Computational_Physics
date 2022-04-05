**Exercise 5.13: Quantum uncertainty in the harmonic oscillator**

In units where all the constants are 1, the wavefunction of the 11th energy level of the one-dimensional quantum harmonic oscillator-Le.,
a spinless point particle in a quadratic potential well-is given by
$$\psi_n(x) =  \frac{1}{\sqrt{2^nn!\sqrt(pi)}}e^{-x^2/2}H_n(x),$$

for $n = 0 ... \inf$, where $H_n(x)$ is the $n^{th}$ Hermite polynomial. Hermite polynomials satisfy a relation 
somewhat similar to that for the Fibonacci numbers, although more complex:

$$ H_{n + 1} (x) = 2xH_n(x) - 2nH_{n-1}(x).$$

Q. a) Write a user-defined function H(n,x) that calculates $H_n(x)$for given x and any integer
  $n\geq 0$. Use your function to make a plot that shows the harmonic oscillator wavefunctions 
  for $n = 0, 1, 2 ,3$, all on the same graph, in the range $x = -4$ to $x = 4$. 
  Hint: There is a function factorial in the math package that calculates the factorial of an integer.
  
  
Q. b) Make a separate plot of the wavefunction for $n = 30$ from $x = -10$ to $x = 10$.
Hint: If your program takes too long to run in this case, then you're doing the
calculation wrong-the program should take only a second or so to run.

Q. c)The quantum uncertainty in the position of a particle in the $n^{th}$ level of a harmonic oscillator can
be quantified by its root-mean-square position $\sqrt{\langle x^2\rangle}$, 
where $$\langle x^2\rangle = \int_{-inf}^{inf}x^2|\psi_n(x)|^2 dx$$.
Write a program that evaluates this integral using Gaussian quadrature on 100 points, then calculates 
the uncertainty (i.e., the root-mean-square position of the particle) for a given value of $n$. 
Use your program to calculate the uncertainty for $n = 5$. You should get an answer in the vicinity of $\sqrt{\langle x^2\rangle} = 2.3$.
