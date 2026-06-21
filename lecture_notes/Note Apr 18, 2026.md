# Chapter 9: Dynamics of a System of Particles (Continued) - Lecture: Apr 18, 2026

## 1. Course Outline & Introduction (سرفصل‌های درس و مقدمه)

**Original Notes Transcription:**
> **پیش از دستور:** (Outline / Prologue)
> - **دینامیک سیستم ذرات** (Dynamics of a System of Particles) - ۱ هفته (1 week)
> - **حرکت در دستگاه ناخت** (Motion in Non-Inertial Frames) - ۱ هفته (1 week)
> - **دینامیک اجسام صلب** (Dynamics of Rigid Bodies) - ۲.۵ هفته (2.5 weeks)
> - **نوسان‌های جفت‌شده** (Coupled Oscillations) - ۳ هفته (3 weeks)
> - **سیستم پیوسته، موج** (Continuous Systems, Waves) - ۱ هفته (1 week)
>
> Topics for today:
> - **انرژی سیستم ذرات** (Energy of a System of Particles)
> - **برخورد $\rightarrow$ مرکز جرم** (Collisions $\rightarrow$ CM Frame)
>
> **۱) انرژی جنبشی:** (1. Kinetic Energy)
> $$T_{tot} = \frac{1}{2} \sum_\alpha m_\alpha |\vec{v}_\alpha|^2$$
> $$T = \frac{1}{2} \sum_\alpha m_\alpha (\vec{\dot{R}}_{CM} + \vec{\dot{r}}'_\alpha) \cdot (\vec{\dot{R}}_{CM} + \vec{\dot{r}}'_\alpha)$$
> $$= \frac{1}{2} \left(\sum_\alpha m_\alpha\right) |\vec{\dot{R}}_{CM}|^2 + \frac{1}{2} \sum_\alpha m_\alpha |\vec{\dot{r}}'_\alpha|^2 + \left(\sum_\alpha m_\alpha \vec{\dot{r}}'_\alpha\right) \cdot \vec{\dot{R}}_{CM}$$
>
> Using CM frame properties:
> $\vec{v}_\alpha$ (Lab frame) and $\vec{u}_\alpha$ (CM frame):
> $$T = \frac{1}{2} M |\vec{V}_{CM}|^2 + \frac{1}{2} \sum_\alpha m_\alpha |\vec{u}_\alpha|^2$$
>
> Ads:
> $\vec{v}$: Lab frame
> $\vec{u}$: CM frame

