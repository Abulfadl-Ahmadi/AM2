# Chapter 11: Dynamics of Rigid Bodies (Continued) - Lecture: May 18, 2026

> [!abstract] Navigation
> **Chapter:** [[Chapter 11 - Dynamics of Rigid Bodies]] | **Prev:** [[Note May 16, 2026]] | **Next:** [[Note May 23, 2026]] | [[Journal/Lecture Index|📚 All Lectures]]

## 1. Review and Simple Pendulum Example (مرور و مثال آونگ ساده)

**Original Notes Transcription:**
> **Timeline / Headings:**
> - **لختی دورانی** (Rotational Inertia)
> - **محورهای اصلی** (Principal Axes)
> 
> ■ **مرور:** (Review:)
> $$I_{ij} = \sum_\alpha m_\alpha \left( \delta_{ij} \sum_k x_{\alpha k}^2 - x_{i\alpha} x_{j\alpha} \right)$$
> 
> $$T_{rot} = \frac{1}{2} I_{ij} \omega_i \omega_j \equiv \frac{1}{2} \sum_i \sum_j I_{ij} \omega_i \omega_j \quad \left( A_i B^i \equiv \sum_i A_i B^i \text{ dummy index} \right)$$
> 
> $$L_i = \sum_j I_{ij} \omega_j$$
> 
> ■ **مثال ساده:** (Simple Example:)
> *(Diagram shows a pendulum consisting of a rigid massless rod of length $b$ pivoted at the origin $O$. A mass $m_2$ is located at distance $b/2$, and a mass $m_1$ is located at the end $b$. The rod makes an angle $\theta$ with the vertical axis $x_3$ (or $z$ axis). Gravity acts downwards).*
> 
> $$\vec{\tau}(\vec{N}) = \frac{d\vec{L}}{dt}$$
> $$\rightarrow \vec{\tau} = \frac{d\vec{L}}{dt} \rightarrow \text{معادله ی نیوتون در دستگاه مختصات لخت}$$
> (Newton's equation in an inertial coordinate system)
> 
> *Coordinates in fixed frame:*
> $$\begin{cases} \vec{x}_1 = 0 \hat{i} + b \sin\theta \hat{j} - b \cos\theta \hat{k} \\ \vec{x}_2 = 0 \hat{i} + \frac{b}{2} \sin\theta \hat{j} - \frac{b}{2} \cos\theta \hat{k} \end{cases}$$
> $\rightarrow \theta(t)$
> 
> $$\rightarrow I_{ij} = m_1 \left( \delta_{ij} b^2 - x_i^{(1)} x_j^{(1)} \right) + m_2 \left( \delta_{ij} \frac{b^2}{4} - x_i^{(2)} x_j^{(2)} \right)$$
> $$\rightarrow I_{ij} = I_{ij}(\theta)$$
> 
> *Boxed equation (Physics 101):*
> $$\vec{\tau}_H = I \vec{\alpha} \quad (I = \text{const.}) \rightarrow \vec{\tau}_H = I \frac{d\vec{\omega}}{dt} \quad (\text{Phys101})$$
> 
> ■ تلاش می کنیم ، تانسور لختی دورانی را در دستگاه چسبیده به جسم بدست آوریم:
> (We try to find the rotational inertia tensor in the body-fixed coordinate system:)
> $$\vec{\omega} = (0, 0, \dot{\theta})$$

> **Elaboration:**
> The lecture starts with a brief review of the Moment of Inertia Tensor $I_{ij}$, rotational kinetic energy $T_{rot}$, and angular momentum $L_i$. The Einstein summation convention (dummy indices) is briefly mentioned.
> 
> A simple example of a physical pendulum is presented: a rigid rod with two point masses, $m_2$ at the midpoint ($b/2$) and $m_1$ at the end ($b$). 
> If we attempt to solve this system using Newton's equations $\vec{\tau} = \frac{d\vec{L}}{dt}$ in a fixed (inertial) coordinate system, the positions of the masses depend on the angle $\theta(t)$. As a result, the inertia tensor components $I_{ij}$ become time-dependent functions of $\theta$, which makes the equations of motion highly complex.
> 
> In introductory physics (Physics 101), we simply used the scalar equation $\tau = I \alpha = I \frac{d\omega}{dt}$, treating $I$ as a constant. To recover a constant inertia tensor and simplify the problem in 3D rigid body dynamics, we must shift our perspective and calculate the inertia tensor in a **body-fixed coordinate system** (a frame attached to the moving body). In this frame, the mass distribution is stationary, meaning $I_{ij}$ is strictly constant.

---

## 2. Inertia Tensor in Body-Fixed Frame (تانسور لختی در دستگاه متصل به جسم)

**Original Notes Transcription:**
> *(Diagram shows the pendulum aligned with the x-axis ($x_1$) of the body-fixed coordinate system. The y-axis ($x_2$) and z-axis ($x_3$) are perpendicular).*
> 
> **مختصات جسمی:** (Body Coordinates:)
> $$\vec{x}_1 = (b, 0, 0)$$
> $$\vec{x}_2 = \left(\frac{b}{2}, 0, 0\right)$$
> *(lethal - written as a side note for the mass term $I_{11}$)*
> 
> • $I_{11} = m_1 \left( 1 \times b^2 - b^2 \right) + m_2 \left( 1 \times \frac{b^2}{4} - \frac{b^2}{4} \right) = 0$
> *(در دستگاه چسبیده به جسم گسسته ای ذرات رو اگر روی یک محور قرار بدهیم شعاع عمودشون ۰ میشه)*
> *(In a body-fixed frame, if we place discrete particles on an axis, their perpendicular radius becomes 0, assuming they are point masses $m_1, m_2$.)*
> 
> • $I_{22} = m_1 \left( 1 \times b^2 - 0 \times 0 \right) + m_2 \left( 1 \times \frac{b^2}{4} - 0 \right) = b^2 \left( m_1 + \frac{m_2}{4} \right) = I_{33}$
> 
> $$\rightarrow \{I\} = \begin{pmatrix} 0 & 0 & 0 \\ 0 & \left(m_1 + \frac{m_2}{4}\right)b^2 & 0 \\ 0 & 0 & \left(m_1 + \frac{m_2}{4}\right)b^2 \end{pmatrix} \quad \checkmark$$
> 
> • **قدم دوم : محاسبه بردار تکانه زاویه ای:** (Step two: Calculating the angular momentum vector:)
> $$\vec{L} = \{I\}\vec{\omega}$$
> 
> $$L_1 = \sum_j I_{1j} \omega_j = 0$$
> $$L_2 = \sum_j I_{2j} \omega_j = 0$$
> $$L_3 = \sum_j I_{3j} \omega_j = I_{33} \omega_3 = b^2 \left( m_1 + \frac{m_2}{4} \right) \dot{\theta}$$
> 
> *Boxed equation:*
> $$L = I \omega$$
> 
> • **قدم سوم :** (Step three:)
> *(Diagram shows the pendulum with gravitational forces $m_1 g$ and $m_2 g$ acting downwards, creating a torque).*
> $$\vec{\tau} = \sum \vec{r}_\alpha \times \vec{F}_\alpha^{ext}$$
> $$= -\left( m_1 g b \sin\theta + m_2 g \frac{b}{2} \sin\theta \right) \hat{e}_3$$
> 
> $$\vec{\tau} = \frac{d\vec{L}}{dt} \rightarrow -bg \sin\theta \left( m_1 + \frac{m_2}{2} \right) = b^2 \left( m_1 + \frac{m_2}{4} \right) \ddot{\theta}$$

> **Elaboration:**
> To solve the physical pendulum problem cleanly, we attach a coordinate frame directly to the rod, aligning the $x_1$-axis with the rod itself. In this **body-fixed frame**, the coordinates of the two masses are permanently fixed at $\vec{x}_1 = (b,0,0)$ and $\vec{x}_2 = (b/2,0,0)$.
> 
> 1. **Inertia Tensor Calculation:**
>    Since both point masses lie exactly on the $x_1$-axis, their perpendicular distance to the $x_1$-axis is zero, resulting in $I_{11} = 0$. The moments of inertia about the $x_2$ and $x_3$ axes are identical due to symmetry: $I_{22} = I_{33} = m_1 b^2 + m_2 (b/2)^2 = b^2(m_1 + m_2/4)$. Since all masses lie on an axis, all products of inertia (off-diagonal terms) are zero. The tensor is perfectly diagonal and constant over time.
> 
> 2. **Angular Momentum:**
>    The pendulum swings in a plane, meaning the rotation is purely about the $x_3$-axis. Thus, the angular velocity in the body frame is $\vec{\omega} = (0, 0, \dot{\theta})$. Multiplying this by the diagonal inertia tensor gives an angular momentum entirely along the $x_3$-axis: $L_3 = I_{33} \dot{\theta}$. We successfully recover the simple scalar relation $L = I\omega$.
> 
> 3. **Equation of Motion:**
>    We calculate the external torque due to gravity about the pivot. Equating this torque to the rate of change of angular momentum ($\tau = \frac{dL}{dt}$) yields the nonlinear differential equation governing the pendulum's motion.

---

## 3. Small Oscillations of the Pendulum (نوسانات کوچک آونگ)

**Original Notes Transcription:**
> $$\theta \ll 1 \rightarrow \ddot{\theta} + \omega_0^2 \theta = 0 \rightarrow \omega_0^2 = \frac{\left( m_1 + \frac{m_2}{2} \right)}{\left( m_1 + \frac{m_2}{4} \right)} \frac{g}{b}$$
> 
> *Boxed equation:*
> $$\rightarrow \omega_0 = \sqrt{\frac{g}{b}} \sqrt{\frac{1 + \frac{m_2}{2m_1}}{1 + \frac{m_2}{4m_1}}}$$
> 
> ■ **یادآوری:** (Reminder:)
> (I) $$\left( \frac{d\vec{Q}}{dt} \right)_{fixed} = \left( \frac{d\vec{Q}}{dt} \right)_{rot} + \vec{\omega} \times \vec{Q}$$
> $$\rightarrow \left( \frac{d\vec{\omega}}{dt} \right)_{fixed} = \left( \frac{d\vec{\omega}}{dt} \right)_{rot}$$
> 
> (II) $$\vec{\tau}_{(\text{II})} = I \vec{\alpha}_{(\text{II})}$$
> *(خطرات فیزیک ۱)* (Dangers of Physics 1)
> *(Diagram shows a small face and a heart. A box says: $\tau_i = I_i \alpha_i$)*
> *(آرزوی رسیدن به چنین معادله ای را داریم)* (We wish to reach such simple equations)
> 
> $$L_i = \sum_j I_{ij} \omega_j \rightarrow I_{ij}(t) \quad I_{i \neq j} \neq 0$$

> **Elaboration:**
> For small angles ($\theta \ll 1$), we use the small-angle approximation $\sin\theta \approx \theta$. This linearizes the differential equation into the standard form of a simple harmonic oscillator: $\ddot{\theta} + \omega_0^2 \theta = 0$. We then extract the natural angular frequency $\omega_0$ of the physical pendulum.
> 
> The professor provides an important reminder regarding rotating reference frames: the rate of change of any vector $\vec{Q}$ in a fixed frame equals its rate of change in the rotating frame plus $\vec{\omega} \times \vec{Q}$. Interestingly, if we apply this to the angular velocity vector itself ($\vec{Q} = \vec{\omega}$), the cross product $\vec{\omega} \times \vec{\omega}$ vanishes. This proves that the angular acceleration vector $\vec{\alpha} = \frac{d\vec{\omega}}{dt}$ is identical in both the fixed and the body-fixed frames.
> 
> A warning is given about the "dangers of Physics 1". In introductory physics, we comfortably use $\tau = I\alpha$. However, in full 3D dynamics, the inertia tensor often has off-diagonal components ($I_{i \neq j} \neq 0$), and if viewed from a fixed frame, these components change over time ($I_{ij}(t)$). Our ultimate goal (our "wish") is to find a special coordinate frame where the equations decouple into simple, independent equations like $\tau_i = I_i \alpha_i$.

---

## 4. Principal Axes of Inertia and Diagonalization (محورهای اصلی لختی و قطری سازی)

**Original Notes Transcription:**
> ■ **محورهای اصلی لختی:** (Principal Axes of Inertia:)
> *(فرض کنید همه ایستاده اند)* (Assume everyone is standing up - presumably referring to a classroom demonstration)
> 
> *(Diagram shows a rigid body with general axes $\hat{n}_1, \hat{n}_2, \hat{n}_3$ and a special set of axes $\tilde{n}_1, \tilde{n}_2, \tilde{n}_3$.)*
> 
> $$I_{ij} = I_i \delta_{ij} \rightarrow \{I\} = \begin{pmatrix} I_1 & 0 & 0 \\ 0 & I_2 & 0 \\ 0 & 0 & I_3 \end{pmatrix}$$
> 
> - اگر این محورهای اصلی را بیابیم، آنگاه داریم:
> (If we find these principal axes, then we have:)
> $$\begin{cases} L_i = \sum_j I_{ij} \omega_j = \sum_j I_i \delta_{ij} \omega_j = I_i \omega_i \\ T_{rot} = \frac{1}{2} \sum I_i \omega_i^2 \end{cases}$$
> 
> - نکته جالب : اگر حول یکی از این محورهای اصلی دوران کنیم:
> (Interesting point: If we rotate around one of these principal axes:)
> *(فقط حول محور اصلی)* (Only around the principal axis)
> $$\vec{L} = I \vec{\omega} \rightarrow \vec{L} = \{I\} \vec{\omega}$$
> *(به ازای یک I مناسب چنین رابطه ای درست است)* (For an appropriate I this relation is true.)
> *(Diagram shows $\vec{\omega}$ and $\vec{L}$ are parallel if rotated around a principal axis. $\vec{L} \parallel \vec{\omega}$).*
> 
> ■ **فرآیند قطری سازی:** (Diagonalization process:)
> $\vec{\omega} = (\omega_1, \omega_2, \omega_3)$
> $\vec{\omega}$ در امتداد یکی از محورهای اصلی:
> ($\vec{\omega}$ along one of the principal axes:)
> $$L_i = I \omega_i$$
> $$L_i = \sum_j I_{ij} \omega_j$$
> 
> $$\rightarrow \begin{cases} I \omega_1 = I_{11} \omega_1 + I_{12} \omega_2 + I_{13} \omega_3 \\ I \omega_2 = I_{21} \omega_1 + I_{22} \omega_2 + I_{23} \omega_3 \\ I \omega_3 = I_{31} \omega_1 + I_{32} \omega_2 + I_{33} \omega_3 \end{cases}$$
> 
> $$\rightarrow \begin{cases} (I_{11} - I) \omega_1 + I_{12} \omega_2 + I_{13} \omega_3 = 0 \\ I_{21} \omega_1 + (I_{22} - I) \omega_2 + I_{23} \omega_3 = 0 \\ I_{31} \omega_1 + I_{32} \omega_2 + (I_{33} - I) \omega_3 = 0 \end{cases}$$
> 
> برای اینکه دستگاه معادلات بالا جواب غیربدیهی (برای $\vec{\omega} \neq 0$) داشته باشد، دترمینان ضرایب باید صفر شود:
> (For the above system of equations to have a non-trivial solution (for $\vec{\omega} \neq 0$), the determinant of the coefficients must be zero:)
> 
> $$\begin{vmatrix} I_{11}-I & I_{12} & I_{13} \\ I_{21} & I_{22}-I & I_{23} \\ I_{31} & I_{32} & I_{33}-I \end{vmatrix} = 0$$
> 
> $$\det(\{I\} - I\{\mathbf{1}\}) = 0$$
> 
> بعد از حل معادله بالا، سه جواب برای $I$ می یابیم که لزوماً با هم متفاوت نیستند.
> (After solving the above equation, we find three solutions for $I$, which are not necessarily distinct.)

> **Elaboration:**
> The "Principal Axes of Inertia" represent a special body-fixed coordinate system where the inertia tensor becomes perfectly diagonal (all products of inertia vanish). If we can align our coordinate axes with these principal axes, the mathematics simplifies immensely. The angular momentum components become cleanly uncoupled: $L_1 = I_1 \omega_1$, $L_2 = I_2 \omega_2$, and $L_3 = I_3 \omega_3$.
> 
> A fascinating consequence is that if a rigid body rotates purely around one of its principal axes, the angular momentum vector $\vec{L}$ points in the exact same direction as the angular velocity vector $\vec{\omega}$. In general rotations, $\vec{L}$ and $\vec{\omega}$ are not parallel.
> 
> Finding these principal axes is equivalent to the linear algebra problem of finding the eigenvalues and eigenvectors of the inertia tensor matrix. We set up the eigenvalue equation $\vec{L} = \{I\}\vec{\omega} = I\vec{\omega}$, which leads to a homogeneous system of linear equations. For a non-trivial rotating body ($\vec{\omega} \neq 0$), the determinant of the coefficient matrix must equal zero (the characteristic equation).
> Solving this cubic characteristic equation $\det(\{I\} - I\mathbf{1}) = 0$ yields three roots ($I_1, I_2, I_3$). These are the **Principal Moments of Inertia** (the eigenvalues).

---

## 5. Properties of Principal Axes and Example of Cube (ویژگی های محورهای اصلی و مثال مکعب)

**Original Notes Transcription:**
> ■ **چند نکته ساده:** (Some simple points:)
> i) محورهای اصلی را با توجه به تقارن های جسم می توان یافت.
> (Principal axes can be found by considering the symmetries of the body.)
> 
> ii) برای اشکال ناشی از دوران (Surface of revolution) (رویه ی دوار):
> که یکی از محورهای اصلی محور دوران است، اندازه $I_2 = I_3$.
> (For surfaces of revolution, where one of the principal axes is the axis of revolution, the magnitudes are $I_2 = I_3$.)
> 
> iii) $I_1 = I_2 = I_3$ به اصطلاح فرفره کروی گفته می شود.
> (When $I_1 = I_2 = I_3$, it is called a "spherical top".)
> برای حالتی که $I_1 \neq I_2 = I_3$ فرفره متقارن (symmetric top).
> در حالتی که $I_1 \neq I_2 \neq I_3$ به اصطلاح فرفره نامتقارن (asymmetric top / rotor).
> *(Diagrams show examples of a symmetric top and a planar object).*
> 
> $$I_1 = I_2 + I_3 \quad \text{(Perpendicular axis theorem for planar objects)}$$
> 
> ■ **مثال:** برای مسأله مکعب ، محورهای اصلی و $I$ حول محورهای اصلی را بیابید:
> (Example: For the cube problem, find the principal axes and $I$ around the principal axes:)
> 
> *(Diagram of a cube with side $L$ and origin at one corner. The diagonal from the origin is drawn).*
> Let $\beta = M L^2$
> 
> $$\{I\} = \begin{pmatrix} +\frac{2}{3}\beta & -\frac{1}{4}\beta & -\frac{1}{4}\beta \\ -\frac{1}{4}\beta & +\frac{2}{3}\beta & -\frac{1}{4}\beta \\ -\frac{1}{4}\beta & -\frac{1}{4}\beta & +\frac{2}{3}\beta \end{pmatrix}$$
> 
> $$\rightarrow \det(\{I\} - I \{\mathbf{1}\}) = 0 \rightarrow I_1 = \frac{1}{6} \beta, \quad I_2 = \frac{11}{12} \beta, \quad I_3 = \frac{11}{12} \beta$$
> 
> $$\begin{vmatrix} \frac{2}{3}\beta - I & -\frac{1}{4}\beta & -\frac{1}{4}\beta \\ -\frac{1}{4}\beta & +\frac{2}{3}\beta - I & -\frac{1}{4}\beta \\ -\frac{1}{4}\beta & -\frac{1}{4}\beta & +\frac{2}{3}\beta - I \end{vmatrix} = 0$$
> 
> نکته تستی : (Test tip: ...)

