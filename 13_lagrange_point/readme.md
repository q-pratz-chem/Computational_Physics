## Exercise 6.16: The Lagrange point

There is a magical point between the Earth and the Moon, called the L1 Lagrange point, 
at which a satellite will orbit the Earth in perfect synchrony with the Moon, staying always in 
between the two. This works because the inward pull of the Earth and the outward pull of the Moon 
combine to create exactly the needed centripetal force that keeps the satellite in its orbit. Here's the setup:

![image](/Lagrange_point_diagram.png)

(a) Assuming circular orbits, and assuming that the Earth is much more massive than either the Moon or the satellite,
show that the distance r from the center of the Earth to the L1 point satisfies

$$\frac{GM}{r^2} - \frac{Gm}{(R-r)^2} = w^2r$$


where 

$$\begin{split}
R & \quad \text{the distance from the Earth to the Moon}\\
M,m & \quad \text{the masses of Earth and Moon, respectively,}\\
G & \quad  \text{Newton's gravitational constant},\\ 
w & \quad \text{the angular velocity of both the Moon and the satellite.}
\end{split}$$


(b) The equation above is a degree-five polynomial equation in $r$ (also called a quintic equation).
Such equations cannot be solved exactly in closed form, but it's straightforward to solve them numerically.
Write a program that uses either Newton's method or the secant method to solve for the distance r from the 
Earth to the L1 point. Compute a solution accurate to at least four significant figures. The values of the various parameters are:

$$\begin{split}
G &= 6.674 x 10^{-11}m^3kg^{-1}s^{-2},\\
M &= 5.974 x 10^{24} kg, \\
m &= 7.348 x 10^{22} kg,\\
R &= 3.844 x 10^8 m, \\
w &= 2.662x10^{-6} s^{-1}.
\end{split}$$

You will also need to choose a suitable starting value for r, or two starting values if you use the secant method.
