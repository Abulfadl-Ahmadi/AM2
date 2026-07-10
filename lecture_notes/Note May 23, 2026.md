# Chapter 11: Dynamics of Rigid Bodies (Continued) - Lecture: May 23, 2026

> [!abstract] Navigation
> **Chapter:** [[Chapter 11 - Dynamics of Rigid Bodies]] | **Prev:** [[Note May 18, 2026]] | **Next:** [[Note May 25, 2026]] | [[Lecture Index|📚 All Lectures]]

## 1. General Properties and Orthogonality (مرور و تعامد بردارهای ویژه)

**Original Notes Transcription:**
> **Timeline / Headings:**
> - **قضیه محورهای موازی تعمیم یافته** (Generalized Parallel Axis Theorem)
> - **خواص دورانی تانسور I** (Rotational Properties of Tensor I)
> - **معادلات دوران جسم صلب** (Equations of Rotation of a Rigid Body)
> 
> ■ **نکته : تعامد بردارهای ویژه ماتریس های حقیقی متقارن:**
> (Note: Orthogonality of eigenvectors of real symmetric matrices:)
> 
> $$\begin{cases} A \vec{v} = \lambda \vec{v} \\ A \vec{w} = \mu \vec{w} \end{cases}$$
> *(Here, $A$ represents a symmetric matrix like the inertia tensor $\{I\}$, while $\vec{v}, \vec{w}$ are its eigenvectors and $\lambda, \mu$ are the corresponding eigenvalues).*
> 
> ■ **مرور مکانیک تحلیلی I:** (Review of Analytical Mechanics I:)
> $$\vec{v}^T \vec{w} \rightarrow v^T w$$
> - اگر تعامد ویژه بردارها مدنظر است $v^T w$ را محاسبه کنید:
> (If orthogonality of eigenvectors is considered, calculate $v^T w$:)
> 
> $$v^T \{A\} w = v^T (\mu w) = \mu v^T w$$
> $$v^T \{A\} w = (v^T \{A\}) w = (\{A\} v)^T w = (\lambda v)^T w = \lambda v^T w$$
> *(Since $A$ is symmetric, $A = A^T$)*
> 
> $$\rightarrow \mu v^T w = \lambda v^T w \rightarrow (\mu - \lambda) v^T w = 0$$
> 
> *Boxed equation:*
> $$\text{If } \mu \neq \lambda \rightarrow v^T w = 0 \quad (\text{شرط تعامد - Orthogonality condition})$$
> 
> - **تبه‌گن یعنی چی؟** (What does degenerate mean?)

> **Elaboration:**
> The lecture begins with a mathematical property of real symmetric matrices, such as the Inertia Tensor $I_{ij}$. If you find the eigenvectors of a symmetric matrix corresponding to distinct eigenvalues ($\mu \neq \lambda$), those eigenvectors are guaranteed to be orthogonal to each other ($v^T w = 0$).
> 
> Physically, the eigenvectors of the inertia tensor represent the **Principal Axes of Inertia**. This theorem guarantees that as long as the principal moments of inertia are distinct (a non-degenerate "asymmetric top"), the three principal axes are mutually perpendicular, forming a valid Cartesian coordinate system. 
> The professor poses the question: "What does degenerate mean?" Degeneracy occurs when two or more eigenvalues are equal (e.g., $I_1 = I_2$). In this case, any linear combination of the corresponding eigenvectors is also an eigenvector, meaning the principal axes are not uniquely defined, but we can still choose them to be orthogonal (like any two perpendicular axes in the symmetric plane of a cylinder).

---

## 2. Generalized Parallel Axis Theorem (قضیه محورهای موازی تعمیم یافته)

