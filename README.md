# Physics-Simulations
Functions that simulate or calculate physics phenomena and specialised mathematical models.

Function written by Eleni Christoforidou in MATLAB R2022b.

## triangle_wave:

The function computes the sum shown in the attached image, for each of 1001 values of t uniformly spaced from 0 to 4pi inclusive. The input argument is a scalar non-negative integer n, and the output argument is a row vector of 1001 such sums (one sum for each value of t).

![formula](https://github.com/eleni-chr/Physics-Simulations/blob/master/formula_triangle_wave.png)

## spherical_mirror_aberr:

The light striking a vertical plane at a distance f from a mirror is spread over a circular disk. The light from the centre of the mirror strikes the centre of the disk, but light arriving from a point a distance x from the centre of the mirror strikes the plane on a circle with diameter d. The function calculates d for all values of x, then it calculates the mean blur diameter.

![figure](https://github.com/eleni-chr/Physics-Simulations/blob/master/Figure.png)

![formula](https://github.com/eleni-chr/Physics-Simulations/blob/master/Formula.png)

## cyclotron:

The function returns the energy of a positively charged isotope of hydrogen when it escapes a particle accelerator, and the number of times the isotope enters two vacuum chambers, after a voltage is applied to it. The input argument (must be a scalar) is the voltage applied to a cyclotron (see attached figure), which is a device that accelerates subatomic particles (positively charged isotopes of hydrogen, called “deuterons”) which spiral outward in a clockwise direction. The cyclotron rapidly alternates the sign of the voltage difference V in units of volts between two “D”-shaped vacuum chambers (blue outlines in the figure), which are placed within a strong uniform magnetic field (not shown but perpendicular to the screen). The deuteron is accelerated only as it is leaving one “D” and entering the other. While the deuteron is inside a given “D”, it moves at a constant speed, and the magnetic field causes it to move on a semicircle. Each deuteron moves as follows (check the numbers in the figure): (1) It originates from a source (red dot) located at a distance 𝑠𝑠0 to the left of the center of the cyclotron, is accelerated vertically into the upper “D” and then moves on a semi-circle of radius r1. (2) It leaves the upper “D” and is accelerated vertically downward into the lower “D” where it moves with a larger radius r2. (3) It leaves the lower “D” and is accelerated vertically into the upper “D”, etc, moving with ever increasing radii until (N) it is accelerated for the final time as it leaves the upper “D” and enters the lower “D”, follows a semicircle, and emerges from the cyclotron at the left. The deuteron escapes through a window at the left that is placed so the particle cannot leave until it is more than 0.500 meters to the left of the center of the cyclotron. The gap between the “D”s is exaggerated in the figure, has no effect, and can be assumed to be of zero width. The function returns the energy E of the deuteron when it escapes in units of million electron volts (MeV), and the number N of times the deuteron enters the “D”s. Notice that the centres of the semicircles ≠ the center of the cyclotron.

![cyclotron](https://github.com/eleni-chr/Physics-Simulations/blob/master/cyclotron.png)

## voltage:

This function computes the voltages at junctions A, B and C of a basic electrical circuit with 8 resistors (see figure below). The function has two inputs, V for the voltage of the supply in volts and R, a vector of the values of the resistors in ohm. R1 in the figure is R(1), that is, the first element of the vector R. The output of the function is a three-element column vector with the voltage levels at junctions A, B and C, respectively. To compute the voltage levels, the function uses Kirchhoff's current law that states that the sum of current flowing in and out of a junction must be zero. The current across a resistor is the voltage difference divided by the resistance.

![circuit diagram](https://github.com/eleni-chr/Physics-Simulations/blob/master/circuit.png)

## pendulum:

The function calculates the period T of a simple pendulum, which is the time required for a weight attached to a rod of length L and negligible weight to start from rest, swing with no friction under the influence of gravity from an initial angle a0, to –a0 and back to a0 again, as shown in the attached figure. The motion is determined by physics.

![pendulum](https://github.com/eleni-chr/Physics-Simulations/blob/master/pendulum.png)
