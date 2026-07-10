# Chapter 11: Dynamics of Rigid Bodies (Continued) - Lecture: May 16, 2026

> [!abstract] Navigation
> **Chapter:** [[Chapter 11 - Dynamics of Rigid Bodies]] | **Prev:** [[Note May 11, 2026]] | **Next:** [[Note May 18, 2026]] | [[Lecture Index|📚 All Lectures]]

## 1. Rotational Kinetic Energy and the Inertia Tensor (انرژی جنبشی دورانی و تانسور لختی)

**Original Notes Transcription:**
> **Timeline:** 14-15 May (China) $\rightarrow$ Weekend $\rightarrow$ 14 June (World Cup) $\rightarrow$ 19 July (25 days / 2 weeks)
> 
> - **تانسور لختی دورانی** (Rotational Inertia Tensor)
> - **انرژی جنبشی صلب** (Kinetic Energy of a Rigid Body)
> - **تکانه زاویه ای** (Angular Momentum)
> - **محورهای اصلی** (Principal Axes)
> 
> ■ **مرور:** (Review:)
> **(I) separation of kinetic energy:**
> $$T = T_{trans} + T_{rot}$$
> *برای انتخاب مبدا (مرکز جرم):* (By choosing the origin at the Center of Mass:)
> $$T_{transl} = \frac{1}{2} M V^2$$
> $$T_{rot} = \frac{1}{2} \sum_\alpha m_\alpha (\vec{\omega} \times \vec{r}_\alpha)^2$$
> *(Diagram shows coordinate systems: origin $O'$ (fixed), origin $O$ (moving CM frame), position vector $\vec{R}$ between them, $\vec{r}'$ in fixed, $\vec{r}$ in CM frame. $\vec{V} = \frac{d\vec{R}}{dt}$.)*
> $\rightarrow$ **Physics 101**
> 
> **(II) Moment of Inertia Tensor derivation:**
> $$T_{rot} = \frac{1}{2} \sum_\alpha m_\alpha (\vec{\omega} \times \vec{r}_\alpha)^2 \rightarrow T_{rot} = \frac{1}{2} \sum_{ij} I_{ij} \omega_i \omega_j$$
> $\alpha$: شماره ذره (particle number)
> $i, j, k \in [1, 2, 3]$
> 
> **Matrix Representation:**
> $$I_{ij} = \begin{bmatrix}
> \sum_\alpha m_\alpha (x_{\alpha 2}^2 + x_{\alpha 3}^2) & -\sum_\alpha m_\alpha x_{\alpha 1} x_{\alpha 2} & -\sum_\alpha m_\alpha x_{\alpha 1} x_{\alpha 3} \\
> -\sum_\alpha m_\alpha x_{\alpha 2} x_{\alpha 1} & \sum_\alpha m_\alpha (x_{\alpha 1}^2 + x_{\alpha 3}^2) & -\sum_\alpha m_\alpha x_{\alpha 2} x_{\alpha 3} \\
> -\sum_\alpha m_\alpha x_{\alpha 3} x_{\alpha 1} & -\sum_\alpha m_\alpha x_{\alpha 3} x_{\alpha 2} & \sum_\alpha m_\alpha (x_{\alpha 1}^2 + x_{\alpha 2}^2)
> \end{bmatrix}$$
> *(⚠️ Notice the negative sign for off-diagonal elements)*
> *(Diagram shows a particle $P$ at $(x_1, x_2, x_3)$, illustrating that its distance squared to axis 1 is $x_2^2 + x_3^2$).*
> 
> **Tensor Properties:**
> $$I_{ij} = I_{ji} \quad \text{since } x_i x_j = x_j x_i \quad \checkmark$$
> 
> 1) **ماتریس متقارن** ($I_{ij} = I_{ji}$) (Symmetric matrix)
> 2) **این تانسور دارای ۶ مؤلفه مستقل است:** [۳ تا روی قطر، ۳ تا خارج قطر]
>    (This tensor has 6 independent components: [3 diagonal, 3 off-diagonal])
> 3) **$I_{ij}^{tot} = \sum I_{ij}^{(1)}$ (نسبت به جمع خطی است):**
>    (It is linear with respect to addition: $\sum_\alpha \rightarrow \sum_{\alpha_1} + \sum_{\alpha_2} \rightarrow \dots$)
> 4) **Continuous limit formulation:**
>    $$I_{ij} = \int_V \rho(\vec{r}) \left( \delta_{ij} \sum_k x_k^2 - x_i x_j \right) dV$$
>    *(where $\int_V \leftrightarrow \sum_\alpha$ and $\rho(\vec{r}) dV \leftrightarrow m_\alpha$)*
> 5) **ماتریس قطری می شود و دارای مقادیر ویژه مثبت است.**
>    (The matrix can be diagonalized and has positive eigenvalues.)