> **Elaboration:**
> The lecture concludes with practical rules for identifying principal axes without doing heavy math:
> 1. **Symmetry:** If a body has an axis of symmetry, that axis is automatically a principal axis. If it has a plane of symmetry, any axis perpendicular to that plane is a principal axis.
> 2. **Surfaces of Revolution:** Objects like cylinders or cones have an infinite number of symmetry planes through their rotational axis. Therefore, the rotational axis is a principal axis, and the transverse moments of inertia are degenerate (equal): $I_2 = I_3$.
> 3. **Classification of Rigid Bodies:**
>    - **Spherical Tops:** All three principal moments are equal ($I_1 = I_2 = I_3$). Example: A uniform sphere or a uniform cube rotating about its center.
>    - **Symmetric Tops:** Two principal moments are equal ($I_1 \neq I_2 = I_3$). Example: A cylinder.
>    - **Asymmetric Tops (Rotors):** All three principal moments are distinct ($I_1 \neq I_2 \neq I_3$). Example: A rectangular block.
> 
> Finally, we revisit the uniform cube from the previous lecture (computed around a corner). By solving the determinant of its inertia tensor, we find its eigenvalues. The roots are $I_1 = \frac{1}{6}ML^2$ and a repeated root $I_2 = I_3 = \frac{11}{12}ML^2$. Because two eigenvalues are equal, the cube (when pivoted at a corner) behaves dynamically as a **symmetric top**. The principal axis corresponding to $I_1$ lies exactly along the main diagonal of the cube passing through the origin.
