# Chapter 9: Dynamics of a System of Particles

## 1. Linear Momentum of a System

**Original Notes Transcription:**
> $\vec{p}_i = m_i \vec{v}_i = m_i \dot{\vec{r}}_i$
> $\vec{P} = \sum_i m_i \dot{\vec{r}}_i = \left(\sum_i m_i \vec{r}_i\right)^{\cdot}$
> $= M \times \frac{1}{M} \frac{d}{dt} \left( \sum_i m_i \vec{r}_i \right) = M \frac{d}{dt} \left( \frac{1}{M} \sum_i m_i \vec{r}_i \right)$
> $\vec{R}_{CM} = \frac{1}{M} \sum_i m_i \vec{r}_i$
> $\vec{V}_{CM} = \frac{d}{dt} \vec{R}_{CM}$
> $\vec{P} = M \vec{V}_{CM}$

> **Elaboration:**
> The total linear momentum of a system of particles ($\vec{P}$) is the vector sum of the individual momenta ($\vec{p}_i$) of all particles in the system. 
> By factoring out the total mass $M$, we naturally derive the definition of the **Center of Mass (CM)**, denoted as $\vec{R}_{CM}$. 
> The beauty of this formulation is that the total momentum of a complex system of many interacting particles can be simply expressed as the total mass of the system multiplied by the velocity of its center of mass ($\vec{P} = M \vec{V}_{CM}$). This allows us to treat macroscopic objects as if all their mass is concentrated at a single point (the CM).

### Newton's Second Law for a System

**Original Notes Transcription:**
> For a single particle: $\vec{F} = m\vec{a} \rightarrow \vec{F} = \frac{d\vec{p}}{dt}$
> For the system: $\vec{P}_{tot} = \sum_i \vec{p}_i \rightsquigarrow \frac{d\vec{P}}{dt} = \sum_i \frac{d\vec{p}_i}{dt} = \sum_i \vec{F}_i$
> $\frac{d\vec{P}}{dt} = \sum_i \vec{F}_i^{int} + \sum_i \vec{F}_i^{ext} = \sum_i \sum_{j \neq i} \vec{F}_{ij} + \sum_i \vec{F}_i^{ext}$
> $\vec{F}_{12} + \vec{F}_{21} + \vec{F}_{13} + \vec{F}_{31} + \dots = 0 + \vec{F}_{tot}^{ext}$
> $\rightarrow \frac{d\vec{P}}{dt} = \vec{F}^{ext}$
> 
> *Notes:* 
> 1) Newton's second law for a system of particles. 
> 2 & 3) Newton's third law.

> **Elaboration:**
> When we sum the forces acting on all particles in a system, the forces can be categorized into **internal forces** ($\vec{F}^{int}$) and **external forces** ($\vec{F}^{ext}$). 
> According to **Newton's Third Law** (action and reaction), the internal force exerted by particle $j$ on particle $i$ ($\vec{F}_{ij}$) is equal and opposite to the force exerted by $i$ on $j$ ($\vec{F}_{ji}$). Therefore, when summing over all particles, all internal forces perfectly cancel each other out ($\sum \vec{F}_{ij} = 0$). 
> This leaves us with a profound result: **Only external forces can change the total momentum of a system.** The center of mass accelerates as if all external forces were applied directly to it: $\vec{F}^{ext} = M\vec{A}_{CM}$.

### Conservation of Linear Momentum

**Original Notes Transcription:**
> If $\vec{F}^{ext} = 0 \rightarrow \frac{d\vec{P}}{dt} = 0 \rightarrow \vec{P} = \text{const}$
> If $\vec{F}^{ext} \cdot \hat{n} = 0 \rightarrow \frac{d}{dt}(\vec{P} \cdot \hat{n}) = 0 \Rightarrow \vec{P} \cdot \hat{n} = \text{const}$
> *(We saw this previously in the Lagrangian chapter.)*

> **Elaboration:**
> - **Total Conservation:** If the net external force on a system is zero, the total linear momentum is strictly conserved.
> - **Directional Conservation:** Even if there is a net external force, if the force has no component in a specific direction $\hat{n}$ (i.e., the dot product $\vec{F}^{ext} \cdot \hat{n} = 0$), then the momentum along that specific direction is conserved. This is an application of Noether's Theorem, which links continuous translational symmetries to momentum conservation, a concept heavily utilized in Lagrangian mechanics.

---

## 2. Example Problem: The Falling Rope

**Problem Statement:**
> A rope of length $b$ is attached from both ends to the ceiling. At one instant, we cut the connection of one side.

**Original Notes Transcription:**
> Let $x$ be the distance the free end has fallen.
> Left (fixed) part length: $\frac{b+x}{2}$
> Right (falling) part length: $\frac{b-x}{2}$
> Mass density: $\rho = \frac{M}{b}$
> General Force Equation: $Mg - T = \dot{P}$
> 
> (I) $T(x) = Mg - \dot{P}(x)$
> (II) $P(x) = P_I + P_{II}$
> $P_I = 0$ (fixed side)
> $P_{II} = m_{II} \times v_{II} = \rho \left(\frac{b-x}{2}\right) \times \dot{x}$
> $\dot{P} = \frac{d}{dt} \left[ \rho \left(\frac{b-x}{2}\right) \dot{x} \right] = \frac{\rho}{2} \left[ -\dot{x}^2 + \ddot{x}(b-x) \right]$