> **Elaboration:**
> The lecture began with a roadmap outlining the remaining topics of the classical mechanics course. The immediate focus is completing the study of particle systems (specifically their energy and collisions) before moving on to non-inertial reference frames and rigid body dynamics.
>
> The mathematical derivation of the kinetic energy of a system of particles (König's Theorem) was reviewed. By defining the position of each particle relative to the Center of Mass (CM) frame ($\vec{r}_\alpha = \vec{R}_{CM} + \vec{r}'_\alpha$), the total kinetic energy separates into:
> 1. The translational kinetic energy of the system's total mass $M$ moving with the velocity of the center of mass $\vec{V}_{CM}$.
> 2. The internal kinetic energy of the particles relative to the center of mass (using the CM frame velocities $\vec{u}_\alpha$).
>
> The cross term vanishes because, by definition, the total mass-weighted position (and thus momentum) relative to the center of mass is zero ($\sum_\alpha m_\alpha \vec{r}'_\alpha = 0$).

---

## 2. Two-Body System in the CM Frame (سیستم دو جسمی در دستگاه مرکز جرم)

**Original Notes Transcription:**
> **• مثال:** (Example)
> **یادآوری + تبلیغات:** (Reminder + Promo/Tangent)
> Two frames:
> - **Lab-frame:** masses $m_1$ and $m_2$ with velocities $\vec{v}_1$ and $\vec{v}_2$.
> - **CM-frame:** masses $m_1$ and $m_2$ with velocities $\vec{u}_1$ and $\vec{u}_2$.
>
> In the CM-frame:
> $$m_1 \vec{u}_1 + m_2 \vec{u}_2 = 0 \rightarrow \vec{u}_2 = -\frac{m_1}{m_2} \vec{u}_1$$
> $$T_{CM} = \frac{1}{2} m_1 |\vec{u}_1|^2 + \frac{1}{2} m_2 |\vec{u}_2|^2$$
> $$= \frac{1}{2} m_1 u_1^2 + \frac{1}{2} m_2 \left(\frac{m_1}{m_2}\right)^2 u_1^2$$
> $$= \frac{1}{2} m_1 u_1^2 \left(1 + \frac{m_1}{m_2}\right) = \frac{1}{2} m_1 u_1^2 \left(\frac{m_1 + m_2}{m_2}\right)$$
>
> Let the relative velocity be $\vec{u}_{rel} = \vec{u}_1 - \vec{u}_2$.
> $$\vec{u}_{rel} = \vec{u}_1 + \frac{m_1}{m_2} \vec{u}_1 = \vec{u}_1 \left(1 + \frac{m_1}{m_2}\right) = \frac{m_1 + m_2}{m_2} \vec{u}_1$$
> $$\rightarrow \vec{u}_1 = \frac{m_2}{m_1 + m_2} \vec{u}_{rel}$$
>
> Substituting back into $T_{CM}$:
> $$T_{CM} = \frac{1}{2} m_1 \left(\frac{m_2}{m_1+m_2}\right)^2 \left(\frac{m_1+m_2}{m_2}\right) |\vec{u}_{rel}|^2$$
> $$T_{CM} = \frac{1}{2} \mu u_{rel}^2$$
> (where $\mu = \frac{m_1 m_2}{m_1 + m_2}$ is the reduced mass)

> **Elaboration:**
> For a two-body system, calculations are simplified by transforming into the Center of Mass frame. In this frame, the total momentum is zero, which means the two particles always move in opposite directions with momentum of equal magnitude ($m_1 u_1 = m_2 u_2$). 
>
> By expressing the velocities of the individual particles in terms of their relative velocity $\vec{u}_{rel} = \vec{u}_1 - \vec{u}_2$ (which is frame-independent and equal to $\vec{v}_1 - \vec{v}_2$ in the lab frame), the total kinetic energy in the CM frame can be written elegantly in terms of a single fictitious particle with **reduced mass ($\mu$)** moving at the relative velocity. This reduces a two-body problem to an equivalent one-body problem, which is a fundamental technique in planetary dynamics and scattering theory.

---

## 3. Potential Energy of a System (انرژی پتانسیل سیستم)

**Original Notes Transcription:**
> **- انرژی پتانسیل:** (Potential Energy)
> *ریاضیدان‌ها: $\vec{V}$ میدان پتانسیل است.* (Mathematicians: $\vec{V}$ is the potential field.)
>
> **قدم I:** (Step I)
> $$\vec{V}(\vec{r}) \rightarrow \vec{V}(\vec{r}) = \vec{\nabla}\Phi(\vec{r})$$
>
> **قدم II) میدان خارجی:** (Step II: External Field)
> $$\vec{F}(\vec{r}) = q \vec{g}(\vec{r})$$
> (where $q$ represents electric charge or mass, and $\vec{g}$ represents electric field or gravitational field)
> $$\vec{g}(\vec{r}) = -\vec{\nabla}\Phi_g(\vec{r}) \rightarrow \vec{F}(\vec{r}) = -q \vec{\nabla}\Phi_g(\vec{r})$$
>
> The work done along a path:
> $$W_{12} = \int_1^2 \vec{F}(\vec{r}) \cdot d\vec{r} = -q \int_1^2 \vec{\nabla}\Phi_g(\vec{r}) \cdot d\vec{r}$$
> $$= -q \left[\Phi_g(\vec{r}_2) - \Phi_g(\vec{r}_1)\right] \equiv -q\Phi_g(\vec{r}_2) + q\Phi_g(\vec{r}_1) \equiv U(\vec{r}_1) - U(\vec{r}_2)$$
> *(Up to here, we dealt with the concept of potential!)*
>
> **قدم III:** (Step III)
> **مثال I:** *در سیستم روبرو، تنها برهم‌کنش گرانشی دو به دوی ذرات وجود دارد.* (In the system opposite, there is only pairwise gravitational interaction between the particles.)
>
> **مثال II: سیستم یک ذره و زمین:** (Example II: Single particle and Earth system)
> Enclosing Earth ($M_{earth}$) and mass ($m$) with spring:
> $$\vec{F}_g \downarrow, m \uparrow \rightsquigarrow F_g = -\nabla \Phi_g$$
> $$K + U = \text{const}$$
>
> **• مسأله در اینجا، تعریف کردن انرژی پتانسیل کل سیستم است.** (The problem here is to define the total potential energy of the system.)
> $$K + U = E = \text{const}$$

