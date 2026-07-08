# Chapter 10: Motion in Non-Inertial Reference Frames (Continued) - Lecture: May 9, 2026

> [!abstract] Navigation
> **Chapter:** [[Chapter 10 - Non-Inertial Reference Frames]] | **Prev:** [[Note May 4, 2026]] | **Next:** [[Note May 11, 2026]] | [[Journal/Lecture Index|📚 All Lectures]]

## 1. Introduction and Outline (مقدمه و سرفصل‌ها)

**Original Notes Transcription:**
> **Cyclones**
> 
> - **سقوط آزاد در نزدیکی زمین:** (Free fall near the Earth)
> - **له انحراف جانبی پرتابه:** (Lateral deflection of a projectile)
> - **آونگ فوکو (دانشکده):** (Foucault Pendulum (department/college))
> - **مقدمات جسم صلب:** (Introduction to Rigid Body)
> 
> ■ **مرور:** (Review:)
> اگر یک ناظر اصرار به نوشتن معادلات قوانین نیوتن در دستگاه نالخت داشته باشد:
> (If an observer insists on writing Newton's equations/laws in a non-inertial frame:)
> **اطراف زمین - چرخش $\vec{\omega}$ تقریباً ثابت:**
> (Around Earth - rotation $\vec{\omega}$ approximately constant:)
> $$\vec{F}_{eff} = \vec{F} + m\vec{g}_{eff} - 2m\vec{\omega} \times \vec{v}_{rot}$$
> $$\vec{g}_{eff} \equiv \vec{g}_0 - \vec{\omega} \times [\vec{\omega} \times (\vec{r} + \vec{R})]$$
> $$\vec{r} \ll \vec{R} \rightarrow \vec{g}_{eff} \approx \vec{g}_0 - \vec{\omega} \times (\vec{\omega} \times \vec{R})$$
> 
> ■ **مسأله I) صورت نسبتاً ساده:** (Problem I: A relatively simple case:)
> *(Diagram shows a tower of height $h$ on the Earth. A person drops a ball from the top.)*
> Local coordinate system at latitude $\lambda$:
> - x-axis points South.
> - y-axis points East.
> - z-axis points Up (local vertical).
> 
> *(Top View shows x-axis pointing South, y-axis pointing East (to the left in the diagram), showing the direction of rotation and deflection)*

> **Elaboration:**
> This lecture covers the physical applications of motion on a rotating Earth. The four main topics are:
> 1. Eastward deflection of a free-falling object.
> 2. General deflection of projectiles.
> 3. The Foucault Pendulum as proof of Earth's rotation.
> 4. Preliminary concepts of rigid body dynamics.
> 
> First, we review the effective force equation on a rotating Earth. The rotation vector $\vec{\omega}$ of the Earth is assumed constant in magnitude and direction. Since any localized motion involves distances $\vec{r}$ much smaller than the Earth's radius $\vec{R}$ ($|\vec{r}| \ll |\vec{R}|$), the centrifugal force term is approximated as a constant depending only on latitude $\lambda$ and is absorbed into the effective gravitational acceleration $\vec{g}_{eff}$.
> 
> To solve the free-fall problem, we set up a local coordinate system at latitude $\lambda$ in the Northern Hemisphere:
> - The **z-axis** is the local vertical pointing upward.
> - The **x-axis** is horizontal, pointing South (along the meridian towards the equator).
> - The **y-axis** is horizontal, pointing East.
> 
> This local coordinate system forms a right-handed Cartesian coordinate system ($\hat{x} \times \hat{y} = \hat{z}$).

---

## 2. Derivation of Free Fall Deflection (محاسبه انحراف سقوط آزاد)

