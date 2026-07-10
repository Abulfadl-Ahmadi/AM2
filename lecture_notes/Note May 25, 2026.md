# Chapter 11: Dynamics of Rigid Bodies (Continued) - Lecture: May 25, 2026

> [!abstract] Navigation
> **Chapter:** [[Chapter 11 - Dynamics of Rigid Bodies]] | **Prev:** [[Note May 23, 2026]] | **Next:** [[Note May 30, 2026]] | [[Lecture Index|📚 All Lectures]]

## 1. Free Top and Euler Equations (فرفره آزاد و معادلات اویلر)

**Original Notes Transcription:**
> **Timeline / Headings:**
> - **فرفره آزاد:** (Free top:)
> 
> ■ **مرور : دستگاه لخت** (Review: Inertial frame)
> $$\vec{N} = \left(\frac{d\vec{L}}{dt}\right)_{fixed}$$
> $$\vec{L} = M \vec{R} \times \vec{V} + \vec{L}_{body}$$
> *(Diagram shows a fixed laboratory frame with origin $O$ and a center of mass frame with origin $O'$ moving with the object).*
> 
> If $\vec{F}_{inertial} (\text{خارجی}) \rightarrow \vec{N}_{inertial} = 0$ about the CM:
> 
> - اگر محور ثابت داشتیم که "فبها المراد" 
> (If we had a fixed axis, "so much the better")
> - لکن اگر محوری نداشتیم به سراغ مرکز جرم بروید ناامید نخواهید شد. کعبه آمال
> (But if we do not have an axis, go to the center of mass, you will not be disappointed. It is the Kaaba of hopes.)
> 
> $$\left(\frac{d\vec{L}}{dt}\right)_{fixed} = \left(\frac{d\vec{L}}{dt}\right)_{body} + \vec{\omega} \times \vec{L}$$
> 
> *Boxed equation:*
> $$\rightarrow \left(\frac{d\vec{L}}{dt}\right)_{body} + \vec{\omega} \times \vec{L} = \vec{N}$$
> 
> ■ فرض می کنیم ، محورهای جسمی را منطبق بر محورهای اصلی جسم در نظر می گیریم:
> (We assume the body axes are taken to coincide with the principal axes of the body:)
> 
> *Euler's Equations Box:*
> $$\begin{cases} \dot{L}_3 + \omega_1 L_2 - \omega_2 L_1 = N_3 & \rightarrow I_3 \dot{\omega}_3 - (I_1 - I_2)\omega_1 \omega_2 = N_3 \\ \dot{L}_2 + \omega_3 L_1 - \omega_1 L_3 = N_2 & \rightarrow I_2 \dot{\omega}_2 - (I_3 - I_1)\omega_3 \omega_1 = N_2 \\ \dot{L}_1 + \omega_2 L_3 - \omega_3 L_2 = N_1 & \rightarrow I_1 \dot{\omega}_1 - (I_2 - I_3)\omega_2 \omega_3 = N_1 \end{cases}$$
> 
> Using $L_i = I_i \omega_i \quad (\vec{L} = I \vec{\omega})$.
> *(Warning sign: این روابط فقط برای دوران حول محورهای اصلی برقرار است - These relations hold true only for rotation about principal axes).*
> 
> Since $I_i = \text{const}$ in the body frame:
> $\rightarrow (I_3 \omega_3)^{\cdot} + \omega_1 I_2 \omega_2 - \omega_2 I_1 \omega_1 = N_3$
> $\rightarrow I_3 \dot{\omega}_3 - (I_1 - I_2) \omega_1 \omega_2 = N_3$
> 
> *Compact Boxed Equation:*
> $$(I_i - I_j) \omega_i \omega_j - \sum_k (I_k \dot{\omega}_k - N_k) \varepsilon_{ijk} = 0 \quad (\text{برای علاقمندان - for enthusiasts})$$
> $\leadsto \omega_i(t)$ (خواسته ی مسأله ما - our problem's requirement)
> 
> ■ **نکته:** (Notes:)
> (۱) علی الاصول با داشتن $I_1, I_2, I_3$ و تعدادی شرایط اولیه دینامیک جسم صلب تعیین می شود. البته باید گشتاور نیروهای خارجی را به درستی تعیین کنیم.
> (1) In principle, having $I_1, I_2, I_3$ and some initial conditions determines the dynamics of the rigid body. Of course, we must correctly determine the torque of the external forces.
> 
> (۲) این معادلات، یک دستگاه معادلات دیفرانسیل جفت شده هستند. معادلات مرتبه اول زمانی هستند ولی به یک دلیل به راحتی حل پذیر نیستند : معادلات خطی نیستند.
> (2) These equations are a system of coupled differential equations. They are first-order in time but are not easily solvable for one reason: they are non-linear equations.

> **Elaboration:**
> The lecture continues the discussion of rigid body dynamics, focusing on the "Free Top"—a rigid body subject to zero net torque ($\vec{N} = 0$).
> 
> The professor emphasizes the importance of the Center of Mass (CM). If a body has a fixed pivot (like a pendulum), we calculate torques about that pivot. However, if the body is completely free (like a thrown football or a spacecraft), we should ALWAYS place our coordinate origin at the CM. The CM is referred to as the "Kaaba of hopes" because calculating angular momentum and torque about the CM structurally decouples the translational motion from the rotational motion.
> 
> We rewrite Newton's rotational law using the rotating frame derivative operator. By aligning our body-fixed frame with the Principal Axes of the body, the inertia tensor becomes diagonal ($I_1, I_2, I_3$ are constant scalars), yielding the famous **Euler Equations**. 
> 
> A warning is provided: Euler's equations in this simple form *only* apply when the axes are principal axes. Furthermore, while the equations are only first-order differential equations in $\vec{\omega}$, they contain non-linear quadratic terms (like $\omega_1 \omega_2$). This non-linearity is what makes 3D rotational dynamics notoriously difficult to solve analytically, leading to chaotic behavior in asymmetric bodies (like the Dzhanibekov effect).

---

## 2. Example: Unbalanced Rotating Masses (مثال: جرم های در حال دوران نامتوازن)

**Original Notes Transcription:**
> ■ **مثال:** (Example:)
> *(Diagram showing a massless rigid rod with two masses $m_1$ and $m_2$ at distances $r_1$ and $r_2$ from the origin $O$ (the CM). The rod is tilted at an angle $\alpha$ relative to the vertical axis $\hat{e}_3$. The system rotates with angular velocity $\vec{\omega}$ about the vertical axis).*
> 
> In the fixed frame: $\vec{L} = \sum_\alpha m_\alpha \vec{r}_\alpha \times \vec{v}_\alpha$ does not point purely along $\hat{e}_3$.
> 
> Let's analyze in the body frame, choosing the rod as an axis.
> $\rightarrow$ آنگاه محورهای اصلی به عنوان محورهای جسمی (then principal axes as body axes) $\rightarrow L_i = I_i \omega_i$
> 
> The angular velocity vector in the body frame components:
> $$\vec{\omega} = (0, \omega \sin\alpha, \omega \cos\alpha)$$
> 
> For a thin rod, $I_3 = 0$ (moment of inertia about its own axis) and the transverse moments are equal $(I_1 = I_2)$:
> $$L_1 = 0, \quad L_2 = (m_1 r_1^2 + m_2 r_2^2) \omega \sin\alpha, \quad L_3 = 0$$
> 
> - لذا این مثال با معادلات اویلر جاگذاری کن (فرض کنید $N=0$):
> (So insert this example into Euler's equations (assume $N=0$):)
> 
> $$N_1 = I_1 \dot{\omega}_1 - (I_2 - I_3)\omega_2 \omega_3 = 0 - I_2 (\omega \sin\alpha)(\omega \cos\alpha) = -(m_1 r_1^2 + m_2 r_2^2)\omega^2 \sin\alpha \cos\alpha \quad \checkmark$$
> $$N_2 = I_2 \dot{\omega}_2 - (I_3 - I_1)\omega_3 \omega_1 = 0 - 0 = 0$$
> $$N_3 = I_3 \dot{\omega}_3 - (I_1 - I_2)\omega_1 \omega_2 = 0 - 0 = 0$$
> 
> - محاسبه برای درک بهتر : (Calculation to show a point:)
> $$\vec{L} = \hat{e}_2 (m_1 r_1^2 \sin\alpha + m_2 r_2^2 \sin\alpha) \omega$$
> $$\frac{d\vec{L}}{dt} = \vec{\omega} \times \vec{L} = (m_1 r_1^2 + m_2 r_2^2) \omega \sin\alpha \, (\vec{\omega} \times \hat{e}_2)$$
> Since $\vec{\omega} = \omega \sin\alpha \hat{e}_2 + \omega \cos\alpha \hat{e}_3$, the cross product is:
> $$(\omega \sin\alpha \hat{e}_2 + \omega \cos\alpha \hat{e}_3) \times \hat{e}_2 = -\omega \cos\alpha \hat{e}_1$$
> $$\rightarrow \frac{d\vec{L}}{dt} = -(m_1 r_1^2 + m_2 r_2^2)\omega^2 \sin\alpha \cos\alpha \, \hat{e}_1$$
> *(Matches $N_1$ calculated from Euler equations).*

> **Elaboration:**
> To demonstrate the power of Euler's equations, we revisit the unbalanced rotating masses problem. A rod with two masses rotates about an axis that is not aligned with the rod itself (tilted by angle $\alpha$).
> 
> If we analyze this using the principal axes attached to the rod, the inertia tensor is diagonal ($I_3 = 0, I_1 = I_2$). However, the angular velocity vector $\vec{\omega}$ is not aligned with the principal axes; it has components along both $\hat{e}_2$ and $\hat{e}_3$. 
> 
> We plug these constant $\omega$ components into Euler's equations. Even though $\dot{\omega}_i = 0$ (the rotation rate is constant), the non-linear cross terms $(I_2 - I_3)\omega_2 \omega_3$ survive. This instantly tells us that $N_1$ is non-zero. A constant torque must be applied continuously along the $\hat{e}_1$ axis to keep this unbalanced system rotating at a constant angular velocity. 
> A direct vector calculation of $\frac{d\vec{L}}{dt} = \vec{\omega} \times \vec{L}$ confirms Euler's prediction perfectly.

---

## 3. The Free Symmetric Top (فرفره ی متقارن آزاد)

**Original Notes Transcription:**
> ■ **فرفره ی متقارن آزاد :** (Free symmetric top:)
> *(Diagram of a coin or disk spinning with angular velocity $\vec{\omega}$ not aligned with its symmetry axis).*
> 
> A symmetric top has two equal principal moments of inertia:
> $$I_1 = I_2 \neq I_3$$
> 
> Since it is free, there are no external torques ($\vec{N} = 0$). Euler's equations become:
> $$I_1 \dot{\omega}_1 - (I_2 - I_3)\omega_2 \omega_3 = 0$$
> $$I_2 \dot{\omega}_2 - (I_3 - I_1)\omega_1 \omega_3 = 0$$
> $$I_3 \dot{\omega}_3 - (I_1 - I_2)\omega_1 \omega_2 = 0$$
> 
> Since $I_1 = I_2$, the third equation simplifies immediately:
> $$I_3 \dot{\omega}_3 - (0)\omega_1 \omega_2 = 0 \rightarrow I_3 \dot{\omega}_3 = 0 \rightarrow \dot{\omega}_3 = 0$$
> 
> *Boxed equation:*
> $$\omega_3 = \text{const}$$
> 
> Substitute $I_2 = I_1$ into the first two equations:
> $$(1) \quad I_1 \dot{\omega}_1 - (I_1 - I_3)\omega_3 \omega_2 = 0$$
> $$(2) \quad I_1 \dot{\omega}_2 - (I_3 - I_1)\omega_3 \omega_1 = 0$$
> 
> Rearranging:
> $$\dot{\omega}_1 = - \left( \frac{I_3 - I_1}{I_1} \omega_3 \right) \omega_2$$
> $$\dot{\omega}_2 = + \left( \frac{I_3 - I_1}{I_1} \omega_3 \right) \omega_1$$
> 
> Let's define a constant precession frequency $\Omega$:
> $$\Omega = \frac{I_3 - I_1}{I_1} \omega_3$$
> 
> با این تعریف معادلات جفت شده خطی مرتبه اول زیر برای $\omega_1, \omega_2$ می یابیم:
> (With this definition, we find the following coupled linear first-order equations for $\omega_1, \omega_2$:)
> 
> $$\begin{cases} \dot{\omega}_1 = - \Omega \omega_2 \\ \dot{\omega}_2 = + \Omega \omega_1 \end{cases}$$

> **Elaboration:**
> We now solve the case of a "Free Symmetric Top", such as a frisbee or a coin tumbling through the air in zero gravity. Because it is symmetric ($I_1 = I_2$), the non-linear Euler equations magically simplify.
> 
> The third Euler equation shows that the angular velocity component along the symmetry axis ($\omega_3$) is absolutely constant. This is a crucial conservation law. 
> 
> Because $\omega_3$ is constant, the non-linear terms in the first two Euler equations become linear. By defining a new constant frequency $\Omega = \omega_3(I_3 - I_1)/I_1$, the dynamics reduce to a pair of simple, linear, coupled differential equations representing coupled harmonic oscillators.

---

## 4. Solving the Equations of Motion (حل معادلات حرکت)

**Original Notes Transcription:**
> ■ **راه حل اول :** (First solution using complex variables:)
> Let $\eta \equiv \omega_1 + i \omega_2$
> $$\dot{\eta} = \dot{\omega}_1 + i \dot{\omega}_2 = -\Omega \omega_2 + i \Omega \omega_1 = i\Omega(\omega_1 + i\omega_2) = i\Omega \eta$$
> $$\dot{\eta} = i\Omega \eta \rightarrow \eta(t) = A e^{i\Omega t}$$
> Using Euler's formula $e^{i\Omega t} = \cos\Omega t + i \sin\Omega t$:
> 
> *Boxed equations:*
> $$\begin{cases} \omega_1 = A \cos \Omega t \\ \omega_2 = A \sin \Omega t \end{cases}$$
> 
> ■ **راه حل دوم :** (Second solution using substitution:)
> Differentiate the first equation: $\ddot{\omega}_1 = -\Omega \dot{\omega}_2$
> Substitute the second equation $\dot{\omega}_2 = \Omega \omega_1$:
> $$\ddot{\omega}_1 = -\Omega (\Omega \omega_1) \rightarrow \ddot{\omega}_1 + \Omega^2 \omega_1 = 0$$
> This is a simple harmonic oscillator. The solution is:
> $$\omega_1 = A \cos(\Omega t + \phi)$$
> If we choose the initial time such that $\phi = 0$ (با انتخاب):
> $$\omega_1 = A \cos \Omega t$$
> Then use $\dot{\omega}_1$ to find $\omega_2$:
> $$\omega_2 = \frac{-\dot{\omega}_1}{\Omega} = \frac{-(-A\Omega \sin\Omega t)}{\Omega} = A \sin \Omega t$$
> 
> ■ پس با انتخاب مناسب شرایط اولیه داریم : 
> (So with an appropriate choice of initial conditions we have:)
> $$\begin{cases} \omega_1 = A \cos \Omega t \\ \omega_2 = A \sin \Omega t \\ \omega_3 = \text{const} \end{cases}$$
> 
> ■ پس درباره اندازه سرعت زاویه ای داریم : 
> (So regarding the magnitude of the angular velocity vector we have:)
> $$|\vec{\omega}| \equiv \omega = (\omega_1^2 + \omega_2^2 + \omega_3^2)^{1/2} = (A^2 \cos^2\Omega t + A^2 \sin^2\Omega t + \omega_3^2)^{1/2}$$
> $$|\vec{\omega}| = (A^2 + \omega_3^2)^{1/2} = \text{const}$$

> **Elaboration:**
> The coupled differential equations $\dot{\omega}_1 = -\Omega \omega_2$ and $\dot{\omega}_2 = \Omega \omega_1$ can be solved using two methods. The elegant method combines $\omega_1$ and $\omega_2$ into a single complex variable $\eta = \omega_1 + i\omega_2$. The resulting equation $\dot{\eta} = i\Omega \eta$ integrates immediately to a complex exponential, yielding sines and cosines.
> 
> The second method uses standard substitution to create a second-order differential equation, revealing that both $\omega_1$ and $\omega_2$ undergo simple harmonic oscillation with frequency $\Omega$.
> 
> The result shows that the magnitude of the total angular velocity vector $|\vec{\omega}|$ is strictly constant.

---

## 5. Description of Motion and Precession (توصیف حرکت و تقدیم)

**Original Notes Transcription:**
> ■ پس روی محورهای جسمی داریم : 
> (So on the body-fixed axes we have:)
> $$\Omega = \left| \frac{I_3 - I_1}{I_1} \omega_3 \right|$$
> *(Diagram showing the body axes (1,2,3). The vector $\vec{\omega}$ rotates around the $\hat{e}_3$ axis, tracing out a cone known as the "Body Cone").*
> 
> ■ **توصیف حرکت فرفره متقارن :** (Description of the motion of a symmetric top:)
> 
> (۱) تکانه زاویه ای کل به صورت برداری ثابت است :
> (1. The total angular momentum is a constant vector:)
> $\vec{L} = \text{const}$ (به عنوان یک شرط اولیه داده می شود - Given as an initial condition).
> *(Diagram showing a fixed spatial axis $x_3'$ aligned with the constant vector $\vec{L}$).*
> 
> (۲) اگر جسم منفرد (ایزوله) است ، انرژی جنبشی دورانی آن ثابت است:
> (2. If the body is isolated, its rotational kinetic energy is constant:)
> $$T_{rot} = \frac{1}{2} \vec{\omega} \cdot \vec{L} = \text{const}$$
> $\rightarrow$ زاویه بین $\vec{\omega}$ و $\vec{L}$ باید ثابت باشد.
> (The angle between the angular velocity $\vec{\omega}$ and angular momentum $\vec{L}$ must be constant.)
> 
> (۳) از طرف دیگری می دانیم که $\vec{\omega}$ حول محور $x_3$ جسمی نیز در حال دوران است.
> (3. On the other hand, we know that $\vec{\omega}$ is also rotating around the body axis $x_3$.)
> 
> *(Diagram shows the Space Cone and Body Cone. The vector $\vec{\omega}$ lies exactly between the symmetry axis $\hat{e}_3$ and the fixed angular momentum vector $\vec{L}$. The body cone rolls without slipping on the space cone).*
> 
> ■ چک تحلیلی: (Analytical check to prove $\vec{L}, \vec{\omega}$, and $\hat{e}_3$ are coplanar:)
> We check the scalar triple product $\vec{L} \cdot (\vec{\omega} \times \hat{e}_3)$:
> $$\vec{\omega} \times \hat{e}_3 = (\omega_1 \hat{e}_1 + \omega_2 \hat{e}_2 + \omega_3 \hat{e}_3) \times \hat{e}_3 = \omega_2 \hat{e}_1 - \omega_1 \hat{e}_2$$
> 
> $$\vec{L} \cdot (\vec{\omega} \times \hat{e}_3) = (I_1 \omega_1 \hat{e}_1 + I_2 \omega_2 \hat{e}_2 + I_3 \omega_3 \hat{e}_3) \cdot (\omega_2 \hat{e}_1 - \omega_1 \hat{e}_2)$$
> $$= I_1 \omega_1 \omega_2 - I_2 \omega_1 \omega_2$$
> 
> Since it's a symmetric top ($I_1 = I_2$):
> $$\vec{L} \cdot (\vec{\omega} \times \hat{e}_3) = 0 \quad \checkmark$$
> *(This proves that $\vec{L}, \vec{\omega}$, and the symmetry axis $\hat{e}_3$ always lie in the same flat plane).*

> **Elaboration:**
> The complete motion of a free symmetric top is a beautiful geometric ballet involving two cones. 
> 
> From an observer sitting ON the rotating body (body frame), the angular velocity vector $\vec{\omega}$ appears to rotate around the symmetry axis $\hat{e}_3$ at the precession rate $\Omega$. This traces out the **Body Cone**.
> 
> From a stationary observer in the laboratory (space frame), the angular momentum vector $\vec{L}$ is absolutely fixed in space (due to zero external torque). The kinetic energy $T = \frac{1}{2} \vec{\omega} \cdot \vec{L}$ is also constant, forcing the angle between $\vec{\omega}$ and $\vec{L}$ to be constant. Thus, in the space frame, $\vec{\omega}$ rotates around the fixed $\vec{L}$ vector, tracing out the **Space Cone**.
> 
> We analytically prove that $\vec{L}, \vec{\omega}$, and the symmetry axis $\hat{e}_3$ are strictly coplanar. Consequently, the actual motion of the body can be perfectly visualized as the Body Cone rolling without slipping on the outside (or inside) of the Space Cone.
