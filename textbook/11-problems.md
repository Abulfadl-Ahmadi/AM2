## Chapter 11 Problems

> [!abstract] Vault Links
> **Concept Hub:** [[Chapter 11 - Dynamics of Rigid Bodies]] | **Textbook Index:** [[Textbook Ch 11 - Dynamics of Rigid Bodies]] | [[Brain-Map|🧠 Brain Map]]

### Original Transcribed Notes

**11-1.** Calculate the moments of inertia $I_1$, $I_2$, and $I_3$ for a homogeneous sphere of radius $R$ and mass $M$. (Choose the origin at the center of the sphere.)

**11-2.** Calculate the moments of inertia $I_1$, $I_2$, and $I_3$ for a homogeneous cone of mass $M$ whose height is $h$ and whose base has a radius $R$. Choose the $x_3$-axis along the axis of symmetry of the cone. Choose the origin at the apex of the cone, and calculate the elements of the inertia tensor. Then make a transformation such that the center of mass of the cone becomes the origin, and find the principal moments of inertia.

**11-3.** Calculate the moments of inertia $I_1$, $I_2$, and $I_3$ for a homogeneous ellipsoid of mass $M$ with axes' lengths $2a > 2b > 2c$.

**11-4.** Consider a thin rod of length $l$ and mass $m$ pivoted about one end. Calculate the moment of inertia. Find the point at which, if all the mass were concentrated, the moment of inertia about the pivot axis would be the same as the real moment of inertia. The distance from this point to the pivot is called the radius of gyration.

**11-5.** (a) Find the height at which a billiard ball should be struck so that it will roll with no initial slipping. (b) Calculate the optimum height of the rail of a billiard table. On what basis is the calculation predicated?

**11-6.** Two spheres are of the same diameter and same mass, but one is solid and the other is a hollow shell. Describe in detail a nondestructive experiment to determine which is solid and which is hollow.

**11-7.** A homogeneous disk of radius $R$ and mass $M$ rolls without slipping on a horizontal surface and is attracted to a point a distance $d$ below the plane. If the force of attraction is proportional to the distance from the disk's center of mass to the force center, find the frequency of oscillations around the position of equilibrium.

**11-8.** A door is constructed of a thin homogeneous slab of material; it has a width of $1\text{ m}$. If the door is opened through $90^\circ$, it is found that on release it closes itself in $2\text{ s}$. Assume that the hinges are frictionless, and show that the line of hinges must make an angle of approximately $3^\circ$ with the vertical.

**11-9.** A homogeneous slab of thickness $a$ is placed atop a fixed cylinder of radius $R$ whose axis is horizontal. Show that the condition for stable equilibrium of the slab, assuming no slipping, is $R > a/2$. What is the frequency of small oscillations? Sketch the potential energy $U$ as a function of the angular displacement $\theta$. Show that there is a minimum at $\theta = 0$ for $R > a/2$ but not for $R \le a/2$.

**11-10.** A solid sphere of mass $M$ and radius $R$ rotates freely in space with an angular velocity $\omega$ about a fixed diameter. A particle of mass $m$, initially at one pole, moves with a constant velocity $v$ along a great circle of the sphere. Show that, when the particle has reached the other pole, the rotation of the sphere will have been retarded by an angle:

$$\Delta \theta = \omega T \left( 1 - \sqrt{\frac{2M}{2M + 5m}} \right)$$

where $T$ is the total time required for the particle to move from one pole to the other.

**11-11.** A homogeneous cube, each edge of which has a length $b$, is initially in a position of unstable equilibrium with one edge in contact with a horizontal plane. The cube is then given a small displacement and allowed to fall. Show that the angular velocity of the cube when one face strikes the plane is given by:

$$\omega^2 = A \frac{g}{b} (\sqrt{2} - 1)$$

where $A = 3/2$ if the edge cannot slide on the plane, and where $A = 12/5$ if sliding can occur without friction.

**11-12.** Show that none of the principal moments of inertia can exceed the sum of the other two.

**11-13.** A three-particle system consists of masses $m_i$ and coordinates $(x_{i1}, x_{i2}, x_{i3})$ as follows:
- $m_1 = 3m$, $(b, 0, b)$
- $m_2 = 4m$, $(b, b, -b)$
- $m_3 = 2m$, $(-b, b, 0)$