**Original Notes Transcription:**
> **پروژه اول:** (First project:)
> **Step I)**
> $$\vec{F}_{eff} = m\vec{g}_{eff} - 2m\vec{\omega}\times\vec{v}_{rot} = m\vec{a}_{rot}$$
> $$\vec{g}_{eff} \approx \vec{g}_0 + O(\omega^2)$$
> 
> Components of Earth's rotation vector $\vec{\omega}$:
> $$\text{(a)} \rightarrow \begin{cases} \omega_x = -\omega \cos\lambda \\ \omega_y = 0 \\ \omega_z = \omega \sin\lambda \end{cases}$$
> 
> Up to first order in $\omega$ (تا مرتبه از $\omega$):
> $$\text{(b)} \rightarrow \begin{cases} \dot{x} \approx 0 \\ \dot{y} \approx 0 \\ \dot{z} \approx -gt \end{cases} \quad (\text{since } \dot{x} = O(\omega), \, \dot{y} = O(\omega), \, \dot{z} = -gt + O(\omega))$$
> 
> $$\text{(c)} \rightarrow g_{eff,x} = 0, \quad g_{eff,y} = 0, \quad g_{eff,z} \approx -g$$
> 
> **Step II)**
> $$\vec{g}_{eff} \approx 0\hat{x} + 0\hat{y} - g\hat{z}$$
> $$\vec{\omega} \times \vec{v}_{rot} = (\omega_y v_z - \omega_z v_y)\hat{x} + (\omega_z v_x - \omega_x v_z)\hat{y} + (\omega_x v_y - \omega_y v_x)\hat{z}$$
> 
> To first order in $\omega$, since $v_x, v_y \approx 0$:
> $$\vec{\omega} \times \vec{v}_{rot} \approx -\omega_x v_z \hat{y} = [\omega \cos\lambda v_z]\hat{y} + O(\omega^2)$$
> Using $v_z \approx -gt$:
> $$\vec{\omega} \times \vec{v}_{rot} \approx -\omega \cos\lambda g t \hat{y}$$
> 
> The Coriolis acceleration term is:
> $$-2\vec{\omega} \times \vec{v}_{rot} \approx 2\omega g t \cos\lambda \hat{y}$$
> 
> So, the components of relative acceleration $m\vec{a}_r \approx m\vec{g}_{eff} - 2m\vec{\omega}\times\vec{v}_{rot}$ are:
> $$\begin{cases} (a_{rot})_x \approx 0 \\ (a_{rot})_y \approx 2\omega g t \cos\lambda \\ (a_{rot})_z \approx -g \end{cases}$$
> 
> **Step III)**
> Integrating the accelerations to find the deflection:
> $$(a_{rot})_y \approx 2\omega g t \cos\lambda \rightarrow (v_{rot})_y \approx \int_0^t (a_{rot})_y dt' = \omega g t^2 \cos\lambda$$
> $$(a_{rot})_z \approx -g \rightarrow z(t) = h - \frac{1}{2}gt^2 \rightarrow t_{fall} = \sqrt{\frac{2h}{g}}$$
> 
> $$y(t) = \int_0^t (v_{rot})_y dt' = \frac{1}{3}\omega g t^3 \cos\lambda$$
> 
> The total eastward deflection at landing ($t = t_{fall}$) is:
> $$d = \frac{1}{3}\omega \cos\lambda \sqrt{\frac{8h^3}{g}}$$

> **Elaboration:**
> We calculate the deflection of a mass dropped from rest at height $h$.
> 
> 1. **Angular Velocity Components:** 
>    At latitude $\lambda$ in the Northern Hemisphere, the Earth's rotation vector $\vec{\omega}$ lies in the vertical-meridian (xz) plane. The z-axis (upward) and the x-axis (Southward) components are:
>    - $\omega_z = \omega \sin\lambda$ (positive upward).
>    - $\omega_x = -\omega \cos\lambda$ (negative because it points Northward, opposite to our Southward x-axis).
>    - $\omega_y = 0$ (no East-West component).
> 
> 2. **First-Order Approximation:** 
>    Since $\omega \approx 7.29 \times 10^{-5} \text{ rad/s}$ is extremely small, we use a perturbation expansion in powers of $\omega$.
>    - To zero-th order ($\omega = 0$), the particle is in simple vertical free fall: $\dot{x} \approx 0, \dot{y} \approx 0, \dot{z} \approx -gt$, and $z(t) \approx h - \frac{1}{2}gt^2$.
> 
> 3. **Coriolis Force Calculation:**
>    The Coriolis acceleration is $-2\vec{\omega} \times \vec{v}_r$.
>    Expanding the cross product to first order in $\omega$:
>    - The horizontal velocities $v_x, v_y$ are $O(\omega)$ and can be ignored when multiplied by $\vec{\omega}$.
>    - The vertical velocity is $v_z \approx -gt$.
>    - This simplifies the cross product to: $-2\vec{\omega} \times \vec{v}_r \approx -2(-\omega_x v_z) \hat{y} = 2\omega_x v_z \hat{y} = 2(-\omega \cos\lambda)(-gt)\hat{y} = 2\omega g t \cos\lambda \hat{y}$.
> 
> 4. **Deflection Integration:**
>    - The acceleration in the y-direction (Eastward) is $a_y = 2\omega g t \cos\lambda$.
>    - Integrating once gives the Eastward velocity: $v_y(t) = \omega g t^2 \cos\lambda$.
>    - Integrating again gives the Eastward position: $y(t) = \frac{1}{3}\omega g t^3 \cos\lambda$.
>    - The total time of fall is determined by the vertical motion: $t_{fall} = \sqrt{\frac{2h}{g}}$.
>    - Substituting $t_{fall}$ into the expression for $y(t)$ yields the final deflection:
>      $$ d = \frac{1}{3}\omega \cos\lambda \sqrt{\frac{8h^3}{g}} $$
>    This deflection is to the **East** ($+y$).