**Original Notes Transcription:**
> ■ **تانسور لختی در دستگاه های مختلف (انتقال):** 
> (Inertia tensor in different coordinate systems (Translation):)
> 
> *(Diagram shows a fixed frame $X, Y, Z$ and a moving frame $x, y, z$ whose origin is displaced by a vector $\vec{a}$. A particle $m_\alpha$ has position $\vec{X}_\alpha$ in the fixed frame and $\vec{x}_\alpha$ in the moving frame).*
> 
> $$I_{ij} = \sum_\alpha m_\alpha \left( \delta_{ij} \sum_k X_{\alpha k}^2 - X_{\alpha i} X_{\alpha j} \right)$$
> *(اندیس ها فضایی 1,2,3 - spatial indices 1,2,3; $\alpha$ is اندیس ذره - particle index)*
> 
> **Step I)** $\vec{X} = \vec{a} + \vec{x} \rightarrow X_i = a_i + x_i$
> 
> نمادگذاری : تانسور لختی دورانی در دستگاه آبی را با $J_{ij}$ نمایش دهیم :
> (Notation: Let's denote the rotational inertia tensor in the blue translated frame as $J_{ij}$:)
> $$J_{ij} = \sum_\alpha m_\alpha \left( \delta_{ij} \sum_k X_{\alpha k}^2 - X_{\alpha i} X_{\alpha j} \right)$$
> Substitute $X_{\alpha k} = a_k + x_{\alpha k}$:
> *(ربطی به اندیس ذره ندارد $a_k \rightarrow$ مختصات همه ذرات به یک اندازه انتقال داده می شوند)*
> *(The shift $a_k$ does not depend on the particle index; all particles are translated by the same amount)*
> 
> $$J_{ij} = \sum_\alpha m_\alpha \left[ \delta_{ij} \sum_k (a_k + x_{\alpha k})^2 - (x_{\alpha i} + a_i)(x_{\alpha j} + a_j) \right]$$
> 
> Expanding this gives three groups of terms:
> $$J_{ij} = \sum_\alpha m_\alpha \left( \delta_{ij} \sum_k x_{\alpha k}^2 - x_{\alpha i} x_{\alpha j} \right) \quad \text{(I)}$$
> $$+ \sum_\alpha m_\alpha \left( \delta_{ij} \sum_k a_k^2 - a_i a_j \right) \quad \text{(II)}$$
> $$+ \sum_\alpha m_\alpha \left( \delta_{ij} \times 2 \times \sum_k a_k x_{\alpha k} - x_{\alpha i} a_j - a_i x_{\alpha j} \right) \quad \text{(III)}$$
> 
> - روی جمله سوم تمرکز کنیم (III): (Let's focus on the third term (III):)
> $$\text{III} = 2 \delta_{ij} \sum_k a_k \sum_\alpha m_\alpha x_{\alpha k} - a_j \sum_\alpha m_\alpha x_{\alpha i} - a_i \sum_\alpha m_\alpha x_{\alpha j}$$
> 
> - اگر مبدا دستگاه آبی روی مرکز جرم باشد تمام جملات بالا برابر صفر هستند:
> (If the origin of the blue frame is at the center of mass, all the above terms are zero, because $\sum m_\alpha \vec{x}_\alpha = \vec{0}$):
> 
> $$J_{ij} = I_{ij}^{(CM)} + M(a^2 \delta_{ij} - a_i a_j)$$
> *(تانسور لختی دورانی برای مبدا دلخواه)* (Rotational inertia tensor for an arbitrary origin)
> 
> *Boxed equation (قضیه محورهای موازی Pro Max Edition):*
> $$I_{ij} = I_{ij}^{(CM)} + M(a^2 \delta_{ij} - a_i a_j)$$
> 
> *Boxed equation (alternative form):*
> $$I_{ij}^{(CM)} = I_{ij} - M(a^2 \delta_{ij} - a_i a_j)$$
> 
> ■ **یادآوری از فیزیک I:** (Reminder from Physics I:)
> $$I = I_{CM} + M d^2$$
> 
> ■ **مثال:** (Example: The uniform cube from previous lectures)
> Center of mass is in the middle of the cube, original origin at a corner. Translation vector is $\vec{a} = \left(\frac{b}{2}, \frac{b}{2}, \frac{b}{2}\right)$.
> 
> $$\{J\} = \begin{pmatrix} \frac{2}{3} & -\frac{1}{4} & -\frac{1}{4} \\ -\frac{1}{4} & \frac{2}{3} & -\frac{1}{4} \\ -\frac{1}{4} & -\frac{1}{4} & \frac{2}{3} \end{pmatrix} M b^2$$
> 
> - شما حدس بزنید انتقال مبدأ به مرکز جرم ماتریس لختی دورانی قطری می شود:
> (You can guess that translating the origin to the center of mass makes the inertia matrix diagonal:)
> 
> Using $a^2 = |\vec{a}|^2 = \frac{3}{4}b^2$:
> $$I_{11}^{CM} = I_{11} - M\left(\frac{3}{4}b^2 - \frac{b}{2} \times \frac{b}{2}\right) = \frac{2}{3}Mb^2 - \frac{1}{2}Mb^2 = \frac{1}{6}Mb^2$$
> $$I_{12}^{CM} = -\frac{1}{4}Mb^2 - M\left( - \frac{b}{2} \times \frac{b}{2} \right) = 0$$
> 
> $$\rightarrow \{I^{CM}\} = \frac{1}{6}Mb^2 \begin{pmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{pmatrix} = \text{diag}\left(\frac{1}{6}Mb^2, \frac{1}{6}Mb^2, \frac{1}{6}Mb^2\right)$$

> **Elaboration:**
> The "Generalized Parallel Axis Theorem" (humorously called the Pro Max Edition) extends the 1D parallel axis theorem $I = I_{CM} + Md^2$ to the full 3D Inertia Tensor.
> 
> If we know the inertia tensor $I_{ij}^{(CM)}$ about a coordinate system located at the Center of Mass (CM), we can find the tensor $J_{ij}$ about *any* parallel coordinate system shifted by a vector $\vec{a}$. 
> The resulting formula is $J_{ij} = I_{ij}^{(CM)} + M(a^2 \delta_{ij} - a_i a_j)$. Notice that this formula adds an "inertia tensor of a point mass $M$ located at distance $\vec{a}$". 
> 
> A crucial feature is that this theorem ONLY works if one of the frames is strictly located at the Center of Mass, because that is the only way the cross-terms $\sum m_\alpha \vec{x}_\alpha$ vanish.
> 
> As an application, we revisit the uniform cube. Previously, we found its inertia tensor about a corner, which had non-zero off-diagonal elements (products of inertia). By translating our origin to the center of the cube (the CM), the parallel axis theorem immediately shows that all off-diagonal terms become zero, and the diagonal terms become equal to $\frac{1}{6}Mb^2$. Thus, about its center of mass, a uniform cube is a **spherical top** with a perfectly diagonal, degenerate inertia tensor.

---

## 3. Transformation of Inertia Tensor under Rotation (تبدیل تانسور لختی تحت دوران)

**Original Notes Transcription:**
> ■ **تبدیل تانسور لختی تحت دوران:** (Transformation of inertia tensor under rotation:)
> 
> $$L_k = \sum_l I_{kl} \omega_l \leftarrow \text{رابطه اصلی برای شروع}$$ (Main relation to start)
> 
> - مدل قصه در دستگاه دوران یافته $L, \omega, I$ را محاسبه می کنیم:
> (In the rotated frame, we calculate $L', \omega', I'$:)
> $$\vec{L}' = \{I'\} \vec{\omega}'$$
> 
> - در مکانیک تحلیلی I تبدیلات مختصات (مؤلفه های بردارها) را بدست آورده ایم:
> (In Analytical Mechanics I, we derived the coordinate transformations for vector components using the rotation matrix $\lambda$:)
> $$x_i' = \sum_j \lambda_{ij} x_j \rightarrow x_i = \sum_j \lambda_{ij}^T x_j' = \sum_j \lambda_{ji} x_j'$$
> 
> Applying this inverse transformation to the vectors $\vec{L}$ and $\vec{\omega}$:
> $$L_k = \sum_m \lambda_{mk} L_m' \quad \text{(*)}$$
> $$\omega_l = \sum_j \lambda_{jl} \omega_j' \quad \text{(**)}$$
> 
> - با جایگذاری در رابطه بالا داریم:
> (By substituting into the original relation $L_k = \sum_l I_{kl} \omega_l$:)
> $$\sum_m \lambda_{mk} L_m' = \sum_l I_{kl} \left( \sum_j \lambda_{jl} \omega_j' \right) = \sum_l \sum_j I_{kl} \lambda_{jl} \omega_j'$$
> 
> - سؤال: اگر دوست داشته باشیم $L_i'$ را در رابطه بالا استخراج کنیم چه پیشنهادی می دهید؟ 
> (Question: If we want to extract $L_i'$ from the above relation, what do you suggest?)
> طرفین را در $\lambda_{ik}$ ضرب کنیم و روی $k$ جمع بزنیم:
> (Multiply both sides by $\lambda_{ik}$ and sum over $k$:)
> 
> $$\sum_k \sum_m \lambda_{mk} \lambda_{ik} L_m' = \sum_m \left( \sum_k \lambda_{mk} \lambda_{ik} \right) L_m' = \sum_m \delta_{mi} L_m' = L_i'$$
> *(Left side simplifies using orthogonality of rotation matrices: $\sum_k \lambda_{mk} \lambda_{ik} = \delta_{mi}$)*
> 
> $$\sum_k \sum_l I_{kl} \sum_j \lambda_{ik} \lambda_{jl} \omega_j' = \sum_j \omega_j' \left( \sum_k \sum_l \lambda_{ik} \lambda_{jl} I_{kl} \right)$$
> *(Right side)*
> 
> Equating the two sides gives $L_i' = \sum_j I_{ij}' \omega_j'$, where:
> $$I_{ij}' = \sum_k \sum_l \lambda_{ik} \lambda_{jl} I_{kl}$$
> 
> *Boxed equation:*
> $$\{I'\} = \lambda \{I\} \lambda^T = \lambda \{I\} \lambda^{-1}$$

> **Elaboration:**
> Having covered how the inertia tensor transforms under *translation* (Parallel Axis Theorem), we now look at how it transforms under *rotation* of the coordinate axes. 
> 
> A standard vector like angular momentum $\vec{L}$ or angular velocity $\vec{\omega}$ transforms under a rotation matrix $\lambda$ as $\vec{L}' = \lambda \vec{L}$. However, the Inertia Tensor $\{I\}$ is a rank-2 tensor (a matrix), so it requires a "double" transformation.
> 
> We derive this by writing the fundamental equation $\vec{L} = \{I\}\vec{\omega}$ in the original unrotated frame, and substituting the inverse vector transformations $\vec{L} = \lambda^T \vec{L}'$ and $\vec{\omega} = \lambda^T \vec{\omega}'$. Solving the resulting algebraic equation for $\vec{L}'$ reveals that the inertia tensor in the new rotated frame $\{I'\}$ is related to the old tensor by the similarity transformation: $\{I'\} = \lambda \{I\} \lambda^T$. 
> This is the defining characteristic of a rank-2 tensor.

---

## 4. Euler's Equations for a Rigid Body (معادلات اویلر برای جسم صلب)

**Original Notes Transcription:**
> ■ **معادلات اویلر برای جسم صلب:** (Euler's equations for a rigid body:)
> 
> *(Diagram shows a fixed "Lab frame" $(x, y, z)$ and a rotating "Body frame" $(\hat{e}_1, \hat{e}_2, \hat{e}_3)$ moving with angular velocity $\vec{\omega}$.)*
> 
> گشتاور $\vec{\tau} \rightarrow \vec{N} = \left(\frac{d\vec{L}}{dt}\right)_{fixed}$ 
> *(قانون دوم نیوتون - Newton's second law)*
> 
> From previous lectures, relating a fixed frame to a rotating frame:
> $$\left(\frac{d\vec{r}}{dt}\right)_{fixed} = \left(\frac{d\vec{r}}{dt}\right)_{rot} + \vec{\omega} \times \vec{r}$$
> 
> Applying this to the angular momentum vector $\vec{L}$:
> $$\left(\frac{d\vec{L}}{dt}\right)_{fixed} = \left(\frac{d\vec{L}}{dt}\right)_{rot} + \vec{\omega} \times \vec{L}$$
> 
> **Step I)**
> *Boxed equation:*
> $$\vec{N} = \left(\frac{d\vec{L}}{dt}\right)_{body} + \vec{\omega} \times \vec{L} \quad \leftarrow \text{معادلات در دستگاه جسمی (Equations in body frame)}$$
> 
> - برای داشتن احساس نسبت به معادله برداری بالا، مولفه ۳-ام معادله بالا را در نظر می گیریم:
> (To get a feel for the above vector equation, we write out its 3rd component:)
> $$\dot{L}_3 + \omega_1 L_2 - \omega_2 L_1 = N_3$$
> 
> Where in the body frame: $L_i = \sum_k I_{ik} \omega_k$
> 
> **Step II)**
> محورهای مختصات دستگاه جسمی را منطبق بر محورهای اصلی می گیریم.
> (We take the coordinate axes of the body frame to coincide with the Principal Axes.)
> لذا داریم: (Hence we have:)
> $$L_i = I_i \omega_i$$
> 
> - به طور مثال رابطه ی بالا به صورت زیر ساده می شود:
> (For example, the above relation simplifies to:)
> $$I_3 \dot{\omega}_3 + \omega_1 (I_2 \omega_2) - \omega_2 (I_1 \omega_1) = N_3$$
> $$I_3 \dot{\omega}_3 + I_2 \omega_1 \omega_2 - I_1 \omega_1 \omega_2 = N_3$$
> 
> *Boxed equation:*
> $$I_3 \dot{\omega}_3 + (I_2 - I_1) \omega_1 \omega_2 = N_3 \quad \text{+ permutations}$$

> **Elaboration:**
> We finally arrive at the core equations governing 3D rigid body dynamics: **Euler's Equations**.
> Newton's second law for rotation states that Torque equals the rate of change of angular momentum: $\vec{N} = (\frac{d\vec{L}}{dt})_{fixed}$. However, we know that in the fixed laboratory frame, the inertia tensor components $I_{ij}(t)$ change continuously as the body tumbles, making calculations nearly impossible.
> 
> To bypass this, we use the operator identity for rotating frames to shift the time derivative into the **body-fixed frame**: $\vec{N} = (\frac{d\vec{L}}{dt})_{body} + \vec{\omega} \times \vec{L}$.
> While this adds a non-linear "fictitious torque" term ($\vec{\omega} \times \vec{L}$), the massive advantage is that inside the body-fixed frame, the inertia tensor is constant.
> 
> We simplify this even further (Step II) by aligning the body-fixed axes directly with the **Principal Axes of Inertia**. The inertia tensor becomes purely diagonal, and $L_i = I_i \omega_i$. Substituting this into the cross-product equation yields the three coupled, non-linear differential equations known as Euler's Equations. The third component is:
> $$I_3 \dot{\omega}_3 + (I_2 - I_1) \omega_1 \omega_2 = N_3$$
> The equations for the 1st and 2nd components are found by cyclic permutation of the indices (1->2, 2->3, 3->1).
