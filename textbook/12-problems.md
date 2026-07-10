## Chapter 12 Problems

> [!abstract] Vault Links
> **Concept Hub:** [[Chapter 12 - Coupled Oscillations and Normal Modes]] | **Textbook Index:** [[Textbook Ch 12 - Coupled Oscillations and Normal Modes]] | [[Brain-Map|🧠 Brain Map]]

### Original Transcribed Notes

**12-1.** Reconsider the problem of two coupled oscillators discussed in Section 12.2 in the event that the three springs all have different force constants. Find the two characteristic frequencies, and compare the magnitudes with the natural frequencies of the two oscillators in the absence of coupling.

**12-2.** Continue Problem 12-1, and investigate the case of weak coupling: $\kappa_{12} \ll \kappa_1, \kappa_2$. Show that the phenomenon of beats occurs but that the energy-transfer process is incomplete.

**12-3.** Two identical harmonic oscillators (with masses $M$ and natural frequencies $\omega_0$) are coupled such that by adding to the system a mass $m$ common to both oscillators, the equations of motion become:

$$\ddot{x}_1 + \frac{m}{M} \ddot{x}_2 + \omega_0^2 x_1 = 0$$
$$\ddot{x}_2 + \frac{m}{M} \ddot{x}_1 + \omega_0^2 x_2 = 0$$

Solve this pair of coupled equations, and obtain the frequencies of the normal modes of the system.

**12-4.** Refer to the problem of the two coupled oscillators discussed in Section 12.2. Show that the total energy of the system is constant. (Calculate the kinetic energy of each of the particles and the potential energy stored in each of the three springs, and sum the results.) Notice that the kinetic and potential energy terms that have $\kappa_{12}$ as a coefficient depend on $C_1$ and $\eta_1$ but not on $C_2$ or $\eta_2$. Why is such a result to be expected?

**12-5.** Find the normal coordinates for the problem discussed in Section 12.2 and in Example 12.1 if the two masses are different, $m_1 \neq m_2$. You may again assume all the $\kappa$ are equal.

**12-6.** Two identical harmonic oscillators are placed such that the two masses slide against one another, as in Figure 12-A. The frictional force provides a coupling of the motions proportional to the instantaneous relative velocity. Discuss the coupled oscillations of the system.

