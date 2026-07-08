# Chapter 9: Dynamics of a System of Particles (Continued)

> [!abstract] Navigation
> **Chapter:** [[Chapter 9 - Dynamics of a System of Particles]] | **Prev:** [[Note Apr 11, 2026]] | **Next:** [[Note Apr 18, 2026]] | [[Journal/Lecture Index|📚 All Lectures]]

## 1. Introduction & Overview

**Original Notes Transcription:**
> *"blockade of blockade"* 
> $\Delta O_{BSOH} > 0 \rightarrow f(f(o)) > f(o)$
> *Blockade of Strait of Hormoz*
> *Dates: 7 Oct. 2023, 28 Feb 2026*
> $\propto \exp(\mu t)$
> *نظریه گذار فاز : (Phase Transition Theory)*
> *True Vacuum*
> 
> Topics for today:
> - تکانه زاویه ای (Angular Momentum)
> - تکانه زاویه ای جسم صلب (Angular Momentum of a Rigid Body)
> - انرژی سیستم (Energy of the System)
> - برخورد $\rightarrow$ یک بعدی / در صفحه (Collisions $\rightarrow$ 1D / Planar)

> **Elaboration:**
> The lecture began with a brief tangent into phase transition theories (referencing "True Vacuum" and exponential decay models) before transitioning into the main classical mechanics topics. The core focus of this session is applying the previously established angular momentum principles ($\vec{\tau}_{ext} = d\vec{L}/dt$) specifically to rigid bodies, and deriving the kinetic energy of a system of particles.

---

## 2. Angular Momentum of a Rigid Body (تکانه زاویه ای جسم صلب)

**Original Notes Transcription:**
> جسم صلب : جسمی که اندازه ی فاصله دو به دوی ذرات آن ثابت است.
> *(Rigid body: a body in which the pairwise distance between its particles is constant.)*
> 
> جسم صلب حول یک محور ثابت دوران می کند : 
> *(A rigid body rotates around a fixed axis:)*
> Let $\vec{\omega} = \omega \hat{n}$ be the angular velocity.
> Particle $P$ is at position $\vec{r}_p$.
> Top-View projection:
> $|\Delta \vec{r}_p| = |\vec{r}_p| \sin\theta \times \Delta\phi$
> $\frac{|\Delta \vec{r}_p|}{\Delta t} = |\vec{r}_p| \sin\theta \times \left(\frac{\Delta\phi}{\Delta t}\right) = |\vec{r}_p| \omega \sin\theta$
> Vectorially: $\vec{v}_p = \vec{\omega} \times \vec{r}_p$ and $\frac{d\vec{v}}{dt} = \vec{\omega} \times \vec{v}$

> **Elaboration:**
> A rigid body is an idealized system where internal distances never change, meaning internal kinetic energy cannot be stored as potential energy of deformation. When a rigid body rotates around a fixed axis with angular velocity $\vec{\omega}$, every particle traces out a circle. The linear velocity $\vec{v}$ of any point $\vec{r}$ is perfectly defined by the cross product $\vec{\omega} \times \vec{r}$.

### The Inertia Tensor Derivation

**Original Notes Transcription:**
> مسأله ساده دو جرمی : *(Simple two-mass problem:)*
> $\vec{L} = \sum_\alpha \vec{r}_\alpha \times \vec{p}_\alpha$
> Since $\vec{v}_\alpha = \vec{\omega} \times \vec{r}_\alpha \rightarrow \vec{p}_\alpha = m_\alpha (\vec{\omega} \times \vec{r}_\alpha)$
> $\Rightarrow \vec{L} = \sum_\alpha m_\alpha \vec{r}_\alpha \times (\vec{\omega} \times \vec{r}_\alpha)$
> 
> Using the vector triple product identity: $\vec{A} \times (\vec{B} \times \vec{C}) = \vec{B}(\vec{A} \cdot \vec{C}) - \vec{C}(\vec{A} \cdot \vec{B})$
> $\rightarrow \vec{L} = \sum_\alpha m_\alpha \left[ \vec{\omega}(\vec{r}_\alpha \cdot \vec{r}_\alpha) - \vec{r}_\alpha(\vec{\omega} \cdot \vec{r}_\alpha) \right]$

> **Elaboration:**
> By substituting the rotational velocity formula into the angular momentum definition, we obtain a relation that maps the angular velocity vector $\vec{\omega}$ to the angular momentum vector $\vec{L}$. The resulting mathematical structure (using the BAC-CAB rule) naturally gives rise to the **Moment of Inertia Tensor ($I$)**, proving that in general, $\vec{L}$ is not necessarily parallel to $\vec{\omega}$.

### Parallel and Perpendicular Components

**Original Notes Transcription:**
> Is $\vec{L} = I\vec{\omega}$?
> Decompose $\vec{r}_\alpha = \vec{r}_{\perp \alpha} + \vec{r}_{\parallel \alpha}$ (relative to the rotation axis $\vec{\omega}$).
> Since $\vec{\omega} \times \vec{r}_{\parallel \alpha} = 0$, we have $\vec{\omega} \times \vec{r}_\alpha = \vec{\omega} \times \vec{r}_{\perp \alpha}$.
> $\vec{L} = \sum_\alpha m_\alpha (\vec{r}_{\perp \alpha} + \vec{r}_{\parallel \alpha}) \times (\vec{\omega} \times \vec{r}_{\perp \alpha})$
> 
> **Term I:** $\sum_\alpha m_\alpha \vec{r}_{\perp \alpha} \times (\vec{\omega} \times \vec{r}_{\perp \alpha})$
> $= \left( \sum_\alpha m_\alpha |\vec{r}_{\perp \alpha}|^2 \right) \vec{\omega} = I_{\vec{\omega}} \vec{\omega}$
> 
> **Term II:** $\sum_\alpha m_\alpha \vec{r}_{\parallel \alpha} \times (\vec{\omega} \times \vec{r}_{\perp \alpha})$
> $= \sum_\alpha m_\alpha \vec{r}_{\perp \alpha} (\vec{r}_{\parallel \alpha} \cdot \vec{\omega}) \neq 0$

