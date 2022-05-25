## The Power of a Quasar
Supermassive black holes, with masses of $\approx 10^6 − 10^{10}$ times the mass of the Sun , are
found at the centers of nearly all galaxies. Most of the time they lurk quietly, but if there is
a supply of gas nearby, they will start consuming it. Despite their “supermassive" status,
these black holes are miniscule in size compared to the galaxies they live in. This means
that gas falling toward the black hole has to lose a huge amount of orbital energy and
angular momentum before it actually reaches the black hole’s event horizon.
This process releases vast amounts of energy, much of it in the form of electromagnetic
(EM) radiation, and these extremely luminous objects are called quasars. Quasars emit
radiation across the entire EM spectrum, from radio waves to gamma rays. Telescopes
that use a technique called spectroscopy can determine not only how much total radiation
is emitted by the quasar per unit time, but also how much radiation is emitted in each
portion of the spectrum. You are going to analyze a quasar spectrum and determine the
power of the quasar’s radiation. When the energy we’re considering is from EM radiation,
we call it the luminosity. Recall that power (and thus luminosity) has units of [energy /
time], and that the SI unit of power is Watts [W].
Your assignment is to write a code that can read in a quasar spectrum and calculate
either the total luminosity emitted across all frequencies, or alternatively the luminosity
emitted at a specific range of frequencies. 

The input data you will use is in a file called quasar_spectrum.txt. 
This is an average quasar spectrum derived from analysis of hundreds of individual quasars.
From Richards et al. (2006): https://iopscience.iop.org/article/10.1086/506525


The input file quasar_spectrum.txt has two columns:
• Column 1 contains the (base 10) log of the frequency of each data point in the
spectrum: $log_{10}$(ν) (units: $log_{10}$ Hz)
• Column 2 contains the quasar luminosity at each frequency, expressed in terms of
the following quantity (which has units of $log_{10} W$):
$log_{10} \bigg(ν \frac{dL}{dν}\bigg)

To obtain the total luminosity, you should perform the following integral:
$L_{tot} = \int^{log_{10}(ν_{max})}_{log_{10}(ν_{min})} \bigg(ν \frac{dL}{dν}\bigg) ln(10) dlog_{10}(ν)$

(This uses $log_{10}(ν)$ as the independent variable, making use of the fact that
$ln(ν) = ln(10) log_{10}(ν).$ )

Here are the details of what your submitted homework should include:
1. Write code that can read in the data in quasar_spectrum.txt and assign the
data to appropriate variables. Make a plot of the quasar spectrum.

2. Write code to calculate the luminosity in a specified portion of the quasar spectrum,
by performing numerical integration. Your code should be able to use any of the
following integration methods:
(a) Piecewise constant integration (the “rectangle rule")
(b) Piecewise linear integration (the “trapezoidal rule")
(c) Simpson’s Rule

3. For each of these integration methods, have your code perform the integration over
the entire spectrum to calculate the total luminosity, and print the results. You should
also calculate the relative error for each method, given that the true total luminosity
of the quasar is Ltot,exact = 2.195102 ×1039 W.

4. Compare the total luminosity of the quasar to the luminosity of the Sun. How many
stars with the Sun’s luminosity would a galaxy need for its total stellar luminosity to
equal the quasar’s luminosity? How does this compare to the approximate number
of stars in the Milky Way galaxy?

5. Finally, choose one of these integration methods and calculate the luminosity in only
the visible portion of the spectrum (wavelength range λ = 400 −700 nm). What frac-
tion of the quasar’s total luminosity is emitted in the visible portion of the spectrum?
