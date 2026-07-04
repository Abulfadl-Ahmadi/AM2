# Chapter 11: Dynamics of Rigid Bodies - Lecture: May 11, 2026

## 1. Foucault Pendulum: Equations of Motion (معادلات حرکت آونگ فوکو)

**Original Notes Transcription:**
> ■ **آونگ فوکو:** (Foucault Pendulum)
> ■ **حرکت جسم صلب:** (Motion of a Rigid Body)
> 
> **Step I)**
> $$\vec{a}_{rot} = \frac{\vec{F}_{eff}}{m} = \frac{\vec{F}}{m} - 2\vec{\omega} \times \vec{v}_{rot}$$
> $$\vec{F} = \vec{g} m + \vec{T}$$
> 
> *Boxed centrifugal approximation:*
> $$-m\vec{\omega}\times(\vec{\omega}\times\vec{R}) - m\vec{\omega}\times(\vec{\omega}\times\vec{r}) \xrightarrow{|r| \ll R} \approx -m\vec{\omega}\times(\vec{\omega}\times\vec{R})$$
> 
> $$\rightarrow \vec{a}_{rot} = \vec{g} + \frac{\vec{T}}{m} - 2\vec{\omega}\times\vec{v}_{rot}$$
> *(where $\vec{g} = \vec{g}_{eff}$ is the effective gravity including the centrifugal term)*
> 
> *(Diagram shows the pendulum of length $l$ suspended from $(0, 0, l)$ with bob at $(x, y, z)$ deflected by angle $\theta$. The tension $\vec{T}$ points along the string, and gravity $m\vec{g}$ points vertically downward).*
> 
> **Step II)**
> **(a) Tension components for small oscillations ($\theta \ll 1$):**
> $$\begin{cases} T_x = -T \frac{x}{l} \\ T_y = -T \frac{y}{l} \\ T_z \approx T \end{cases}$$
> 
> **(b) Effective gravity components:**
> $$g_x = 0, \quad g_y = 0, \quad g_z = -g \approx -g_0$$
> 
> **(c) Earth's rotation vector components:**
> $$\begin{cases} \omega_x = -\omega \cos\lambda \\ \omega_y = 0 \\ \omega_z = \omega \sin\lambda \end{cases}$$
> 
> **(d) Relative velocity components (since vertical motion is negligible, $z \approx 0 \rightarrow \dot{z} \approx 0$):**
> $$\begin{cases} (\vec{v}_{rot})_x \equiv \dot{x} \\ (\vec{v}_{rot})_y \equiv \dot{y} \\ (\vec{v}_{rot})_z \approx 0 \end{cases}$$
> 
> **Step III)**
> **Coriolis cross product components:**
> $$(\vec{\omega} \times \vec{v}_{rot})_x \approx -\dot{y}\omega \sin\lambda$$
> $$(\vec{\omega} \times \vec{v}_{rot})_y \approx \dot{x}\omega \sin\lambda$$
> $$(\vec{\omega} \times \vec{v}_{rot})_z \approx -\dot{y}\omega \cos\lambda \quad (\text{بی اهمیت - ذره در جهت z حرکت ندارد / Unimportant})$$
> 
> **معادلات حرکت:** (Equations of motion:)
> $$\begin{cases} (I) \quad \ddot{x} = - \frac{Tx}{lm} + 2\dot{y}\omega_z \\ (II) \quad \ddot{y} = - \frac{Ty}{lm} - 2\dot{x}\omega_z \end{cases} \quad (\text{where } \omega_z = \omega \sin\lambda)$$
> 
> $$\rightarrow \begin{cases} \ddot{x} + \alpha^2 x = 2\omega_z \dot{y} \\ \ddot{y} + \alpha^2 y = -2\omega_z \dot{x} \end{cases}$$
> 
> *Boxed parameters:*
> $$\alpha = \sqrt{\frac{T}{ml}}, \quad \omega_0 = \sqrt{\frac{g}{l}}$$
> $$\alpha \approx \text{const} \rightarrow \alpha = \sqrt{\frac{g}{l}} \quad (\text{since } T \approx mg)$$
> 
> *دستگاه معادلات خطی، مرتبه دوم جفت شده:* (Coupled, second-order linear system of equations:)
> - Trying simple substitution: $\ddot{x} + \alpha^2 x = 2\omega_z \dot{y} \rightarrow \text{Failed!}$
> - Trying direct addition: $(\ddot{x}+\ddot{y}) + \alpha^2(x+y) = 2\omega_z(\dot{y}-\dot{x}) \rightarrow \text{Failed!}$
> 
> **جبر خطی اضافه بین خودمان:** (Extra linear algebra between us:)