> **Elaboration:**
> The lecture begins with a review of rigid body kinetic energy. Under the choice of the Center of Mass (CM) as the origin, the kinetic energy splits cleanly into translational motion of the CM and rotational motion around the CM ($T = T_{trans} + T_{rot}$).
> 
> We expand the rotational kinetic energy component $T_{rot}$ into a matrix form using the Moment of Inertia Tensor $I_{ij}$:
> $$ T_{rot} = \frac{1}{2} \sum_{ij} I_{ij} \omega_i \omega_j $$
> 
> 1. **Diagonal Elements (Moments of Inertia):** 
>    The diagonal elements $I_{ii}$ represent the traditional moment of inertia about axis $i$. For example, $I_{11} = \sum m_\alpha (x_{\alpha 2}^2 + x_{\alpha 3}^2)$ sums the mass multiplied by the perpendicular distance squared of each particle to the 1-axis.
> 
> 2. **Off-Diagonal Elements (Products of Inertia):**
>    The off-diagonal elements $I_{ij} = -\sum m_\alpha x_i x_j$ are defined with a negative sign. They represent the asymmetry of the mass distribution relative to the coordinate planes.
> 
> 3. **Mathematical Properties:**
>    - **Symmetry:** $I_{ij} = I_{ji}$, meaning the tensor is a symmetric $3 \times 3$ matrix. This reduces the number of independent components to 6.
>    - **Linearity:** The total inertia tensor of a composite body is simply the sum of the tensors of its parts.
>    - **Continuous Bodies:** For continuous mass distributions, we replace the summation over discrete masses with an volume integral: $dm = \rho(\vec{r}) dV$.
>    - **Diagonalizability:** Being a symmetric real matrix, the inertia tensor can always be diagonalized. The eigenvectors of this matrix define the **Principal Axes of Inertia**, and the corresponding eigenvalues are the **Principal Moments of Inertia** (which are strictly positive for physical 3D bodies).

---

## 2. Example: Inertia Tensor of a Uniform Cube (مثال: تانسور لختی مکعب یکنواخت)

**Original Notes Transcription:**
> ■ **مثال:** تانسور لختی یک مکعب به جرم $M$ (یکنواخت) و طول ضلع $L$ را محاسبه کنید. این تانسور را برای یک مبدأ منطبق بر یکی از رئوس مکعب حساب کنید. محورهای مختصات را منطبق بر یال های عبوری از آن رأس قرار دهید.
> *(Example: Calculate the inertia tensor of a uniform cube of mass $M$ and side length $L$. Calculate this tensor for an origin coinciding with one of the vertices of the cube. Align the coordinate axes with the edges passing through that vertex.)*
> 
> *(Diagram shows a cube with one vertex at the origin, with axes 1 (x), 2 (y), 3 (z). An element $dV = dxdydz$ is shown inside).*
> 
> **(I) Diagonal components ($I_{11} = I_{22} = I_{33}$):**
> $$I_{11} = \int_V \rho(\vec{r}) [y^2 + z^2] dV \quad \text{where } \rho = \rho_0$$
> $$I_{11} = \rho_0 \int_0^L dx \int_0^L dy \int_0^L dz [y^2 + z^2] = \rho_0 L \int_0^L dy \int_0^L dz [y^2 + z^2]$$
> $$= \rho_0 L \int_0^L dy \left[ y^2 z \Big|_0^L + \frac{z^3}{3} \Big|_0^L \right] = \rho_0 L \int_0^L dy \left[ y^2 L + \frac{L^3}{3} \right]$$
> $$= \rho_0 L \left[ \frac{y^3}{3} L \Big|_0^L + \frac{L^3}{3} y \Big|_0^L \right] = \rho_0 L \left[ \frac{L^4}{3} + \frac{L^4}{3} \right] = \rho_0 L \times \frac{2 L^4}{3}$$
> $$= (\rho_0 L^3) \times \frac{2 L^2}{3} = \frac{2}{3} M L^2 \quad (\text{since } M = \rho_0 L^3)$$
> 
> *Boxed equation:*
> $$I_{11} = I_{22} = I_{33} = \frac{2}{3} M L^2$$
> 
> **(II) Off-diagonal components ($I_{12} = I_{13} = I_{23}$):**
> $$I_{12} = -\int_V \rho(\vec{r}) xy dV$$
> $$I_{12} = -\rho_0 \int_0^L dx \int_0^L dy \int_0^L dz (xy) = -\rho_0 L \int_0^L x dx \int_0^L y dy$$
> $$= -\rho_0 L \times \frac{L^2}{2} \times \frac{L^2}{2} = -\frac{1}{4} (\rho_0 L^3) L^2 = -\frac{1}{4} M L^2$$
> 
> *Boxed equation:*
> $$I_{12} = I_{13} = I_{23} = -\frac{1}{4} M L^2$$

