# Chapter 11: Dynamics of Rigid Bodies (Continued) - Lecture: May 30, 2026

> [!abstract] Navigation
> **Chapter:** [[Chapter 11 - Dynamics of Rigid Bodies]] | **Prev:** [[Note May 25, 2026]] | **Next:** [[Note Jun 1, 2026]] | [[Journal/Lecture Index|📚 All Lectures]]

## 1. Free Symmetric Top - Continued (فرفره متقارن آزاد - ادامه)

**Original Notes Transcription:**
> **Timeline / Headings:**
> - **فرفره متقارن آزاد (ادامه)** (Free symmetric top - continued)
> - **نوسانات جفت شده** (Coupled oscillations)
> 
> ■ مرور جلسه قبل:
> (1) $I_1 = I_2 \neq I_3$ : فرفره متقارن آزاد
> (2) $\vec{N} = 0$
> 
> Euler equations:
> $$I_1 \dot{\omega}_1 - (I_2 - I_3) \omega_2 \omega_3 = N_1 \quad \& \text{ permutation} \quad \left( \begin{matrix} 1 \searrow \\ 3 \leftarrow 2 \end{matrix} \right)$$
> 
> The solutions as functions of time ($\omega_1, \omega_2, \omega_3 \xrightarrow{\text{توابع } t}$):
> $$\begin{cases} \omega_3 = \text{const} \\ \omega_1 = A \cos \Omega t \\ \omega_2 = A \sin \Omega t \end{cases} \quad \text{where} \quad \Omega = \frac{I_3 - I_1}{I_1} \omega_3$$
> 
> ■ **نکته (۱):** به دلیل اینکه داریم $\vec{N} = 0$ ، پس بردار تکانه زاویه ای کل ثابت است: $\vec{L} = \text{const}$ و ما این بردار را در جهت $x_3'$ می گیریم. (Lab-frame (fixed frame))
> (Note 1: Because we have $\vec{N} = 0$, the total angular momentum vector is constant: $\vec{L} = \text{const}$, and we take this vector in the direction of the fixed spatial axis $x_3'$.)
> 
> ■ **نکته (۲):** معادلات به ما می گویند که اندازه بردار $\vec{\omega}$ ثابت است و این بردار ، حول محور $x_3$ (جسمی) با سرعت زاویه ای $\Omega$ می چرخد (حرکت تقدیمی).
> (Note 2: The equations tell us that the magnitude of vector $\vec{\omega}$ is constant and this vector rotates around the $x_3$ body axis with angular velocity $\Omega$ - precession motion.)
> 
> ■ **نکته (۳):** از آنجا که انرژی جنبشی دورانی ثابت است و نیز داریم $T_{rot} = \frac{1}{2} \vec{\omega} \cdot \vec{L}$ ، زاویه بین $\vec{\omega}$ و $\vec{L}$ باید ثابت باشد. ($\phi = \text{const}$)
> (Note 3: Since the rotational kinetic energy is constant and we also have $T_{rot} = \frac{1}{2} \vec{\omega} \cdot \vec{L}$, the angle between $\vec{\omega}$ and $\vec{L}$ must be constant.)
> 
> ■ **یادآوری:** برای دانشجویان کوشا و دقیق :
> (Reminder for diligent and precise students:)
> $$T_{rot} = \vec{\omega} \cdot \vec{L} / 2 = \frac{1}{2} \sum_{ij} \omega_i \omega_j I_{ij}$$
> $$T = T_{trans} + T_{rot}$$
> $$\vec{L}_{free} : \quad V_{CM} = \text{const} \xrightarrow{\text{به دلخواه}} \vec{V}_{CM} = 0$$

> **Elaboration:**
> The lecture begins with a summary of the free symmetric top. We recall that the absence of external torques guarantees that the total angular momentum $\vec{L}$ is perfectly stationary in the fixed laboratory frame (Lab-frame). We conveniently align our fixed spatial $x_3'$ axis with this vector $\vec{L}$.
> 
> The solutions to Euler's equations reveal two simultaneous precessions:
> 1. In the body frame, the angular velocity vector $\vec{\omega}$ maintains a constant magnitude and traces a cone around the body's symmetry axis ($x_3$) at a rate $\Omega$.
> 2. In the space frame, since the kinetic energy $T = \frac{1}{2}\vec{\omega}\cdot\vec{L}$ is constant, the projection of $\vec{\omega}$ onto the constant vector $\vec{L}$ must be constant. Thus, the angle $\phi$ between $\vec{\omega}$ and $\vec{L}$ never changes, meaning $\vec{\omega}$ precesses in a perfect cone around the fixed spatial axis.
> 
> A brief reminder points out that for a completely free body, the center of mass moves at a constant velocity. By simply jumping into an inertial frame moving with the CM ($\vec{V}_{CM} = 0$), we completely eliminate translational kinetic energy ($T_{trans}$), leaving pure rotation.

---

## 2. Precession Angles and Geometry (زوایای تقدیم و هندسه)

**Original Notes Transcription:**
> ■ **حرف نهایی:** (Final word:)
> *(Diagram showing the fixed axis $x_3'$, body axis $x_3$, and vectors $\vec{\omega}$ and $\vec{L}$. The angle between $x_3'$ and $x_3$ is $\theta$. The angle between $x_3$ and $\vec{\omega}$ is $\alpha$.)*
> 
> We proved analytically: $\vec{L} \cdot (\vec{\omega} \times \hat{e}_3) = 0$
> $\rightarrow$ همواره در یک صفحه هستند: $\vec{L}, \vec{\omega}, x_3$
> (They are always in one plane: $\vec{L}, \vec{\omega}, x_3$)
> 
> ■ در این مرحله زاویه ی بین $\vec{L}$ و $x_3$ ($\theta$) را حساب می کنیم:
> (In this step, we calculate the angle $\theta$ between $\vec{L}$ and $x_3$:)
> 
> با محورهای جسمی (With body axes):
> $$\begin{cases} \omega_1 = 0 \\ \omega_2 = \omega \sin \alpha \\ \omega_3 = \omega \cos \alpha \end{cases} \rightarrow \begin{cases} L_1 = I_1 \omega_1 = 0 \quad (\text{since } I_1=I_2) \\ L_2 = I_2 \omega_2 = I_1 \omega_2 = I_1 \omega \sin \alpha \\ L_3 = I_3 \omega_3 = I_3 \omega \cos \alpha \end{cases}$$
> 
> از سوی دیگر داریم: (On the other hand we have:)
> $$\tan\theta = \frac{L_2}{L_3} = \frac{I_1 \omega \sin\alpha}{I_3 \omega \cos\alpha} = \frac{I_1}{I_3} \tan\alpha$$
> 
> *Boxed equation:*
> $$\tan\theta = \frac{I_1}{I_3} \tan\alpha$$
> 
> **Case 1 (Oblate top - e.g., a coin/disk):**
> If $I_1 > I_3 \rightarrow \tan\theta > \tan\alpha \rightarrow \theta > \alpha$
> *(Diagram shows the Space cone is "inside" the Body cone. Precession is in the same direction as spin).*
> 
> **Case 2 (Prolate top - e.g., a football/cigar):**
> If $I_1 < I_3 \rightarrow \tan\theta < \tan\alpha \rightarrow \theta < \alpha$
> *(Diagram shows the Space cone is "outside" the Body cone. Precession is opposite to spin).*
> 
> ■ راستگرد ، چپگرد (Right-handed, left-handed precession):
> $$\Omega = \frac{I_3 - I_1}{I_1} \omega_3$$
> - If $I_3 > I_1$, $\Omega$ and $\omega_3$ هم جهت (same direction) $\rightarrow$ Direct precession.
> - If $I_3 < I_1$, $\Omega$ and $\omega_3$ خلاف جهت (opposite direction) $\rightarrow$ Retrograde precession.

> **Elaboration:**
> The relationship between the three critical axes ($\vec{L}$, $\vec{\omega}$, and the symmetry axis $x_3$) governs the visual geometry of the tumbling top.
> 
> We align our coordinate system momentarily such that $\omega_1 = 0$. By evaluating the components of $\vec{\omega}$ and $\vec{L}$, we find a beautiful trigonometric relation: $\tan\theta = \frac{I_1}{I_3} \tan\alpha$. Here, $\alpha$ is the half-angle of the body cone, and $\theta$ is the half-angle of the spatial cone.
> 
> This equation strictly divides rigid bodies into two geometric categories:
> 1. **Oblate Tops (Flat disks, $I_1 > I_3$):** Because $\theta > \alpha$, the angular momentum vector $\vec{L}$ lies "outside" the angular velocity vector. From the perspective of the body, the precession $\Omega$ has the opposite sign to the spin $\omega_3$, causing a retrograde wobble.
> 2. **Prolate Tops (Long cylinders, $I_1 < I_3$):** Because $\theta < \alpha$, the angular momentum vector $\vec{L}$ lies "inside" the angular velocity vector. The precession $\Omega$ has the same sign as the spin $\omega_3$, causing a direct wobble.

---

## 3. Coupled Oscillations (نوسانات جفت شده)

**Original Notes Transcription:**
> ■ **نوسانات جفت شده:** (Coupled Oscillations:)
> سرآغاز نگری (Q.F.T)
> (Beginning of perspective / introduction to Q.F.T concepts)
> 
> ■ **مثال :** (Example:)
> *(Diagram showing two masses $m_1=M$ and $m_2=M$ connected in series between two rigid walls. The left wall is connected to $m_1$ by spring $K_1=K$. Mass $m_1$ is connected to $m_2$ by spring $K_{12}$. Mass $m_2$ is connected to the right wall by spring $K_2=K$. The displacements from equilibrium are $x_1$ and $x_2$).*
> 
> - **قدم ۱)** دستگاه مختصات (Step 1: Coordinate system) $\checkmark$
> - **قدم ۲)** معادلات حرکت (Step 2: Equations of motion)
> 
> *(برای راحتی طول آزاد فنرها را صفر در نظر بگیرید !)* 
> (For simplicity, assume the rest length of the springs is zero!)
> *(We assume linear restorative forces, meaning no "non-linear terms" - جملات غیرخطی).*
> 
> Writing Newton's laws for each mass:
> **I)** $M \ddot{x}_1 = -K x_1 + K_{12} (x_2 - x_1)$
> **II)** $M \ddot{x}_2 = -K x_2 + K_{12} (x_1 - x_2)$
> 
> Rearranging the terms to group variables:
> 
> *Boxed equations:*
> $$\begin{cases} M \ddot{x}_1 + (K + K_{12})x_1 - K_{12} x_2 = 0 \\ M \ddot{x}_2 + (K + K_{12})x_2 - K_{12} x_1 = 0 \end{cases}$$
> 
> دستگاه معادلات دیفرانسیل خطی مرتبه ۲ جفت شده. 
> (System of coupled second-order linear differential equations.)