> **Elaboration:**
> The potential energy $U$ is defined via the work done by conservative forces. For a conservative force field $\vec{F}$, the work done moving a particle from point 1 to point 2 is independent of the path taken and depends only on the endpoints. This allows us to define a potential energy function $U(\vec{r})$ such that $W_{12} = -\Delta U = U(\vec{r}_1) - U(\vec{r}_2)$.
>
> When considering a system of multiple particles, we must distinguish between:
> 1. **External Potential Energy:** Due to external fields (like a uniform gravitational field or an external electric field) acting on the individual particles.
> 2. **Internal Potential Energy:** Due to the pairwise interactions between the particles within the system (e.g., gravitational forces, electrostatic forces, or spring forces between them).
>
> To write a consistent conservation of energy equation $K + U = E$, the total potential energy $U$ must include both external contributions and all pairwise internal interactions.

---

## 4. Configuration Potential Energy & Symmetries (انرژی پتانسیل پیکربندی و تقارن‌ها)

**Original Notes Transcription:**
> **- پیکربندی (Configuration):**
> $$m_\alpha \rightarrow \vec{r}_\alpha$$
>
> Assembly from infinity ($\infty$):
> Bringing $m_1$ from $\infty$:
> $$W_{s1} = 0$$
> Bringing $m_2$ from $\infty$ in the presence of $m_1$:
> $$W_{s2} = q_2 \Phi_{g1}(|\vec{r}_2 - \vec{r}_1|)$$
>
> $$\rightsquigarrow W_{tot} = U_{tot} = U(|\vec{r}_i - \vec{r}_j|) \rightarrow \text{انرژی پتانسیل پیکربندی}$$ (Configuration Potential Energy)
>
> **Guideline:**
> $$\text{I: } U(\vec{r}_i) \xrightarrow{\text{همگنی (Homogeneity)}} U(\vec{r}_i - \vec{r}_j) \xrightarrow{\text{همسانگردی (Isotropy)}} \text{II: } U(|\vec{r}_i - \vec{r}_j|)$$
>
> Translation invariance:
> $$\begin{cases} \vec{r}_i \rightarrow \vec{r}_i + \vec{a} \\ \vec{r}_j \rightarrow \vec{r}_j + \vec{a} \end{cases}$$
> Rotation invariance:
> $$\begin{cases} \vec{r}_i \rightarrow R\vec{r}_i \\ \vec{r}_j \rightarrow R\vec{r}_j \end{cases}$$