> **Elaboration:**
> We can split the position vector of each mass into a component parallel to the rotation axis ($\vec{r}_\parallel$) and a component perpendicular to it ($\vec{r}_\perp$). 
> - **Term I** yields the familiar scalar moment of inertia $I = \sum m r_\perp^2$. This component of $\vec{L}$ points exactly in the direction of $\vec{\omega}$.
> - **Term II** is the "dynamic imbalance" term. Unless the mass distribution is perfectly symmetric around the rotation axis, this term is non-zero. It creates a component of $\vec{L}$ that is perpendicular to the rotation axis. 
> 
> Because this perpendicular component of $\vec{L}$ rotates with the body, the total $\vec{L}$ vector is constantly changing direction! This means $d\vec{L}/dt \neq 0$, which implies a torque ($\vec{\tau}$) must be continuously applied by the bearings/mounts to keep the axis fixed (this causes vibration/wobble in unbalanced rotors).

---

## 3. Kinetic Energy of a System (انرژی سیستم)

**Original Notes Transcription:**
> انرژی جنبشی سیستم ذرات : *(Kinetic energy of a system of particles:)*
> $T = \sum_\alpha \frac{1}{2} m_\alpha |\dot{\vec{r}}_\alpha|^2$
> Using the CM decomposition: $\vec{r}_\alpha = \vec{R}_{CM} + \vec{r}'_\alpha$
> $\rightarrow T = \frac{1}{2} \sum_\alpha m_\alpha (\dot{\vec{R}}_{CM} + \dot{\vec{r}}'_\alpha) \cdot (\dot{\vec{R}}_{CM} + \dot{\vec{r}}'_\alpha)$
> $= \frac{1}{2} \left(\sum m_\alpha\right) |\dot{\vec{R}}_{CM}|^2 + \frac{1}{2} \sum_\alpha m_\alpha |\dot{\vec{r}}'_\alpha|^2 + \left( \sum_\alpha m_\alpha \dot{\vec{r}}'_\alpha \right) \cdot \dot{\vec{R}}_{CM}$
> 
> Since $\sum m_\alpha \dot{\vec{r}}'_\alpha = 0$, the cross term vanishes:
> $\rightarrow T = \underbrace{\frac{1}{2} M |\vec{V}_{CM}|^2}_{I} + \underbrace{\frac{1}{2} \sum_\alpha m_\alpha |\dot{\vec{r}}'_\alpha|^2}_{II}$
> *Term I: انرژی جنبشی مرکز جرم (Translational kinetic energy of CM)*
> *Term II: انرژی جنبشی در دستگاه مرکز جرم (Internal kinetic energy in the CM frame)*

> **Elaboration:**
> König's Theorem dictates that the total kinetic energy of any system of particles can be cleanly separated into two independent parts:
> 1. The macroscopic translational energy of the entire system moving as a single point mass at the Center of Mass.
> 2. The microscopic/internal kinetic energy of the particles moving relative to the Center of Mass (this includes rotational energy, vibrational energy, or thermal energy).

### Maximum Energy Dissipation in Collisions

**Original Notes Transcription:**
> سؤال : بیشینه انرژی اتلافی در یک سیستم ذرات : 
> *(Question: Maximum dissipated energy in a system of particles:)*
> پایستگی تکانه کل : چون نیروی خارجی نداریم $\rightarrow \vec{V}_{CM} = \text{const}$
> *(Conservation of total momentum: Because we have no external force $\rightarrow \vec{V}_{CM} = \text{const}$)*
> در دستگاه مرکز جرم $V_{CM}=0$ ، اتلاف همه انرژی معادل اتلاف کل جمله II است.
> *(In the center of mass frame $V_{CM}=0$, dissipation of all energy is equivalent to the dissipation of the entire Term II.)*

> **Elaboration:**
> In a completely inelastic collision between macroscopic objects (where they stick together), what is the maximum amount of kinetic energy that can be converted to heat/deformation? 
> Because total momentum must be conserved, the center of mass velocity $\vec{V}_{CM}$ cannot change. Therefore, Term I ($\frac{1}{2}M V_{CM}^2$) is "locked" and can never be dissipated. The maximum possible energy loss occurs when all internal relative motion ceases—meaning Term II goes entirely to zero.

---

## 4. Atomic Spectra Tangent (طیف اتمی)

**Original Notes Transcription:**
> طیف اتمی *(Atomic spectra)*
> $\Delta E = h\nu_\gamma$
> $\Delta E \rightarrow \text{دقیق} \rightarrow \nu_\gamma \rightarrow \text{دقیق}$
> *(Precise $\Delta E \rightarrow$ Precise $\nu_\gamma$)*

> **Elaboration:**
> The lecture ended with a brief connection to quantum mechanics. When an electron in an atom transitions between two discrete energy levels, the energy difference $\Delta E$ is exactly defined. Because energy is conserved, the emitted photon must carry exactly this energy. According to the Planck-Einstein relation ($E = h\nu$), a precisely defined energy results in a precisely defined frequency ($\nu$) of light, giving rise to sharp emission lines in atomic spectra.