> **Elaboration:**
> The lecture transitions to a brand new topic: Coupled Oscillations. This topic serves as the fundamental mechanical analog for many advanced physics concepts, including solid-state physics and Quantum Field Theory (Q.F.T), as hinted by the professor's note "سرآغاز نگری (Q.F.T)".
> 
> A classic system is introduced: two identical masses $M$ connected by three springs. The outer springs have stiffness $K$, and the central coupling spring has stiffness $K_{12}$.
> 
> When we write Newton's second law for each mass, the force on $m_1$ depends not only on its own displacement $x_1$ but also on the displacement $x_2$ of the second mass (because the middle spring stretches by $x_2 - x_1$). This results in a system of equations where the variables $x_1$ and $x_2$ are "coupled" together. We cannot solve for $x_1(t)$ without simultaneously solving for $x_2(t)$.

---

## 4. Solving Coupled Oscillations (حل معادلات نوسانات جفت شده)

**Original Notes Transcription:**
> ■ **قدم III)** حل معادلات: (Step III: Solving equations:)
> 
> با حدس زدن: (By guessing:)
> $$\begin{cases} x_1(t) = B_1 e^{+i\omega t} \\ x_2(t) = B_2 e^{+i\omega t} \end{cases} \quad (B_1, B_2 \text{ are complex numbers - عدد مختلط})$$
> 
> - من جواب بالا را در نظر می گیرم و در نهایت جزء حقیقی آنرا محاسبه می کنم. 
> (I assume the above solution and finally calculate its real part.)
> 
> Substituting the guesses into the differential equations (since $\ddot{x} = -\omega^2 x$):
> 
> $$\rightarrow \begin{cases} (-M\omega^2 + K + K_{12})B_1 - K_{12} B_2 = 0 \\ -K_{12} B_1 + (-M\omega^2 + K + K_{12})B_2 = 0 \end{cases}$$
> *(Rearranged to align $B_1$ and $B_2$).*
> 
> برای وجود جواب غیربدیهی ، باید دترمینان ضرایب صفر باشد:
> (For the existence of non-trivial solutions ($B_1, B_2 \neq 0$), the determinant of the coefficients must be zero:)
> 
> $$\begin{vmatrix} K+K_{12}-M\omega^2 & -K_{12} \\ -K_{12} & K+K_{12}-M\omega^2 \end{vmatrix} = 0$$
> 
> دو جواب دارد. (It has two solutions.)

> **Elaboration:**
> To solve linear coupled differential equations, we exploit the linearity by guessing a complex exponential solution $x(t) = B e^{i\omega t}$, knowing that the physical motion is just the real part of this complex function.
> 
> We substitute this guess into the equations. Because taking the second derivative of an exponential just pulls down a $(-\omega^2)$ factor, the differential equations instantly transform into a system of algebraic linear equations for the amplitudes $B_1$ and $B_2$.
> 
> We can write this system in matrix form. If the determinant of the coefficient matrix is non-zero, the only solution is $B_1 = B_2 = 0$ (the trivial state of no motion). For the masses to actually oscillate, the determinant must equal exactly zero.
> 
> Calculating this determinant will yield a characteristic equation (a polynomial in $\omega^2$). Because it's a $2 \times 2$ matrix, it will produce two distinct solutions for $\omega^2$. These two frequencies represent the **Normal Modes** of the coupled system—the fundamental frequencies at which both masses can oscillate in unison.