> **Elaboration:**
> We calculate the Moment of Inertia Tensor for a uniform solid cube of mass $M$ and side length $L$. The coordinate system is set up with the origin at one corner of the cube, with the axes aligned along the three intersecting edges.
> 
> 1. **Moments of Inertia (Diagonal):**
>    Due to the symmetry of the cube, the moments of inertia about the three coordinate axes are equal: $I_{11} = I_{22} = I_{33}$.
>    Evaluating $I_{11}$:
>    $$ I_{11} = \rho_0 \int_0^L dx \int_0^L dy \int_0^L dz (y^2 + z^2) $$
>    Integrating over $x$ gives a factor of $L$. The remaining double integral evaluates to $\frac{2}{3}L^5$. Using the total mass relation $M = \rho_0 L^3$, we find:
>    $$ I_{11} = I_{22} = I_{33} = \frac{2}{3} M L^2 $$
> 
> 2. **Products of Inertia (Off-Diagonal):**
>    Similarly, by symmetry, the products of inertia are all equal: $I_{12} = I_{13} = I_{23}$.
>    Evaluating $I_{12}$:
>    $$ I_{12} = -\rho_0 \int_0^L dx \int_0^L dy \int_0^L dz (xy) = -\rho_0 L \left( \int_0^L x dx \right) \left( \int_0^L y dy \right) = -\rho_0 L \left(\frac{L^2}{2}\right)\left(\frac{L^2}{2}\right) = -\frac{1}{4} M L^2 $$
> 
> Consequently, the full inertia tensor matrix for the cube about one of its corners is:
> $$ I = M L^2 \begin{bmatrix}
> 2/3 & -1/4 & -1/4 \\
> -1/4 & 2/3 & -1/4 \\
> -1/4 & -1/4 & 2/3
> \end{bmatrix} $$

---

## 3. Total Angular Momentum of a Rigid Body (محاسبه تکانه زاویه ای کل)

**Original Notes Transcription:**
> ■ **محاسبه تکانه زاویه ای:** (Calculating angular momentum:)
> $$\vec{L} = \sum_\alpha \vec{r}_\alpha \times \vec{p}_\alpha \quad (\text{تعریف تکانه زاویه ای کل})$$
> 
> • **یادآوری:** $\vec{\tau} = \frac{d\vec{L}}{dt}$ ، یا نسبت به مبدا ثابت (لخت) یا CM.
> (• Reminder: $\vec{\tau} = \frac{d\vec{L}}{dt}$, either relative to a fixed (inertial) origin or relative to the CM.)
> 
> 1) *فرض کنید نسبت به دستگاه، مبدأ ساکن نوشته شده است.*
>    (1. Assume it is written relative to a frame where the origin is stationary.)
> 2) *این رابطه را برای یک جسم صلب می نویسیم:*
>    (2. We write this relation for a rigid body:)
>    $$\vec{p}_\alpha = m_\alpha \vec{v}_\alpha = m_\alpha \vec{\omega} \times \vec{r}_\alpha$$
>    *(که مستقل از $\alpha$ است)* (where $\vec{\omega}$ is independent of the particle index $\alpha$)
> 
> $$\rightarrow \vec{L} = \sum_\alpha m_\alpha \vec{r}_\alpha \times \vec{v}_\alpha = \sum_\alpha m_\alpha \vec{r}_\alpha \times (\vec{\omega} \times \vec{r}_\alpha)$$
> 
> *یادآوری:*
> $$\vec{A} \times (\vec{B} \times \vec{C}) = \vec{B}(\vec{A} \cdot \vec{C}) - \vec{C}(\vec{A} \cdot \vec{B})$$
> $$r_\alpha \equiv |\vec{r}_\alpha|$$
> 
> $$\rightarrow \vec{L} = \sum_\alpha m_\alpha \left[ \vec{\omega} r_\alpha^2 - \vec{r}_\alpha (\vec{r}_\alpha \cdot \vec{\omega}) \right]$$
> 
> *حال این رابطه را مولفه به مولفه می نویسیم:*
> (Now we write this relation component by component:)
> $$\rightarrow L_i = \sum_\alpha m_\alpha \left[ \omega_i \sum_k x_{\alpha k}^2 - x_{\alpha i} \sum_j x_{\alpha j} \omega_j \right]$$
> *(Using $\omega_i = \sum_j \delta_{ij} \omega_j$)*
> 
> $$L_i = \sum_j \omega_j \left[ \sum_\alpha m_\alpha \left( \delta_{ij} \sum_k x_{\alpha k}^2 - x_{\alpha i} x_{\alpha j} \right) \right] = \sum_j I_{ij} \omega_j$$
> 
> *Boxed equations:*
> $$\rightarrow L_i = \sum_j I_{ij} \omega_j \quad \rightarrow \vec{L} = \{I\}\vec{\omega}$$
> 
> $$T_{rot} = \frac{1}{2} \vec{\omega}^T \{I\}\vec{\omega} \quad (\text{عیدانه})$$

