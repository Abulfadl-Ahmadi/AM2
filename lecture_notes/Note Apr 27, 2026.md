Here is a comprehensive study guide created from your lecture notes. I have transcribed the original Persian text exactly as it appears and provided thorough, expert-level elaborations to fill in the gaps left by the lack of verbal context.

---

# Study Guide: Classical Scattering Theory and Non-Inertial Reference Frames

## Page 1: Introduction to Scattering Cross-Section
> **Original Transcription (Persian):**
> *   **تعریف سطح مقطع پراکندگی:**
> *   $\sigma(\theta) = \frac{dN_s(\theta, \theta+d\theta)}{d\Omega(\theta)}$
> *   **تعریف (سطح مقطع پراکندگی):** تعداد ذرات پراکنده شده به زاویه $\theta$ و $\theta+d\theta$ تقسیم بر [مقدار دیگر].
> *   *در مورد حساسیت پراکندگی، شمارش ذرات برخوردی با سطح مقطع...*

**Expert Elaboration:**
The notes begin by defining the **Differential Scattering Cross-Section**, a fundamental concept in particle and nuclear physics. 
*   **Formula Breakdown:** The professor writes $\sigma(\theta) = \frac{dN_s}{d\Omega}$. Note that in standard definitions, the number of scattered particles ($dN_s$) into a solid angle $d\Omega$ is proportional to the incident particle flux ($I$). The complete definition is:
    $$ \frac{d\sigma}{d\Omega} = \frac{1}{I} \frac{dN_s}{d\Omega} $$
    where $I$ is the number of incident particles per unit area per unit time. If the incident flux $I=1$, the formula simplifies to the one written in the notes.
*   **Physical Meaning:** The differential cross-section $\frac{d\sigma}{d\Omega}$ represents the effective area that the target presents to the incoming beam for scattering particles into a specific angle $\theta$. It is usually measured in units of area (e.g., barns).

---

## Page 2: Derivation of Cross-Section from Impact Parameter
> **Original Transcription (Persian):**
> *   **تعریف:**
> *   $\sigma(\theta) d\Omega_s = \frac{dN_s(\theta, \theta+d\theta)}{I}$, where $I = \frac{dN}{dA}$.
> *   **در حالت کلی: پراکندگی ذره نقطه‌ای، کلاسیک و مستقل از ذرات.**
> *   $\sigma(\theta) = \frac{b}{\sin\theta} \left| \frac{db}{d\theta} \right|$ 
> *   *Note in margin:* $db$ و $b$ پارامتر برخورد هستند.

**Expert Elaboration:**
This page derives the relationship between the **scattering angle** and the **impact parameter** ($b$). The impact parameter is the perpendicular distance between the incident particle's trajectory and the center of the scattering potential.
*   **Conservation of Particles:** For a thin target, the number of particles scattered into a solid angle $d\Omega$ between $\theta$ and $\theta+d\theta$ must equal the number of particles entering the system through an annular ring defined by impact parameters $b$ and $b+db$.
    *   Incident particles in the ring: $I \times 2\pi b db$.
    *   Scattered particles in the solid angle: $I \times \sigma(\theta) \times d\Omega_s = I \times \sigma(\theta) \times 2\pi \sin\theta d\theta$.
*   **Important Result:** By equating these two quantities, we arrive at the general formula for calculating the differential cross-section in classical scattering:
    $$ \sigma(\theta) = \frac{b}{\sin\theta} \left| \frac{db}{d\theta} \right| $$
    This formula is immensely powerful. If you know how the impact parameter $b$ relates to the scattering angle $\theta$ (i.e., $b(\theta)$), you can calculate the cross-section.

---

## Page 3: The Hard-Sphere Scattering Model
> **Original Transcription (Persian):**
> *   **سوال: سطح مقطع پراکندگی برای پراکندگی از یک گوی سخت (Hard Sphere) چقدر است؟**
> *   $b = (R_1+R_2) \cos\alpha$ ، $\theta = 2\alpha$
> *   $\sigma(\theta) = \frac{b}{\sin\theta} \left|\frac{db}{d\theta}\right| \rightarrow \sigma(\theta) = \frac{1}{4}(R_1+R_2)^2$
> *   **محاسبه سطح مقطع کل:**
> *   $\sigma_t = \int \sigma(\theta) d\Omega_s$
> *   $\sigma_t = \int_0^\pi \frac{1}{4}(R_1+R_2)^2 \times 2\pi \sin\theta d\theta = \pi(R_1+R_2)^2$