![Figure 12-A](file:///c:/Users/Mester/Desktop/semester%204/AM%20II/exam/textbook/M-Chapter-12/41.png)
**Figure 12-A Context:** Two identical harmonic oscillators with friction-based coupling.

**12-7.** A particle of mass $m$ is attached to a rigid support by a spring with force constant $\kappa$. At equilibrium, the spring hangs vertically downward. To this mass-spring combination is attached an identical oscillator, the spring of the latter being connected to the mass of the former. Calculate the characteristic frequencies for one-dimensional vertical oscillations, and compare with the frequencies when one or the other of the particles is held fixed while the other oscillates. Describe the normal modes of motion for the system.

**12-8.** A simple pendulum consists of a bob of mass $m$ suspended by an inextensible (and massless) string of length $l$. From the bob of this pendulum is suspended a second, identical pendulum. Consider the case of small oscillations (so that $\sin \theta \approx \theta$), and calculate the characteristic frequencies. Describe also the normal modes of the system (refer to Problem 7-7).

**12-9.** The motion of a pair of coupled oscillators may be described by using a method similar to that used in constructing a phase diagram for a single oscillator (Section 3.4). For coupled oscillators, the two positions $x_1(t)$ and $x_2(t)$ may be represented by a point (the system point) in the two-dimensional configuration space $x_1 - x_2$. As $t$ increases, the locus of all such points defines a certain curve. The loci of the projection of the system points onto the $x_1$- and $x_2$-axes represent the motions of $m_1$ and $m_2$, respectively. In the general case, $x_1(t)$ and $x_2(t)$ are complicated functions, and so the curve is also complicated. But it is always possible to rotate the $x_1 - x_2$ axes to a new set $\eta_1 - \eta_2$ in such a way that the projection of the system point onto each of the new axes is simple harmonic. The projected motions along the new axes take place with the characteristic frequencies and correspond to the normal modes of the system. The new axes are called normal axes. Find the normal axes for the problem discussed in Section 12.2 and verify the preceding statements regarding the motion relative to this coordinate system.

**12-10.** Consider two identical, coupled oscillators (as in Figure 12-1). Let each of the oscillators be damped, and let each have the same damping parameter $\beta$. A force $F_0 \cos \omega t$ is applied to $m_1$. Write down the pair of coupled differential equations that describe the motion. Obtain the solution by expressing the differential equations in terms of the normal coordinates given by Equation 12.11 and by comparing these equations with Equation 3.53. Show that the normal coordinates $\eta_1$ and $\eta_2$ exhibit resonance peaks at the characteristic frequencies $\omega_1$ and $\omega_2$, respectively.

**12-11.** Consider the electrical circuit in Figure 12-B. Use the developments in Section 12.2 to find the characteristic frequencies in terms of the capacitance $C$, inductance $L$, and mutual inductance $M$. The Kirchhoff circuit equations are:

$$L \ddot{q}_1 + \frac{q_1}{C} + M \ddot{q}_2 = 0$$
$$L \ddot{q}_2 + \frac{q_2}{C} + M \ddot{q}_1 = 0$$

![Figure 12-B](file:///c:/Users/Mester/Desktop/semester%204/AM%20II/exam/textbook/M-Chapter-12/42.png)
**Figure 12-B Context:** Electrical circuit consisting of two inductively coupled loops.

**12-12.** Show that the equations in Problem 12-11 can be put into the same form as Equation 12.1 by solving the second equation above for $\ddot{q}_2$ and substituting the result into the first equation. Similarly, substitute for $\ddot{q}_1$ in the second equation. The characteristic frequencies may then be written down immediately in analogy with Equation 12.8.

**12-13.** Find the characteristic frequencies of the coupled circuits of Figure 12-C.

![Figure 12-C](file:///c:/Users/Mester/Desktop/semester%204/AM%20II/exam/textbook/M-Chapter-12/42.png#page=2)
**Figure 12-C Context:** Coupled electrical circuits with capacitors and inductors.

**12-14.** Discuss the normal modes of the system shown in Figure 12-D.

![Figure 12-D](file:///c:/Users/Mester/Desktop/semester%204/AM%20II/exam/textbook/M-Chapter-12/42.png#page=3)
**Figure 12-D Context:** Coupled mechanical systems representing modes of oscillation.

**12-15.** In Figure 12-C, replace $L_{12}$ by a resistor and analyze the oscillations.

**12-16.** A thin hoop of radius $R$ and mass $M$ oscillates in its own plane hanging from a single fixed point. Attached to the hoop is a small mass $m$ constrained to move (in a frictionless manner) along the hoop. Consider only small oscillations, and show that the eigenfrequencies are:

$$\omega_1 = \sqrt{\frac{g}{2R}}$$
$$\omega_2 = \sqrt{\frac{g}{R} \left(1 + \frac{m}{M}\right)}$$

Find the two sets of initial conditions that allow the system to oscillate in its normal modes. Describe the physical situation for each mode.

**12-17.** Find the eigenfrequencies and describe the normal modes for a system such as the one discussed in Section 12.2 but with three equal masses $m$ and four springs (all with equal force constants $\kappa$) with the system fixed at the ends.

**12-18.** A mass $M$ moves horizontally along a smooth rail. A pendulum is hung from $M$ with a weightless rod of length $l$ and mass $m$ at its end. Find the eigenfrequencies and describe the normal modes.

**12-19.** In the problem of the three coupled pendula, consider the three coupling constants as distinct, so that the potential energy may be written as:

$$U = \frac{1}{2} \left[ \theta_1^2 + \theta_2^2 + \theta_3^2 + \epsilon_{12}(\theta_1 - \theta_2)^2 + \epsilon_{13}(\theta_1 - \theta_3)^2 + \epsilon_{23}(\theta_2 - \theta_3)^2 \right]$$

with $\epsilon_{12}, \epsilon_{13}, \epsilon_{23}$ all different. Show that no degeneracy occurs in such a system. Show also that degeneracy can occur only if $\epsilon_{12} = \epsilon_{13} = \epsilon_{23}$.

**12-20.** Construct the possible eigenvectors for the degenerate modes in the case of the three coupled pendula by requiring $a_{12} = 2a_{11}$. Interpret this situation physically.

**12-21.** Three oscillators of equal mass $m$ are coupled such that the potential energy of the system is given by:

$$U = \frac{1}{2} \left[ \kappa (x_1^2 + x_2^2 + x_3^2) + \kappa_0 (x_1 x_2 + x_2 x_3) \right]$$

where $\kappa_0 = \sqrt{2}\kappa$. Find the eigenfrequencies by solving the secular equation. What is the physical interpretation of the zero-frequency mode?

**12-22.** Consider a thin homogeneous plate of mass $M$ that lies in the $x_1 - x_2$ plane with its center at the origin. Let the length of the plate be $2A$ (in the $x_1$-direction) and let the width be $2B$ (in the $x_2$-direction). The plate is suspended from a fixed support by four springs of equal force constant $\kappa$ at the four corners of the plate. The plate is free to oscillate but with the constraint that its center must remain on the $x_3$-axis. Thus, we have three degrees of freedom: (1) vertical motion, with the center of the plate moving along the $x_3$-axis; (2) a tipping motion lengthwise, with the $x_2$-axis serving as an axis of rotation (choose an angle $\theta$ to describe this motion); and (3) a tipping motion sidewise, with the $x_1$-axis serving as an axis of rotation (choose an angle $\phi$ to describe this motion). Assume only small oscillations and show that the secular equation has a double root, and hence that the system is degenerate. Discuss the normal modes of the system. (In evaluating the $a_{jr}$ for the degenerate modes, arbitrarily set one of the $a_{jr}$ equal to zero to remove the indeterminacy.)

**12-23.** Show that the degeneracy can be removed by adding to the plate a thin bar of mass $m$ and length $2A$ situated (at equilibrium) along the $x_1$-axis. Find the new eigenfrequencies for the system.

**12-24.** Evaluate the total energy associated with a normal mode, and show that it is constant in time. Show this explicitly for the case of Example 12.3.

**12-25.** Show that the equations of motion for longitudinal vibrations of a loaded string are of exactly the same form as the equations for transverse motion (Equation 12.131), except that the factor $\tau/d$ must be replaced by $\kappa$, the force constant of the string.

**12-26.** Rework the problem in Example 12.7, assuming that all three particles are displaced a distance $a$ and released from rest.

**12-27.** Consider three identical pendula instead of the two shown in Figure 12-5 with a spring of constant $0.20\text{ N/m}$ between the center pendulum and each of the side ones. The mass bobs are $250\text{ g}$, and the pendula lengths are $47\text{ cm}$. Find the normal frequencies.

**12-28.** Consider the case of a double pendulum shown in Figure 12-E where the top pendulum has length $L_1$ and the bottom length is $L_2$, and similarly, the bob masses are $m_1$ and $m_2$. The motion is only in the plane. Find and describe the normal modes and coordinates. Assume small oscillations.

![Figure 12-E](file:///c:/Users/Mester/Desktop/semester%204/AM%20II/exam/textbook/M-Chapter-12/44.png)
**Figure 12-E Context:** Problem 12-28. Double pendulum geometry.

**12-29.** Find the normal modes for the coupled pendulums in Figure 12-5 when the pendulum on the left has mass bob $m_1 = 300\text{ g}$ and the right has mass bob $m_2 = 500\text{ g}$. The length of both pendula is $40\text{ cm}$, and the spring constant is $0.020\text{ N/m}$. When the left pendulum is initially pulled back to $\theta_1 = -7^\circ$ and released from rest when $\theta_2 = \dot{\theta}_1 = \dot{\theta}_2 = 0$, what is the maximum angle that $\theta_2$ reaches? Use the small angle approximation.