> **Elaboration:**
> We derive the total angular momentum $\vec{L}$ of a rigid body rotating with angular velocity $\vec{\omega}$ around a fixed origin (or center of mass).
> 
> 1. **Velocity Substitution:**
>    Since every point $\alpha$ of the rigid body has velocity $\vec{v}_\alpha = \vec{\omega} \times \vec{r}_\alpha$ (where the angular velocity vector $\vec{\omega}$ is identical for all points), the angular momentum is:
>    $$ \vec{L} = \sum_\alpha m_\alpha \vec{r}_\alpha \times (\vec{\omega} \times \vec{r}_\alpha) $$
> 
> 2. **Vector Expansion:**
>    Using the triple cross product expansion $\vec{A} \times (\vec{B} \times \vec{C}) = \vec{B}(\vec{A} \cdot \vec{C}) - \vec{C}(\vec{A} \cdot \vec{B})$, we expand:
>    $$ \vec{L} = \sum_\alpha m_\alpha \left[ \vec{\omega} r_\alpha^2 - \vec{r}_\alpha (\vec{r}_\alpha \cdot \vec{\omega}) \right] $$
> 
> 3. **Component Expression:**
>    Writing the $i$-th component $L_i$:
>    $$ L_i = \sum_\alpha m_\alpha \left[ \omega_i r_\alpha^2 - x_i (\vec{r} \cdot \vec{\omega}) \right] = \sum_\alpha m_\alpha \left[ \left(\sum_j \delta_{ij} \omega_j\right) \left(\sum_k x_{\alpha k}^2\right) - x_{\alpha i} \left(\sum_j x_{\alpha j} \omega_j\right) \right] $$
>    Factoring out the angular velocity components $\omega_j$:
>    $$ L_i = \sum_j \omega_j \left[ \sum_\alpha m_\alpha \left( \delta_{ij} \sum_k x_{\alpha k}^2 - x_{\alpha i} x_{\alpha j} \right) \right] = \sum_j I_{ij} \omega_j $$
> 
> This matches the definition of the Moment of Inertia Tensor $I_{ij}$. In matrix form:
> $$ \vec{L} = \{I\} \vec{\omega} $$
> 
> This matrix multiplication highlights that, in general, **the angular momentum vector $\vec{L}$ is not parallel to the angular velocity vector $\vec{\omega}$**. They are only parallel if the rotation axis is aligned with one of the Principal Axes of the body.
> 
> Additionally, the rotational kinetic energy can be elegantly written in matrix notation as:
> $$ T_{rot} = \frac{1}{2} \vec{\omega}^T \{I\} \vec{\omega} $$

---

## 4. Application: Two-Mass Rotating System (مثال راهگشا: سیستم دو جرمی دورانی)