**Expert Elaboration:**
This page solves the classic "Hard Sphere" scattering problem. Imagine two solid spheres: an incoming particle of radius $R_1$ and a target sphere of radius $R_2$.
*   **Geometry:**
    *   The effective collision radius is $(R_1 + R_2)$.
    *   The geometry of the collision allows us to write the relationship between the impact parameter $b$ and the scattering angle $\theta$. Using the law of cosines and geometry, $b = (R_1+R_2) \sin\alpha$. However, the notes define $\theta = 2\alpha$, deriving $b = (R_1+R_2)\cos(\theta/2)$.
*   **Derivation of $\sigma(\theta)$:**
    *   Squaring the impact parameter gives $b^2 = (R_1+R_2)^2 \cos^2(\theta/2)$.
    *   Using the trigonometric identity $\cos^2(\theta/2) = \frac{1+\cos\theta}{2}$, we find $b^2 = \frac{1}{2}(R_1+R_2)^2 (1+\cos\theta)$.
    *   Taking the derivative with respect to $\theta$ yields $|\frac{db^2}{d\theta}| = \frac{1}{2}(R_1+R_2)^2 \sin\theta$.
    *   Substituting this into the generalized formula $\sigma(\theta) = \frac{1}{2\sin\theta} |\frac{db^2}{d\theta}|$ gives $\sigma(\theta) = \frac{1}{4}(R_1+R_2)^2$.
*   **Key Physical Result:** The differential cross-section for a hard sphere is **independent of the angle** ($\theta$). This means that scattering is isotropic in the Center of Mass frame. The **Total Cross-Section** ($\sigma_t$) integrates this constant over the full solid angle, yielding $\sigma_t = \pi(R_1+R_2)^2$, which is exactly the geometric cross-sectional area of the two colliding spheres.

---

