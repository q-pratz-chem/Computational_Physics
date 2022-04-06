## Exercise 8.15 The double pendulum

If you did Exercise 8.4 you will have created a program
to calculate the movement of a nonlinear pendulum. Although it is nonlinear, the non-
linear pendulum's movement is nonetheless perfectly regular and periodic-there are
no surprises. A double pendulum, on the other hand, is completely the opposite---chaotic
and unpredictable. A double pendulum consists of a normal pendulum with another
pendulum hanging from its end. For simplicity let us ignore friction, and assume that
both pendulums have bobs of the same mass m and massless arms of the same length e.
Thus the setup looks like this:

![double pendulum](/double pendulum.png)

(a) Derive an expression for the total energy E = T + V of the system in terms of the
variables $\theta_1, \theta_2, \omega_1, and \omega_2$, plus the constants g, l, and m.

(b) Write a program using the fourth-order Runge-Kutta method to solve the equations of
motion for the case where $l = 40cm$, with the initial conditions $\theta_1 = \theta_2 =
90°$ and  $\omega_1 = \omega_2 = 0$. Use your program to calculate the total energy of the 
system assuming that the mass of the bobs is 1 kg each, and make a graph of energy
as a function of time from t = 0 to t = 100 seconds.

Because of energy conservation, the total energy should be constant over time
(actually it should be zero for these particular initial conditions), but you will find
that it is not perfectly constant because of the approximate nature of the solution
of the differential equations. Choose a suitable value of the step size h to ensure
that the variation in energy is less than $10^{-5}$ joules over the course of the calculation.