> **Elaboration:**
> The potential energy of a configuration of particles can be computed by calculating the work required to assemble the system by bringing each particle from infinity to its final position, one by one. The first particle requires no work ($W_1 = 0$) because there are no other particles to exert forces. The second particle requires work to overcome the force exerted by the first particle, and so on. Summing these works gives the total configuration potential energy.
>
> Fundamental symmetries of space impose constraints on the mathematical form of the potential energy:
> - **Homogeneity of Space (Translation Invariance):** If space is uniform, translating the entire system by a vector $\vec{a}$ should not change its internal potential energy. This implies that the potential energy of interaction between two particles can only depend on their relative position vector, $\vec{r}_i - \vec{r}_j$.
> - **Isotropy of Space (Rotation Invariance):** If space has no preferred direction, rotating the entire system should not change its internal potential energy. This further restricts the potential to depend only on the scalar distance between the particles, $|\vec{r}_i - \vec{r}_j|$.
>
> If an external field (like a uniform electric field $\vec{E}$) is introduced, it breaks these symmetries for the system as a whole, because translating or rotating the system relative to the external field changes its energy.

---

## 5. Elastic Collisions in One Dimension (برخورد دو ذره‌ای کشسان در یک بعد)

**Original Notes Transcription:**
> **■ برخورد دو ذره‌ای کشسان:** (Elastic Two-Particle Collision)
> **قدم اول: برخورد دو ذره‌ای در یک بعد:** (First Step: Two-particle collision in 1D)
> Assume $v_1$ is positive.
>
> **- مسأله‌ی برخورد:** (The Collision Problem)
> **۱) انتخاب دستگاه (Election of frame):**
>
> **قدم I:**
> $$V_{CM} = \frac{m_1 v_1 + m_2 v_2}{m_1 + m_2}$$
>
> **قدم II) در دستگاه مرکز جرم:**
> $$\begin{cases} u_1 \equiv v_1 - V_{CM} \\ u_2 \equiv v_2 - V_{CM} \end{cases} \rightarrow \begin{cases} u_1 = v_1 - \frac{m_1 v_1 + m_2 v_2}{m_1 + m_2} \\ u_2 = v_2 - \frac{m_1 v_1 + m_2 v_2}{m_1 + m_2} \end{cases}$$
>
> **قدم III) پایستگی تکانه و انرژی در دستگاه CM:**
> Before collision: $u_1, u_2$ (CM), $v_1, v_2$ (Lab)
> After collision: $u'_1, u'_2$ (CM), $v'_1, v'_2$ (Lab)
>
> **پایستگی تکانه خطی:**
> $$\text{(I) } m_1 u_1 + m_2 u_2 = m_1 u'_1 + m_2 u'_2 = 0$$
> **پایستگی انرژی:**
> $$\text{(II) } \frac{1}{2} m_1 u_1^2 + \frac{1}{2} m_2 u_2^2 = \frac{1}{2} m_1 {u'_1}^2 + \frac{1}{2} m_2 {u'_2}^2$$
>
> Solving these equations:
> $$\rightarrow \begin{cases} |u'_1| = |u_1| \\ |u'_2| = |u_2| \end{cases}$$
>
> **جواب I:** (Trivial solution)
> $$\begin{cases} u'_1 = u_1 \\ u'_2 = u_2 \end{cases}$$
> *تغییری نکرده، برخورد صورت نگرفته (Trivial answer: no collision occurred)*
>
> **جواب II:** (Physical solution)
> $$\begin{cases} u'_1 = -u_1 \\ u'_2 = -u_2 \end{cases}$$
>
> **بعد از برخورد:** (After collision - transforming back to Lab frame)
> $$u'_1 = -u_1 \xrightarrow{\text{Lab-frame}} v'_1 = u'_1 + V_{CM}$$
> $$u'_2 = -u_2 \xrightarrow{\text{Lab-frame}} v'_2 = u'_2 + V_{CM}$$
> $$\rightarrow v'_1 = -u_1 + V_{CM} = -(v_1 - V_{CM}) + V_{CM} = -v_1 + 2V_{CM}$$
> $$\rightarrow v'_2 = -u_2 + V_{CM} = -(v_2 - V_{CM}) + V_{CM} = -v_2 + 2V_{CM}$$