## Page 4: Central Potential Scattering
> **Original Transcription (Persian):**
> *   **پراکندگی دو ذره‌ای: پراکندگی ذره نقطه‌ای بر روی پتانسیل**
> *   $dN_s(\theta, \theta+d\theta) = dN_s(\theta', \theta'+d\theta')$ (تعداد ذرات در چارچوب‌های مختلف برابر است)
> *   **رابطه تبدیل سطح مقطع در دستگاه‌های مختصات مختلف:**
> *   $\sigma(\theta') = \sigma(\theta) \times \frac{\sin\theta}{\sin\theta'} \times \frac{d\theta}{d\theta'}$
> *   **زاویه انحراف:**
> *   $\Delta\Phi = \int_{r_{min}}^{r_{max}} \frac{(L/r^2) dr}{\sqrt{2\mu (E - V(r)) - \frac{L^2}{r^2}}}$
> *   $\theta = \pi - 2\Delta\Phi$

**Expert Elaboration:**
This page introduces scattering due to a generic central force potential $V(r)$. This is crucial for Rutherford scattering and orbital mechanics.
*   **Deflection Angle Integral:** When a particle moves in a central potential $V(r)$, it has a conserved angular momentum $L$ and energy $E$. The total change in the azimuthal angle ($\Delta\Phi$) as the particle travels from a far distance (where $r \to \infty$), reaches a minimum radius ($r_{min}$), and escapes back to infinity, is given by:
    $$ \Delta\Phi = \int_{r_{min}}^{\infty} \frac{(L/r^2) dr}{\sqrt{2\mu (E - V(r)) - \frac{L^2}{r^2}}} $$
    *(Note: In the notes, the professor lists the limits as $r_{min}$ to $r_{max}$, where $r_{max}$ is effectively $\infty$ for scattering, or the turning points).*
*   **Angle Transformation:** The scattering angle $\theta$ (the angle between the initial and final velocity vectors) is related to this orbital angle by:
    $$ \theta = \pi - 2\Delta\Phi $$
    This is because the particle enters from and exits to infinity, causing a total angle $\pi$ minus twice the angle swept from periapsis to infinity.
*   **Frame Mapping:** The notes also provide a transformation formula relating the cross-section $\sigma(\theta)$ in one frame (e.g., Laboratory frame) to $\sigma(\theta')$ in another (e.g., Center of Mass frame), which is essential for analyzing multi-particle collisions.

---

## Page 5: Rutherford Scattering & Introduction to Non-Inertial Frames
> **Original Transcription (Persian):**
> *   **پراکندگی رادرفورد (Rutherford Scattering):**
> *   $\sigma(\theta) = \frac{k^2}{4} \cdot \frac{1}{\sin^4\frac{\theta}{2}}$ ، $k = \frac{zZ e^2}{4\pi\epsilon_0 E}$
> *   $\sigma(\theta) \propto \frac{1}{\sin^4\frac{\theta}{2}} \rightarrow \sigma_t = \int \sigma(\theta) \sin\theta d\theta 2\pi \rightarrow \sigma_t \rightarrow \infty$
> *   **دستگاه مرجع غیر لخت:**
> *   $\vec{r}' = \vec{R} + \vec{r}$
> *   $\hat{e}'_i = \hat{e}_i$ (بردارهای پایه در دستگاه جدید و قدیم یکی هستند)
> *   $\vec{V}' = u'_1 \hat{e}'_1 + \dots$, $\vec{V} = u_1 \hat{e}_1 + \dots$
> *   **⚠️ نکته مهم:** $\hat{e}_i \neq \hat{e}'_i$ ! (این بردارها برابر نیستند!)

**Expert Elaboration:**
*   **Rutherford Scattering:** The notes explicitly present the famous Rutherford scattering formula. This occurs when a charged particle scatters off a Coulomb potential ($V(r) \propto \frac{1}{r}$). The differential cross-section is proportional to $\frac{1}{\sin^4(\theta/2)}$, which perfectly matches the experimental results that revealed the atomic nucleus.
*   **Divergence of $\sigma_t$:** When you attempt to compute the total cross-section $\sigma_t$ for a Coulomb potential, the integral $\int_0^\pi \frac{1}{\sin^4(\theta/2)} \sin\theta d\theta$ diverges (goes to infinity) at small angles ($\theta \to 0$). This is physically significant because the Coulomb force is a long-range force; even very distant particles feel the force and get deflected by a tiny amount, resulting in an infinite total effective area.
*   **Change of Topic - Non-Inertial Frames:** The bottom half transitions to Classical Mechanics, specifically the kinematics of **Non-Inertial (accelerated or rotating) reference frames**.
*   **Basis Vector Warning:** The red warning `$\hat{e}_i \neq \hat{e}'_i$!` is a critical physics point. While the position vectors can be added using $\vec{r}' = \vec{R} + \vec{r}$, the unit vectors defining the coordinate systems are **not equal** if the non-inertial frame is rotating relative to the inertial one. This difference is the fundamental reason why fictitious forces (like Centrifugal and Coriolis forces) appear.

---

## Page 6: Kinematics in Rotating Frames
> **Original Transcription (Persian):**
> *   **مسئله: در دو دستگاه، سرعت و شتاب یک جسم را محاسبه کنیم.**
> *   $\vec{V} = v_1\hat{e}_1 + v_2\hat{e}_2 + v_3\hat{e}_3$
> *   $\frac{d\vec{V}}{dt} = \dot{v}_1\hat{e}_1 + \dot{v}_2\hat{e}_2 + \dot{v}_3\hat{e}_3$
> *   $\frac{d\vec{V}}{dt} \quad (\frac{d\vec{V}}{dt})'$
> *   **صورت:**
> *   $\frac{d\vec{V}}{dt} = \vec{\omega} \times \vec{V}$

**Expert Elaboration:**
This final page derives the basis for the **Coriolis and Centrifugal forces** by looking at how time derivatives work in a rotating frame.
*   **The Fundamental Principle:** The velocities in an inertial frame ($\vec{V}$) and a rotating frame ($\vec{V}'$) are related by $\vec{V} = \vec{V}' + \vec{\omega} \times \vec{r}'$.
*   **Basis Vector Derivatives:** When we differentiate the vector $\vec{V}$ with respect to time in an inertial frame, we must account for the fact that the rotating frame's basis vectors ($\hat{e}_i$) are themselves spinning.
    *   The derivative of a rotating vector is: $\frac{d\hat{e}_i}{dt} = \vec{\omega} \times \hat{e}_i$.
*   **The Transport Theorem:** Taking the time derivative of $\vec{V}$:
    $$ \left( \frac{d\vec{V}}{dt} \right)_{Inertial} = \left( \frac{d\vec{V}}{dt} \right)_{Rotating} + \vec{\omega} \times \vec{V} $$
*   **Final Derivation:** The notes present the equation $\frac{d\vec{V}}{dt} = \vec{\omega} \times \vec{V}$. This is the second term of the transport theorem. It represents the **change in velocity observed in an inertial frame solely due to the rotation of the coordinate system, even if the vector is stationary in the rotating frame**. A complete expansion of this equation leads to the standard acceleration formula:
    $$ \vec{a}_{Inertial} = \vec{a}_{Rotating} + \underbrace{2\vec{\omega} \times \vec{v}_{Rotating}}_{\text{Coriolis Acc.}} + \underbrace{\vec{\omega} \times (\vec{\omega} \times \vec{r})}_{\text{Centripetal Acc.}} + \underbrace{\frac{d\vec{\omega}}{dt} \times \vec{r}}_{\text{Euler Acc.}} $$
    This final page transitions the course from classical scattering into the deeper topic of rotating reference frames and fictitious forces.