## Finding eigenvalues

A mass on a spring acting as a simple harmonic oscillator will have a potential energy given by $V = \frac{1}{2}kx^2$ , 
where $x = 0$ defines the equilibrium position of the spring and $k$ is the force constant of the spring (such that $F = −∂V/∂x = −kx)$.
The frequency of oscillation is given by $ w= \sqrt{k/m}$. If we have multiple masses connected to multiple springs,
however, then the oscillations of each mass are not independent. Instead, we will use linear algebra in this assignment to determine the
resonant frequencies of coupled oscillations.  


Vibrations of atoms in molecules are a prime example of a mechanical system that involves coupled oscillations. 
We can assume that the displacements from equilibrium are small, such that the oscillations can still be modeled as that of a simple
harmonic oscillator. Consider a triatomic molecule with a right triangular structure, as shown in the figure below.
The characteristic (resonant) frequencies of its molecular vibrations are closely related to the eigenvalues $\lambda_i$ of the following matrix:

$$\begin{pmatrix}
1 & -1 & 0 & 0 & 0 & 0\\
-1 & 1.5 & -0.5 & 0 & -0.5 & 0.5\\
0 & -0.5 & 0.5 & 0 & 0.5 & -0.5\\
0 & 0 & 0 & 1 & 0 & -1\\
0 & -0.5 & 0.5 & 0 & 0.5 & -0.5\\
0 & 0.5 & -0.5 & -1 & -0.5 & 1.5
\end{pmatrix}
$$


(a) Use the function 'numpy.linalg.eigvals()' to find the eigenvalues of the above matrix.  

(b) What are the corresponding eigenfrequencies of oscillation for this right triangular molecule 
(expressed in terms of the constants $k$ and $m$)? How many unique, nonzero eigenfrequencies does the 
system have? Speculate about what you think eigenfrequencies of zero might mean for this system.