> **Elaboration:**
> The lecture continues the analysis of the Foucault Pendulum. We set up the equations of motion in the local rotating Earth frame.
> 
> 1. **Acceleration Equation:** The relative acceleration $\vec{a}_{rot}$ is dictated by real forces (gravity $\vec{g} m$ and string tension $\vec{T}$) plus the Coriolis force. The centrifugal force is absorbed into the effective gravity $\vec{g}$ using the $|\vec{r}| \ll |\vec{R}|$ approximation.
> 
> 2. **Force Components:**
>    - **Tension:** For small oscillations ($\theta \ll 1$), the vertical displacement $z$ is negligible, so the vertical tension component is $T_z \approx T \approx mg$. The horizontal restoring components are $T_x = -T \frac{x}{l}$ and $T_y = -T \frac{y}{l}$.
>    - **Gravity:** Points purely in the negative z-direction: $(0, 0, -g)$.
>    - **Coriolis Acceleration:** The relative velocity is horizontal: $\vec{v}_{rot} = (\dot{x}, \dot{y}, 0)$. The cross product $\vec{\omega} \times \vec{v}_{rot}$ yields:
>      - $x$-component: $-\omega_z \dot{y} = -\omega \sin\lambda \dot{y}$.
>      - $y$-component: $\omega_z \dot{x} = \omega \sin\lambda \dot{x}$.
>      - The $z$-component is neglected since the bob is constrained vertically.
> 
> 3. **Coupled System:** Substituting these components into $\vec{a}_{rot} = \vec{g} + \frac{\vec{T}}{m} - 2\vec{\omega} \times \vec{v}_{rot}$ yields two coupled, second-order linear differential equations:
>    $$ \ddot{x} + \alpha^2 x = 2\omega_z \dot{y} $$
>    $$ \ddot{y} + \alpha^2 y = -2\omega_z \dot{x} $$
>    where $\alpha = \sqrt{g/l}$ is the natural frequency of the pendulum and $\omega_z = \omega \sin\lambda$ is the vertical component of Earth's rotation. Standard algebraic additions fail to uncouple these equations, prompting the use of complex numbers.

---

## 2. Foucault Pendulum: Complex Coordinate Solution (حل با مختصات مختلط)

**Original Notes Transcription:**
> $$\begin{cases} \zeta = x + iy \\ \dot{\zeta} = \dot{x} + i\dot{y} \\ \ddot{\zeta} = \ddot{x} + i\ddot{y} \end{cases}$$
> 
> $$\rightarrow I + i \times II$$
> $$\rightarrow (\ddot{x} + i\ddot{y}) + \alpha^2 (x + iy) = 2\omega_z (\dot{y} - i\dot{x}) = -2i\omega_z (\dot{x} + i\dot{y}) \quad \checkmark$$
> 
> *Boxed equation:*
> $$\ddot{\zeta} + 2i\omega_z \dot{\zeta} + \alpha^2 \zeta = 0 \quad (\zeta = |\zeta|e^{i\phi})$$
> 
> **Step IV)** Assume solution $\zeta(t) = A e^{i\Omega t}$:
> $$\rightarrow -\Omega^2 + 2i\omega_z (i\Omega) + \alpha^2 = 0$$
> $$\rightarrow \Omega^2 + 2\omega_z \Omega - \alpha^2 = 0 \rightarrow \Omega = -\omega_z \pm \underbrace{\sqrt{\omega_z^2 + \alpha^2}}_{\tilde{\omega}}$$
> 
> $$\rightarrow \zeta(t) \propto e^{-i\omega_z t} \left[ A e^{+i\tilde{\omega} t} + B e^{-i\tilde{\omega} t} \right]$$
> 
> **تعیین A و B:** (Determining A and B:)
> $$\dot{x} = \dot{y} = 0 \rightarrow \dot{\zeta}(t=0) = 0$$
> $$x_0, y_0 \rightarrow |\zeta(t=0)| = A_0 = \sqrt{x_0^2 + y_0^2} \equiv R_0$$
> 
> $$\dot{\zeta}(0) = -i\omega_z \zeta(0) + i\tilde{\omega}(A - B) = 0$$
> Since $\omega_z \ll \tilde{\omega}$ and $\tilde{\omega} = \sqrt{\omega_z^2 + \alpha^2} \approx \alpha = \sqrt{g/l}$:
> $$\rightarrow i\tilde{\omega} A - i\tilde{\omega} B \approx 0 \rightarrow A = B$$
> 
> Since $A = B$ and $\zeta(0) = R_0 \rightarrow 2A = R_0 \rightarrow A = R_0/2$:
> $$\zeta(t) = e^{-i\phi(t)} R_0 \cos \tilde{\omega} t$$
> $$\text{where } \phi(t) = \phi_0 + \omega_z t$$
> 
> *(Diagram shows the precessing Lissajous flower-like rosette pattern of the pendulum, showing how the plane of swing rotates with angular velocity $\omega_z = \omega \sin\lambda$ relative to the ground).*