---

## 3. Alternative Solution: Conservation of Angular Momentum (راه حل دوم: پایستگی تکانه زاویه ای)

**Original Notes Transcription:**
> ■ **راه حل دوم (شهودی، عمیق تر):** (Second solution (intuitive, deeper):)
> **New Physics**
> 
> *(Diagrams show a falling ball from a tower of height $h$. The top of the tower has radius $R+h$ and speed $v_y = (R+h)\omega \cos\lambda$. The ground has radius $R$ and speed $v_0 = R\omega \cos\lambda$.)*
> 
> Conservation of angular momentum about Earth's rotation axis:
> $$l = m(R+h)v_y = m\omega \cos\lambda (R+h)^2 = \text{const}$$
> $$mr^2 \dot{\theta} = \text{const} \quad (\text{where } r = R+z)$$
> 
> $$\rightarrow \dot{\theta} = \frac{l}{mr^2} = \frac{\omega \cos\lambda (R+h)^2}{(R+z)^2}$$
> 
> Using binomial expansion $[(1+x)^n \approx 1+nx \quad x \ll 1]$ and since $h, z \ll R$:
> $$\dot{\theta} \approx \omega \cos\lambda \left(1 + \frac{2h}{R}\right)\left(1 - \frac{2z}{R}\right)$$
> 
> Integrating to find the angular displacement $\Delta \Theta$ along the latitude circle:
> $$\Delta \Theta = \int_0^{t_{fall}} \dot{\theta} dt = \omega \cos\lambda \left(1 + \frac{2h}{R}\right) \int_0^{t_{fall}} \left(1 - \frac{2z}{R}\right) dt$$
> 
> Substituting $z \approx h - \frac{1}{2}gt^2$:
> $$\Delta \Theta \approx \omega \cos\lambda \left(1 + \frac{2h}{R}\right) \int_0^{t_{fall}} \left(1 - \frac{2h}{R} + \frac{gt^2}{R}\right) dt$$
> $$\Delta \Theta \approx \omega \cos\lambda t_{fall} + \frac{\omega g \cos\lambda t_{fall}^3}{3R}$$
> 
> The total linear displacement of the particle in the eastward direction is:
> $$y_{particle} \approx R \Delta \Theta = \omega R \cos\lambda t_{fall} + \frac{\omega g \cos\lambda t_{fall}^3}{3}$$
> 
> **توجه کنید، در همین مدت زمان، نقطه مقابل ذره روی زمین هم جابجا شده است:**
> (Note that during this same time interval, the point on the ground opposite to the particle has also moved:)
> $$v_0 = R \cos\lambda \omega \rightarrow d_0 = R \cos\lambda t_{fall}$$
> 
> The net deflection relative to the ground is:
> $$d_{deflection} = y_{particle} - d_0 = \frac{\omega g \cos\lambda t_{fall}^3}{3}$$
> 
> Substituting $t_{fall} = \sqrt{\frac{2h}{g}}$:
> $$d_{deflection} = \frac{1}{3}\omega \cos\lambda \sqrt{\frac{8h^3}{g}}$$
> *(Checked with double ticks and a smiley face in the notes)*