**Original Notes Transcription:**
> ■ **مثال راهگشا:** (An illuminating example:)
> *(Diagram shows a system of two masses $m_1$ and $m_2$ attached to a rotating shaft. The shaft rotates with angular velocity $\vec{\omega}$ along axis 1. Axis 2 is horizontal to the left, Axis 3 is horizontal to the right).*
> 
> $$|\vec{L}| = |\vec{L}_1| + |\vec{L}_2| = m_1 r_1^2 \sin\theta \omega + m_2 r_2^2 \sin\theta \omega$$
> *جهت $\vec{L}$ روی نمودار مشخص شده است.* (The direction of $\vec{L}$ is shown on the diagram.)
> 
> **Cartesian coordinates in terms of rotation angle:**
> $$\begin{cases} x_1 = r_1 \cos\theta \\ y_1 = r_1 \sin\theta \cos\omega t \\ z_1 = r_1 \sin\theta \sin\omega t \end{cases}$$
> $$\begin{cases} x_2 = -r_2 \cos\theta \\ y_2 = -r_2 \sin\theta \cos\omega t \\ z_2 = -r_2 \sin\theta \sin\omega t \end{cases}$$
> 
> ■ **محاسبه $\vec{L}$ از طریق استفاده از رابطه $\vec{L} = \{I\}\vec{\omega}$:**
> (Calculating $\vec{L}$ by using the relation $\vec{L} = \{I\}\vec{\omega}$:)
> $$I_{11} = \sum_\alpha m_\alpha (y_\alpha^2 + z_\alpha^2) = m_1 (r_1 \sin\theta)^2 + m_2 (r_2 \sin\theta)^2$$
> 
> $$I_{22} = \sum_\alpha m_\alpha (x_\alpha^2 + z_\alpha^2) = m_1 ( \dots \rightarrow \text{کارهای تکراری} ) + m_2 ( \dots \text{کارهای تکراری} )$$
> 
> $$I_{12} = -\sum_\alpha m_\alpha x_{\alpha 1} x_{\alpha 2} = m_1 ( \dots ) + m_2 ( \dots )$$

> **Elaboration:**
> We analyze a classic asymmetric system: two masses $m_1$ and $m_2$ fixed to a rigid rod of length $r_1 + r_2$ at an angle $\theta$ relative to a vertical rotating shaft (axis 1).
> 
> 1. **Direct Calculation:**
>    If we calculate the angular momentum directly, each mass travels in a horizontal circle of radius $R_i = r_i \sin\theta$ with speed $v_i = r_i \sin\theta \omega$.
>    - The magnitude of each angular momentum is $|\vec{L}_i| = m_i r_i v_i = m_i r_i^2 \sin\theta \omega$.
>    - The direction of each $\vec{L}_i$ is perpendicular to the rod.
>    - The total angular momentum vector $\vec{L}$ is tilted relative to the shaft (the rotation axis $\vec{\omega}$). As the system rotates, the vector $\vec{L}$ rotates in space, meaning $\frac{d\vec{L}}{dt} \neq 0$. This requires a net external torque to be constantly supplied by the shaft bearings.
> 
> 2. **Coordinates Over Time:**
>    If we align the shaft along the x-axis ($x_1$) and let the system rotate in the yz-plane ($x_2$ and $x_3$ components), the positions of the masses as functions of time are:
>    - $x_1 = r_1 \cos\theta$, $y_1 = r_1 \sin\theta \cos\omega t$, $z_1 = r_1 \sin\theta \sin\omega t$.
>    - $x_2 = -r_2 \cos\theta$, $y_2 = -r_2 \sin\theta \cos\omega t$, $z_2 = -r_2 \sin\theta \sin\omega t$.
> 
> 3. **Inertia Tensor Formulation:**
>    Using the coordinate expressions, we can compute the components of the Moment of Inertia Tensor:
>    - $I_{11} = m_1(y_1^2 + z_1^2) + m_2(y_2^2 + z_2^2) = (m_1 r_1^2 + m_2 r_2^2) \sin^2\theta$.
>    - $I_{22} = m_1(x_1^2 + z_1^2) + m_2(x_2^2 + z_2^2) = (m_1 r_1^2 + m_2 r_2^2) (\cos^2\theta + \sin^2\theta \sin^2\omega t)$.
>    - $I_{12} = -(m_1 x_1 y_1 + m_2 x_2 y_2) = -(m_1 r_1^2 + m_2 r_2^2) \sin\theta \cos\theta \cos\omega t$.
> 
>    By multiplying this time-dependent inertia tensor by the angular velocity vector $\vec{\omega} = (\omega, 0, 0)$, we find the components of the angular momentum vector:
>    $$ L_i = I_{i1} \omega $$
>    This reveals how the products of inertia (the off-diagonal term $I_{12}$) generate components of $\vec{L}$ perpendicular to the rotation axis, causing the dynamic imbalance.