> **Elaboration:**
> We solve the coupled equations of motion by defining a complex coordinate $\zeta = x + iy$.
> 
> 1. **Uncoupling using Complex Variable:**
>    Multiplying the second equation by $i$ and adding it to the first:
>    $$ (\ddot{x} + i\ddot{y}) + \alpha^2 (x + iy) = 2\omega_z (\dot{y} - i\dot{x}) $$
>    Using $i\dot{\zeta} = i(\dot{x} + i\dot{y}) = -\dot{y} + i\dot{x}$, we see that the RHS is exactly $-2i\omega_z \dot{\zeta}$. This yields:
>    $$ \ddot{\zeta} + 2i\omega_z \dot{\zeta} + \alpha^2 \zeta = 0 $$
> 
> 2. **Solving the Characteristic Equation:**
>    We plug in $\zeta = e^{i\Omega t}$ to get the characteristic equation:
>    $$ \Omega^2 + 2\omega_z \Omega - \alpha^2 = 0 $$
>    This quadratic equation has roots $\Omega = -\omega_z \pm \tilde{\omega}$, where $\tilde{\omega} = \sqrt{\omega_z^2 + \alpha^2}$.
>    The general solution is:
>    $$ \zeta(t) = e^{-i\omega_z t} \left[ A e^{i\tilde{\omega} t} + B e^{-i\tilde{\omega} t} \right] $$
> 
> 3. **Applying Boundary Conditions:**
>    We release the pendulum from rest ($\dot{\zeta}(0) = 0$) at initial position $\zeta(0) = R_0$.
>    Differentiating $\zeta(t)$ and setting $t=0$:
>    $$ \dot{\zeta}(0) = -i\omega_z \zeta_0 + i\tilde{\omega}(A-B) = 0 $$
>    Because Earth's rotation is extremely slow compared to the pendulum's swing ($\omega_z \ll \tilde{\omega}$), the first term is negligible, which leads to $A = B$.
>    Using the initial position $\zeta(0) = A+B = 2A = R_0$, we get $A = B = R_0/2$.
> 
> 4. **Physical Interpretation:**
>    The final solution is:
>    $$ \zeta(t) = R_0 e^{-i\omega_z t} \cos \tilde{\omega} t $$
>    This represents a simple harmonic motion $\cos \tilde{\omega} t$ (the back-and-forth swing) multiplied by a slowly rotating complex phase $e^{-i\omega_z t}$. 
>    - The plane of swing rotates (precesses) at an angular rate of $\omega_z = \omega \sin\lambda$.
>    - At the North Pole ($\lambda = 90^\circ$), the plane precesses clockwise once every 24 hours ($\omega_z = \omega$).
>    - At the equator ($\lambda = 0$), there is no precession ($\omega_z = 0$).

---

## 3. Rigid Body Dynamics: Definitions & Reference Frames (تعاریف و دستگاه های مختصات در جسم صلب)

**Original Notes Transcription:**
> ■ **دینامیک اجسام صلب:** (Dynamics of Rigid Bodies:)
> - **جسم صلب:** فاصله نسبی دو به دوی ذرات آن تغییر نمی کند.
>   (Rigid body: a body in which the pairwise distance between its particles is constant.)
>   $$\forall i, j \quad |\vec{x}_i - \vec{x}_j| = \text{const}$$
> 
> - **مختصات جسمی:** مختصات (لختی / نالخت) که مبدأ و محورهای آن نسبت به جسم ثابت هستند.
>   (Body coordinates: coordinates (inertial / non-inertial) whose origin and axes are fixed relative to the body.)
>   *(Diagram shows a spacecraft "سفینه ماه" with its body axes $x, y, z$.)*
> 
> • **نکته اول:** در دستگاه جسمی سرعت هر نقطه از جسم (صلب) $\vec{v}_{\alpha, rot} = 0$.
> (Tip 1: In the body frame, the velocity of any point of the rigid body is zero.)
> 
> $$\rightarrow (\vec{v}_\alpha)_{fixed} = \vec{V} + \vec{\omega} \times \vec{r}_\alpha$$