Find the inertia tensor, principal axes, and principal moments of inertia.

**11-14.** Determine the principal axes and principal moments of inertia of a uniform solid hemisphere of radius $b$ and mass $m$ about its center of mass.

**11-15.** If a physical pendulum has the same period of oscillation when pivoted about either of two points of unequal distances from the center of mass, show that the length of the simple pendulum with the same period is equal to the sum of separations of the pivot points from the center of mass. Such a physical pendulum, called Kater's reversible pendulum, at one time provided the most accurate way (to about 1 part in $10^5$) to measure the acceleration of gravity. Discuss the advantages of Kater's pendulum over a simple pendulum for such a purpose.

**11-16.** Consider the following inertia tensor:

$$\{\mathbf{I}\} = \begin{pmatrix} A & -B & 0 \\ -B & A & 0 \\ 0 & 0 & C \end{pmatrix}$$

Perform a rotation of the coordinate system by an angle $\theta$ about the $x_3$-axis. Evaluate the transformed tensor elements, and show that the choice $\theta = \pi/4$ renders the inertia tensor diagonal with elements $A+B$, $A-B$, and $C$.

**11-17.** Consider a thin homogeneous plate that lies in the $x_1 - x_2$ plane. Show that the inertia tensor takes the form:

$$\{\mathbf{I}\} = \begin{pmatrix} A & -C & 0 \\ -C & B & 0 \\ 0 & 0 & A+B \end{pmatrix}$$

**11-18.** If, in the previous problem, the coordinate axes are rotated through an angle $\theta$ about the $x_3$-axis, show that the new inertia tensor is:

$$\{\mathbf{I}\} = \begin{pmatrix} A' & -C' & 0 \\ -C' & B' & 0 \\ 0 & 0 & A'+B' \end{pmatrix}$$

where:

$$A' = A \cos^2 \theta - C \sin 2\theta + B \sin^2 \theta$$
$$B' = A \sin^2 \theta + C \sin 2\theta + B \cos^2 \theta$$
$$C' = C \cos 2\theta - \frac{1}{2} (B - A) \sin 2\theta$$

and hence show that the $x'_1$ and $x'_2$ axes become principal axes if the angle of rotation is:

$$\tan 2\theta = \frac{2C}{B - A}$$

**11-19.** Consider a plane homogeneous plate of density $\rho$ bounded by the logarithmic spiral $r = k e^{a\theta}$ and the radii $\theta = 0$ and $\theta = \pi$. Obtain the inertia tensor for the origin at $r = 0$ if the plate lies in the $x_1 - x_2$ plane. Perform a rotation of the coordinate axes to obtain the principal moments of inertia, and use the results of the previous problem to show that they are:

$$I_1 = \rho K (Q - R), \quad I_2 = \rho K (Q + R), \quad I_3 = I_1 + I_2$$

where:

$$K = \frac{k^4 (e^{4a\pi} - 1)}{16(1 + 4a^2)}$$
$$Q = 1 + 4a^2, \quad R = \sqrt{1 + 16a^2}$$

**11-20.** A uniform rod of length $l$ stands vertically upright on a rough floor and then tips over. What is the rod's angular velocity when it hits the floor?

**11-21.** The proof represented by Equations 11.54–11.61 is expressed entirely in the summation convention. Rewrite this proof in matrix notation.

**11-22.** The trace of a tensor is defined as the sum of the diagonal elements:

$$\text{tr}\{\mathbf{I}\} = \sum_i I_{ii}$$

Show, by performing a similarity transformation, that the trace is an invariant quantity. In other words, show that:

