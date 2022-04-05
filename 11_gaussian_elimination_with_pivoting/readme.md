## Gaussian elimination with pivoting:


(a) Consider the following system of linear equations, written in the matrix form
$$\textbf{A x = v}:$$

$$
\begin{pmatrix}
0 & 1 & 4 & 1\\
3 & 4 & -1 & -1\\
1 & -4 & 1 & 5\\
2 & -2 & 1 & 3
\end{pmatrix}
\begin{pmatrix}
w \\ x \\ y \\ z  
\end{pmatrix} =
\begin{pmatrix}
-4 \\ 3 \\ 9 \\ 7
\end{pmatrix}
$$

Solve this matrix equation for the unknown variables using Gaussian elimination with pivoting. 
You may start by using the Gaussian elimination algorithm from class (or the 'gausselim.py' script from Newman) and modify it to include
pivoting.  

(b) Compare your answer with the results you obtain using the 'numpy.linalg.solve()' function instead of your own algorithm.