> **Elaboration:**
> The lecture transitions to the study of **Rigid Bodies**.
> 
> A **rigid body** is a system of particles in which the distance between any two particles is constant under all circumstances. That is, $|\vec{x}_i - \vec{x}_j| = \text{const}$ for all particles $i$ and $j$.
> 
> To describe the motion of a rigid body, we introduce a **Body-fixed coordinate system** (or simply the body frame). The origin and axes of this frame are locked to the body and move with it. 
> 
> - Because of this definition, the relative velocity $\vec{v}_{\alpha, rot}$ of any particle of the rigid body in the body frame is strictly zero.
> - The velocity of any particle $\alpha$ as observed in the fixed inertial frame is given by the frame velocity transformation:
>   $$ (\vec{v}_\alpha)_{fixed} = \vec{V} + \vec{\omega} \times \vec{r}_\alpha $$
>   where $\vec{V}$ is the translational velocity of the body frame's origin, $\vec{\omega}$ is the angular velocity of the rigid body, and $\vec{r}_\alpha$ is the position of the particle in the body frame.

---

## 4. Kinetic Energy of a Rigid Body & The Inertia Tensor (انرژی جنبشی جسم صلب و تانسور لختی)

**Original Notes Transcription:**
> **قدم اول: انرژی جنبشی جسم صلب در دستگاه آزمایشگاه (لخت) را محاسبه کنید:**
> (Step 1: Calculate the kinetic energy of the rigid body in the Lab frame (inertial):)
> $$v_\alpha \rightarrow |\vec{v}_{\alpha, fixed}|$$
> 
> $$T = \frac{1}{2} \sum_\alpha m_\alpha v_\alpha^2 = \frac{1}{2} \sum_\alpha m_\alpha (\vec{V} + \vec{\omega} \times \vec{r}_\alpha)^2$$
> 
> $$= \frac{1}{2} \sum_\alpha m_\alpha V^2 + \sum_\alpha m_\alpha \vec{V} \cdot (\vec{\omega} \times \vec{r}_\alpha) + \frac{1}{2} \sum_\alpha m_\alpha (\vec{\omega} \times \vec{r}_\alpha)^2$$
> 
> $$= \frac{1}{2} M V^2 + \vec{V} \cdot \left(\vec{\omega} \times \sum_\alpha m_\alpha \vec{r}_\alpha\right) + \frac{1}{2} \sum_\alpha m_\alpha (\vec{\omega} \times \vec{r}_\alpha)^2$$
> 
> *با قرار دادن (تنظیم) مبدأ دستگاه جسمی روی مرکز جرم (CM)، از دست جمله دوم خلاص می شویم.*
> (By setting the origin of the body frame on the Center of Mass (CM), we get rid of the second term.)
> $$\sum_\alpha m_\alpha \vec{r}_\alpha = 0$$
> 
> *Boxed equations:*
> $$T = T_{trans} + T_{rot}$$
> $$T_{trans} = \frac{1}{2} M V^2$$
> $$T_{rot} = \frac{1}{2} \sum_\alpha m_\alpha (\vec{\omega} \times \vec{r}_\alpha)^2$$
> 
> **قدم دوم: محاسبه $T_{rot}$ برای یک جسم صلب با شکل کلی:**
> (Step 2: Calculate $T_{rot}$ for a rigid body of general shape:)
> 
> $$(\vec{A} \times \vec{B})^2 = A^2 B^2 - (\vec{A} \cdot \vec{B})^2$$
> $$T_{rot} = \frac{1}{2} \sum_\alpha m_\alpha \left[ \omega^2 r_\alpha^2 - (\vec{\omega} \cdot \vec{r}_\alpha)^2 \right]$$
> 
> **نمادگذاری:** (Notation:)
> Let $\alpha$ represent the particle index, and $i, j, k = 1, 2, 3$ represent component indices.
> $$\vec{r}_\alpha = (x_{\alpha 1}, x_{\alpha 2}, x_{\alpha 3})$$
> $$\vec{\omega} = (\omega_1, \omega_2, \omega_3)$$
> 
> $$T_{rot} = \frac{1}{2} \sum_\alpha m_\alpha \left[ \left( \sum_i \omega_i^2 \right) \left( \sum_k x_{\alpha k}^2 \right) - \left( \sum_i \omega_i x_{\alpha i} \right) \left( \sum_j \omega_j x_{\alpha j} \right) \right]$$
> 
> Using $\sum_i \omega_i^2 = \sum_{i,j} \omega_i \omega_j \delta_{ij}$:
> $$T_{rot} = \frac{1}{2} \sum_{i,j} \omega_i \omega_j \sum_\alpha m_\alpha \left( \delta_{ij} \sum_k x_{\alpha k}^2 - x_{\alpha i} x_{\alpha j} \right)$$
> 
> *Boxed final result:*
> $$T_{rot} = \frac{1}{2} \sum_{i,j} \omega_i \omega_j I_{ij}$$
> $$I_{ij} \equiv \sum_\alpha m_\alpha \left( \delta_{ij} \sum_k x_{\alpha k}^2 - x_{\alpha i} x_{\alpha j} \right)$$
> 
> ⚠️ **از آنجایی که $T$ یک کمیت نرده ای است، و $\vec{\omega}$ یک کمیت برداری است، $I_{ij}$ یک تانسور مرتبه ۲ است.**
> (Since $T$ is a scalar quantity, and $\vec{\omega}$ is a vector quantity, $I_{ij}$ is a tensor of rank 2.)