$$\text{tr}\{\mathbf{I}\} = \text{tr}\{\mathbf{I}'\}$$

where $\{\mathbf{I}\}$ is the tensor in one coordinate system and $\{\mathbf{I}'\}$ is the tensor in a coordinate system rotated with respect to the first system. Verify this result for the different forms of the inertia tensor for a cube given in several examples in the text.

**11-23.** Show by the method used in the previous problem that the determinant of the elements of a tensor is an invariant quantity under a similarity transformation. Verify this result also for the case of the cube.

**11-24.** Find the frequency of small oscillations for a thin homogeneous plate if the motion takes place in the plane of the plate and if the plate has the shape of an equilateral triangle and is suspended (a) from the midpoint of one side and (b) from one apex.

**11-25.** Consider a thin disk composed of two homogeneous halves connected along a diameter of the disk. If one half has density $\rho$ and the other has density $2\rho$, find the expression for the Lagrangian when the disk rolls without slipping along a horizontal surface. (The rotation takes place in the plane of the disk.)

**11-26.** Obtain the components of the angular velocity vector $\boldsymbol{\omega}$ (see Equation 11.102) directly from the transformation matrix $\mathbf{A}$ (Equation 11.99).

**11-27.** A symmetric body moves without the influence of forces or torques. Let $x_3$ be the symmetry axis of the body and $\mathbf{L}$ be along $x'_3$. The angle between $\boldsymbol{\omega}$ and $x_3$ is $\alpha$. Let $\boldsymbol{\omega}$ and $\mathbf{L}$ initially be in the $x_2 - x_3$ plane. What is the angular velocity of the symmetry axis about $\mathbf{L}$ in terms of $I_1$, $I_3$, $\omega_3$, and $\alpha$?

**11-28.** Show from Figure 11-9c that the components of $\boldsymbol{\omega}$ along the fixed ($x'_i$) axes are:

$$\begin{aligned}
\omega'_1 &= \dot{\theta} \cos \phi + \dot{\psi} \sin \theta \sin \phi \\
\omega'_2 &= \dot{\theta} \sin \phi - \dot{\psi} \sin \theta \cos \phi \\
\omega'_3 &= \dot{\psi} \cos \theta + \dot{\phi}
\end{aligned}$$

**11-29.** Investigate the motion of the symmetric top discussed in Section 11.11 for the case in which the axis of rotation is vertical (i.e., the $x'_3$- and $x_3$-axes coincide). Show that the motion is either stable or unstable depending on whether the quantity $I_3^2 \omega_3^2 / 4 I_1 Mgh$ is greater than or less than unity. Sketch the effective potential $V(\theta)$ for the two cases, and point out the features of these curves that determine whether the motion is stable. If the top is set spinning in the stable configuration, what is the effect as friction gradually reduces the value of $\omega_3$? (This is the case of the "sleeping top.")

**11-30.** Refer to the discussion of the symmetric top in Section 11.11. Investigate the equation for the turning points of the nutational motion by setting $\dot{\theta} = 0$ in Equation 11.161. Show that the resulting equation is a cubic in $u = \cos \theta$ and has two real roots in the physical region and one root outside the physical region.

**11-31.** Consider a thin homogeneous plate with principal moments of inertia:
- $I_1$ along the principal axis $x_1$
- $I_2 > I_1$ along the principal axis $x_2$
- $I_3 = I_1 + I_2$ along the principal axis $x_3$

Let the origins of the $x'_i$ and $x_i$ systems coincide and be located at the center of mass $O$ of the plate. At time $t = 0$, the plate is set rotating in a force-free manner with an angular velocity $\Omega$ about an axis inclined at an angle $\alpha$ from the plane of the plate and perpendicular to the $x_2$-axis. If $I_1/I_2 = \cos 2\alpha$, show that at time $t$ the angular velocity about the $x_1$-axis is:

$$\omega_1(t) = \Omega \cos \alpha \tanh(\Omega t \sin \alpha)$$

**11-32.** Solve Example 11.2 for the case when the physical pendulum does not undergo small oscillations. The pendulum is released from rest at $\theta_0 = 90^\circ$ at time $t = 0$. Find the angular velocity when the pendulum angle is at $\theta = 0^\circ$. The mass of the pendulum is $340\text{ g}$, the distance $d$ is $13\text{ cm}$, and the radius of gyration $k$ is $17\text{ cm}$.

**11-33.** Do a literature search and explain how a cat can always land on its feet when dropped from a position at rest with its feet pointing upward. Estimate the minimum height a cat needs to fall in order to execute such a maneuver.

**11-34.** Consider a symmetrical rigid body rotating freely about its center of mass. A frictional torque ($N_i = -b_i \omega_i$) acts to slow down the rotation. Find the component of the angular velocity along the symmetry axis as a function of time.