> **Elaboration:**
> This is a classic variable-mass system problem. The system's total momentum changes because mass is constantly transferring from the falling side (moving at velocity $\dot{x}$) to the fixed side (velocity $0$) at the bottom bend. We apply the generalized Newton's second law ($\vec{F} = \dot{\vec{P}}$) to the entire rope. The external forces are gravity ($Mg$) downwards and the tension ($T$) from the ceiling upwards.

### Proposal 1: Free Fall Assumption

**Original Notes Transcription:**
> Assume the falling side is in free fall: $\ddot{x} = g$, $\dot{x} = \sqrt{2gx}$
> $\rightsquigarrow T = \frac{Mg}{2} \left(\frac{3x}{b} + 1\right)$
> When fully fallen ($x=b$): $T(x=b) = 2Mg$
> *We do not have conservation of energy here ($\Delta E \neq 0$).*

> **Elaboration:**
> If we assume the right side is simply in free fall, we can calculate the required tension at the ceiling. Interestingly, when the rope is fully extended ($x=b$), the tension is $2Mg$, not $1Mg$. This is because the ceiling must support both the weight of the rope AND provide the impulse to abruptly stop the falling links of the rope at the bottom bend.
> **Why is energy not conserved?** In this model, as each link of the rope hits the bend, its velocity goes from $\dot{x}$ to $0$ instantly. This is a completely inelastic macroscopic collision, meaning kinetic energy is dissipated as heat or internal deformation within the rope.

### Proposal 2: Continuous Rope & Energy Conservation Assumption

**Original Notes Transcription:**
> In the case of assuming a continuous rope, what equation should we use? Conservation of Energy.
> $U = 0$ at the ceiling.
> (I) Kinetic Energy: $K = \frac{1}{2} \left( \rho \frac{b-x}{2} \right) \dot{x}^2$
> (II) Potential Energy: $U(x) = U_L + U_R = -\rho g \left( \frac{b+x}{2} \right)\left( \frac{b+x}{4} \right) - \rho g \left( \frac{b-x}{2} \right)\left( x + \frac{b-x}{4} \right)$
> $\rightsquigarrow U(x) = -\frac{1}{4} \rho g (b^2 + 2bx - x^2)$
> Conservation: $K(x) + U(x) = K_0 + U_0$
> $\frac{\rho}{4}(b-x)\dot{x}^2 - \frac{1}{4} \rho g (b^2 + 2bx - x^2) = 0 - \frac{g \rho b^2}{4}$

> **Elaboration:**
> Alternatively, if we assume an idealized, perfectly elastic, continuous "fluid-like" rope where no energy is lost at the bend, we can use conservation of mechanical energy. 
> - **Potential Energy Calculation:** The center of mass (CM) of the left side is located halfway down its length, at depth $(b+x)/4$. The right side's CM is halfway down its falling portion, at depth $x + (b-x)/4$. By calculating the PE for both sides, we get the total $U(x)$.
> - **Initial State:** At $t=0$, $x=0$, $K_0 = 0$, and $U_0 = -\frac{1}{4}\rho g b^2$.

**Original Notes Transcription:**
> Solving for $\dot{x}^2$ and taking the time derivative $2\dot{x}\ddot{x} = (\dots)^{\cdot}$ to find $\ddot{x}$:
> $\rightarrow \dot{x}^2 = \frac{g(2bx - x^2)}{b-x}$
> $\rightarrow \ddot{x} = g + \frac{g(2bx - x^2)}{2(b-x)^2}$
> Substituting back into $T$:
> $\rightarrow T = \frac{Mg}{4b} \frac{1}{b-x} (2b^2 + 2bx - 3x^2)$
> *Substituting, with numerical solving in the first stage, is up to you.*

> **Elaboration:**
> By setting $K+U = U_0$, we isolate the squared velocity $\dot{x}^2$. Differentiating this expression implicitly with respect to time yields the acceleration $\ddot{x}$. Notice that $\ddot{x} > g$, meaning the rope actually falls *faster* than free fall in this idealized energy-conserving model. This happens because the energy that would have been lost as heat in the inelastic model is instead doing work to "pull" the rest of the rope down. Finally, substituting $\dot{x}$ and $\ddot{x}$ back into our momentum equation $T = Mg - \dot{P}$ gives us the dynamic tension.

---

## 3. Angular Momentum

**Original Notes Transcription:**
> $\vec{L} = \sum_\alpha \vec{r}_\alpha \times \vec{p}_\alpha$
> *(Diagram shows an origin, the center of mass $m_N$, and individual particles $m_1, m_i$ with position vectors $\vec{r}_i$ and momentum $\vec{p}_i$)*

> **Elaboration:**
> The total angular momentum $\vec{L}$ of a system of particles about a chosen origin is the vector sum of the individual angular momenta of all the particles ($\vec{r} \times \vec{p}$). Just like linear momentum, angular momentum for a system can be elegantly split into two parts: the angular momentum of the Center of Mass relative to the origin, and the angular momentum of the particles relative to the Center of Mass (spin).