> **Elaboration:**
> We derive the kinetic energy of a rigid body and introduce the **Moment of Inertia Tensor**.
> 
> 1. **Kinetic Energy Separation:**
>    By substituting $\vec{v}_\alpha = \vec{V} + \vec{\omega} \times \vec{r}_\alpha$ into the kinetic energy sum, we get three terms:
>    - The translation term $\frac{1}{2} M V^2$.
>    - The cross term $\vec{V} \cdot (\vec{\omega} \times \sum m_\alpha \vec{r}_\alpha)$.
>    - The rotation term $\frac{1}{2} \sum m_\alpha (\vec{\omega} \times \vec{r}_\alpha)^2$.
>    
>    If we position our body-frame origin exactly at the Center of Mass (CM), the position vectors satisfy $\sum m_\alpha \vec{r}_\alpha = 0$, causing the cross term to vanish. Thus, König's theorem is preserved:
>    $$ T = T_{trans} + T_{rot} = \frac{1}{2} M V^2 + \frac{1}{2} \sum_\alpha m_\alpha (\vec{\omega} \times \vec{r}_\alpha)^2 $$
> 
> 2. **Inertia Tensor Derivation:**
>    Using the vector identity $(\vec{A} \times \vec{B})^2 = A^2 B^2 - (\vec{A} \cdot \vec{B})^2$, we rewrite the rotational kinetic energy:
>    $$ T_{rot} = \frac{1}{2} \sum_\alpha m_\alpha \left[ \omega^2 r_\alpha^2 - (\vec{\omega} \cdot \vec{r}_\alpha)^2 \right] $$
>    To extract the angular velocity components $\omega_i, \omega_j$ from this summation, we express the vectors in component form:
>    - $\vec{r}_\alpha = (x_{\alpha 1}, x_{\alpha 2}, x_{\alpha 3})$
>    - $\vec{\omega} = (\omega_1, \omega_2, \omega_3)$
>    
>    By substituting these and utilizing the Kronecker delta ($\delta_{ij}$) to write $\omega^2 = \sum \omega_i \omega_j \delta_{ij}$, we isolate $\omega_i \omega_j$:
>    $$ T_{rot} = \frac{1}{2} \sum_{i,j} \omega_i \omega_j I_{ij} $$
>    where $I_{ij}$ is the **Moment of Inertia Tensor**:
>    $$ I_{ij} \equiv \sum_\alpha m_\alpha \left( \delta_{ij} \sum_k x_{\alpha k}^2 - x_{\alpha i} x_{\alpha j} \right) $$
> 
>    Since the kinetic energy $T_{rot}$ is a coordinate-independent scalar (rank 0 tensor) and angular velocity $\vec{\omega}$ is a vector (rank 1 tensor), the coefficients $I_{ij}$ must transform as a rank 2 tensor. This tensor describes how mass is distributed in 3D space relative to the rotation axes.