> **Elaboration:**
> To analyze a one-dimensional elastic collision, we use the Center of Mass frame. In the CM frame, the conservation laws simplify tremendously:
> 1. Linear momentum conservation requires the particles to have equal and opposite momenta both before and after the collision ($p_1 = -p_2$ and $p'_1 = -p'_2$).
> 2. Kinetic energy conservation then implies that the magnitudes of the velocities in the CM frame must remain unchanged ($|u'_i| = |u_i|$).
>
> This yields two possible mathematical solutions:
> - **Solution I (Trivial):** The velocities are unchanged. Physically, this corresponds to the particles passing through each other without interacting.
> - **Solution II (Physical):** The velocities reverse their directions. Thus, each particle simply bounces back with its speed in the CM frame preserved ($u'_i = -u_i$).
>
> By transforming back to the Lab frame, we find that the final lab velocities are $v'_i = -v_i + 2V_{CM}$. This formula is extremely powerful, providing the final velocities directly without needing to solve quadratic equations in the Lab frame.

---

## 6. Collisions with a Moving Wall & Energy Classification (برخورد با دیوار متحرک و دسته‌بندی انرژی)

**Original Notes Transcription:**
> **• یک تعبیر هیولا!** (A Monster/Striking Interpretation!)
> Collision with a moving wall of mass $M \rightarrow \infty$ at velocity $V$:
> A ball of mass $m$ with velocity $v$ collides with it.
> Since $M \rightarrow \infty$, the center of mass velocity is dominated by the wall: $V_{CM} \approx V$.
> Using the collision formula:
> $$v' = -v + 2V$$
>
> **II) برخوردهای کلی: کشسان، ناکشسان، فوق‌کشسان:** (General Collisions: Elastic, Inelastic, Super-elastic)
> **I)** $$m_1 \vec{v}_1 + m_2 \vec{v}_2 = m_1 \vec{v}'_1 + m_2 \vec{v}'_2$$
> **II)** $$\frac{1}{2} m_1 |\vec{v}'_1|^2 + \frac{1}{2} m_2 |\vec{v}'_2|^2 = \frac{1}{2} m_1 |\vec{v}_1|^2 + \frac{1}{2} m_2 |\vec{v}_2|^2 + Q \rightarrow \begin{cases} Q = 0 \quad \text{(Elastic)} \\ Q > 0 \quad \text{(Super-elastic)} \\ Q < 0 \quad \text{(Inelastic)} \end{cases}$$
>
> **⚠️ حداکثر انرژی قابل اتلاف: انرژی جنبشی کل در دستگاه مرکز جرم**
> (Maximum possible dissipated energy is the total kinetic energy in the CM frame)
>
> **Super-elastic example ($Q > 0$):**
> Release of chemical energy converting to kinetic energy:
> $$K + U_{chemical} = K'$$
> (e.g., an explosive reaction between colliding objects, where chemical energy $\Delta E_{chemical}$ is converted into kinetic energy $K$, resulting in $Q > 0$)

> **Elaboration:**
> The formula $v' = -v + 2V$ has a classic application: a light ball colliding elastically with a massive wall moving at velocity $V$. Since the wall's mass is effectively infinite, the center of mass velocity of the system is simply $V$. Applying the formula yields the final velocity of the ball: $v' = -v + 2V$. This result explains how spacecraft gain speed via gravitational slingshots (where the planet acts as the moving "wall" of infinite mass).
>
> Collisions in general are classified by the change in total kinetic energy, quantified by the $Q$-value:
> - **Elastic ($Q = 0$):** Kinetic energy is conserved.
> - **Inelastic ($Q < 0$):** Kinetic energy is lost (converted to heat, sound, or internal deformation). The maximum possible kinetic energy loss occurs in a completely inelastic collision when the particles stick together; in this case, the final velocity is $\vec{V}_{CM}$, and the entire internal kinetic energy in the CM frame ($\frac{1}{2} \mu u_{rel}^2$) is dissipated.
> - **Super-elastic ($Q > 0$):** Kinetic energy increases. This occurs when stored internal energy (such as chemical energy in an explosive device or nuclear energy) is triggered by the collision and converted into kinetic energy.