> **Elaboration:**
> The Eastward deflection can be derived from an inertial perspective using **conservation of angular momentum**.
> 
> 1. **Initial State:** 
>    At the top of the tower (radius $r_{top} = R+h$), the particle is rotating with the Earth. Its linear speed in the Eastward direction is $v_{top} = (R+h)\omega \cos\lambda$. Its angular momentum about the Earth's axis of rotation is:
>    $$ l = m r_{axis} v_{top} = m (R+h)\cos\lambda \times (R+h)\omega\cos\lambda = m\omega\cos^2\lambda(R+h)^2 $$
> 
> 2. **Conservation of Angular Momentum:** 
>    As the particle falls, there are no Eastward forces acting on it in the inertial frame (gravity is purely radial). Thus, its angular momentum $l = m r^2 \cos^2\lambda \dot{\theta}$ is conserved, where $\theta$ is the longitude.
>    If we define $\dot{\Theta} = \dot{\theta} \cos\lambda$ as the rate of angular displacement along the latitude circle, we have:
>    $$ \dot{\Theta} = \omega\cos\lambda \frac{(R+h)^2}{(R+z)^2} $$
> 
> 3. **Binomial Expansion:**
>    Since the height $h$ and the height during the fall $z$ are tiny compared to the Earth's radius $R$ ($h, z \ll R$), we expand:
>    $$ \frac{(R+h)^2}{(R+z)^2} = \left(1 + \frac{h}{R}\right)^2 \left(1 + \frac{z}{R}\right)^{-2} \approx \left(1 + \frac{2h}{R}\right)\left(1 - \frac{2z}{R}\right) $$
> 
> 4. **Integration:**
>    Substituting $z(t) \approx h - \frac{1}{2}gt^2$:
>    $$ \Delta \Theta \approx \omega\cos\lambda \int_0^{t_{fall}} \left(1 + \frac{2h}{R} - \frac{2z}{R}\right) dt \approx \omega\cos\lambda \int_0^{t_{fall}} \left(1 + \frac{gt^2}{R}\right) dt = \omega\cos\lambda t_{fall} + \frac{\omega g \cos\lambda t_{fall}^3}{3R} $$
> 
> 5. **Relative Deflection:**
>    - The total Eastward linear distance traveled by the particle in space is $y_{particle} = R \Delta \Theta = R \omega \cos\lambda t_{fall} + \frac{1}{3}\omega g \cos\lambda t_{fall}^3$.
>    - During this same time, the base of the tower (on the ground) moves Eastward by $d_0 = R \omega \cos\lambda t_{fall}$.
>    - The net deflection relative to the ground is the difference:
>      $$ d_{deflection} = y_{particle} - d_0 = \frac{1}{3}\omega g \cos\lambda t_{fall}^3 $$
>    Substituting $t_{fall} = \sqrt{\frac{2h}{g}}$ yields exactly the same result as the Coriolis derivation, showing the deep connection between conservation of angular momentum in inertial frames and fictitious forces in rotating frames.

---

## 4. Foucault Pendulum Introduction (مقدمه آونگ فوکو)

**Original Notes Transcription:**
> ■ **آونگ فوکو:** (Foucault Pendulum:)
> *(Diagram shows a 3D coordinate system $x, y, z$ with a pendulum of mass $m$ suspended from a point on the z-axis, showing tension $\vec{T}$ and gravity $m\vec{g}$.)*
> 
> **TACO**
> **Trump**
> **Always**
> **Chickens**
> **Out**

> **Elaboration:**
> The lecture concludes with the setup for the **Foucault Pendulum**.
> 
> A Foucault pendulum consists of a heavy mass suspended by a long wire from a pivot designed to allow the pendulum to swing in any vertical plane. The local coordinate axes are set up such that:
> - The z-axis is local vertical (direction of $\vec{g}_{eff}$).
> - The x-axis points South.
> - The y-axis points East.
> 
> In this coordinate frame, the forces acting on the pendulum are:
> 1. The tension in the wire $\vec{T}$.
> 2. The effective gravity $m\vec{g}_{eff}$.
> 3. The Coriolis force $-2m\vec{\omega} \times \vec{v}_r$.
> 
> The Coriolis force causes the plane of oscillation of the pendulum to precess (rotate) slowly over time. The rate of rotation depends on latitude $\lambda$ and is given by $\Omega_{precession} = \omega \sin\lambda$. This precession provides a direct, localized demonstration of the Earth's rotation without the need for astronomical observations.
> 
> *(The humorous acronym "TACO" - "Trump Always Chickens Out" was noted from the class discussion).*
