## Interpolation of a quasar spectrum

(a) Write a program that can perform interpolation of a data set using either
- your own linear interpolation algorithm, or
- a pre-existing cubic spline interpolation algorithm (using e.g. the interp1d
function from scipy.interpolate, with the ‘cubic’ keyword)

(b) Use each of these methods (linear and cubic spline interpolation) in turn to in-
terpolate the data from the file quasar_spectrum.txt.

(c) (c) For each interpolated data set, use previously created trapezoidal integration routine to 
calculate the total luminosity of the quasar. Compare both results to results from trapezoidal routine, 
as well as the exact answer $(L_{tot,exact} = 2.195102 ×10^{39} W)$.
