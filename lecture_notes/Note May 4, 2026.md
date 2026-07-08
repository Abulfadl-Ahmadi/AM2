# Chapter 10: Motion in Non-Inertial Reference Frames (Continued) - Lecture: May 4, 2026

> [!abstract] Navigation
> **Chapter:** [[Chapter 10 - Non-Inertial Reference Frames]] | **Prev:** [[Note May 2, 2026]] | **Next:** [[Note May 9, 2026]] | [[Journal/Lecture Index|📚 All Lectures]]

## 1. Application: Particle on a Rotating Rail (بررسی حرکت ذره روی ریل دوار)

**Original Notes Transcription:**
> ■ **دستگاه نالخت:** (Non-inertial frame)
> - **کوریولیس:** (Coriolis)
> - **دستگاه دوار (پیچیده ترین):** (Rotating frame (the most complex))
> 
> - **اگر ناظر در دستگاه نالخت اصرار به استفاده از قوانین نیوتن داشته باشد، نسخه پیشنهادی:**
>   (If the observer in the non-inertial frame insists on using Newton's laws, the proposed version:)
>   $$\vec{F} \rightarrow \vec{F}_{eff} = m\vec{a}_r$$
>   $$\vec{F}_{eff} = \vec{F} - m\ddot{\vec{R}}_f - m\dot{\vec{\omega}} \times \vec{r} - 2m\vec{\omega} \times \vec{v}_r - m\vec{\omega} \times (\vec{\omega} \times \vec{r})$$
> 
> • **مثال آموزشی (منطبق بر نمایش):** (Educational example (matching the demonstration):)
> *(Diagram shows a disk of radius $R$ rotating with angular velocity $\vec{\omega}$. In the Lab-frame, a particle at the edge has radial position vector $\vec{r}$. In the rotating frame, the particle has velocity $\vec{v}_{or}$. The linear velocity of that point on the disk is $\omega R$. The total velocity in the Lab-frame is $\vec{v}_{o-lab} = \vec{v}_{or} + \vec{\omega} \times \vec{r}$, which is the vector sum represented by the diagonal of a rectangle with sides $\vec{v}_{or}$ and $\omega R$.)*
> 
> - **با توجه به فیلم از دید ناظر در دستگاه دوار مسیر حرکت چیزی شبیه نمودار زیر است:**
>   (According to the video, from the perspective of the observer in the rotating frame, the trajectory is something like the diagram below:)
>   *(Diagram shows a vertical rotating guide/wire with a bead sliding on it under rotation $\vec{\omega}$.)*
> 
>   $$\vec{F}_{eff} = \vec{F} - m\ddot{\vec{R}}_f - m\dot{\vec{\omega}} \times \vec{r} - 2m\vec{\omega} \times \vec{v}_r - m\vec{\omega} \times (\vec{\omega} \times \vec{r})$$
>   *چون سرعت در دستگاه دوار ریلی در جهت شعاعی دارد.* (Because the velocity in the rotating rail frame is along the radial direction.)
> 
>   **شرایط مسأله:** (Problem conditions:)
>   - **ذره آزاد:** (Free particle / free motion along the rail)
>     - (i) $\vec{F} = 0$
>     - (ii) $\ddot{\vec{R}}_f = 0$
>     - (iii) $-m\dot{\vec{\omega}} \times \vec{r} = 0$ (Constant angular velocity $\dot{\vec{\omega}} = 0$)
> 
>   *(از دانش خود موضوع را مدنظر قرار می دهیم.)* (We consider the topic based on our own knowledge.)
>   $$\rightarrow \vec{F}_{eff} = -2m\vec{\omega} \times \vec{v}_r - m\vec{\omega} \times (\vec{\omega} \times \vec{r})$$
> 
> - **در دستگاه نالخت چه مختصاتی انتخاب کنیم؟** (What coordinates should we choose in the non-inertial frame?)
>   **Step I)**
>   *(Diagram shows the 2D rotating frame with polar unit vectors $\hat{r}$ and $\hat{\theta}$. The z-axis is along the rotation axis $\vec{\omega} = \omega \hat{z}$.)*
>   $$\vec{r}_r = r \hat{r}$$
>   $$\rightarrow \vec{v}_{rot} = \dot{r}\hat{r} + r\dot{\theta}\hat{\theta}$$
>   $$\vec{a}_{rot} = (\ddot{r} - r\dot{\theta}^2)\hat{r} + (2\dot{r}\dot{\theta} + r\ddot{\theta})\hat{\theta}$$
> 
>   **Step II)**
>   $$\cdot \quad 2\vec{\omega} \times \vec{v}_r = 2\omega\hat{z} \times (\dot{r}\hat{r} + r\dot{\theta}\hat{\theta}) = 2\omega\dot{r}\hat{\theta} - 2\omega r\dot{\theta}\hat{r}$$
>   $$\cdot \quad \vec{\omega} \times (\vec{\omega} \times \vec{r}) = -\omega^2 r \hat{r}$$
> 
>   $$\vec{F}_{eff} = m\vec{a}_r \rightarrow m\vec{a}_r = 0 + 0 + 0 - 2m(\omega\dot{r}\hat{\theta} - \omega r\dot{\theta}\hat{r}) + m\omega^2 r\hat{r}$$
>   $$\rightarrow m(\ddot{r} - r\dot{\theta}^2)\hat{r} + m(2\dot{r}\dot{\theta} + r\ddot{\theta})\hat{\theta} = (2m\omega r\dot{\theta} + m\omega^2 r)\hat{r} - 2m\omega\dot{r}\hat{\theta}$$
>   By equating the $\hat{r}$ and $\hat{\theta}$ components, we obtain the system of equations:
>   $$\begin{cases} (I) \quad \ddot{r} - r\dot{\theta}^2 = 2\omega r\dot{\theta} + \omega^2 r \\ (II) \quad 2\dot{r}\dot{\theta} + r\ddot{\theta} = -2\omega\dot{r} \end{cases}$$
> 
> - **برای مسئله خاص نمایشی که دیدیم، یک حل ساده وجود دارد که باید در دستگاه معادلات بالا صدق کند:**
>   (For the specific demonstration problem we saw, there is a simple solution that must satisfy the above system of equations:)
>   *(Diagram shows a particle moving along a straight line in the Lab frame at constant speed $v$.)*
> 
>   **In the Lab-frame:**
>   $$\vec{r}' = \vec{R}_0 - \vec{V}t \rightarrow \begin{cases} r' = R - vt \\ \theta' = 0 \end{cases}$$
> 
>   **Transforming to the rotating frame (تبدیل به دستگاه دوار):**
>   $$r = r' \rightarrow \dot{r} = -v, \quad \ddot{r} = 0$$
>   $$\theta' = \theta + \omega t \rightarrow \theta = \theta' - \omega t = -\omega t \rightarrow \dot{\theta} = -\omega, \quad \ddot{\theta} = 0$$
> 
>   *این مقادیر باید جواب دستگاه معادلات بالا باشد.* (These values must satisfy the system of equations above.)
>   Let's check:
>   - For equation (II):
>     $$2\dot{r}\dot{\theta} + r\ddot{\theta} = 2(-v)(-\omega) + 0 = 2v\omega$$
>     $$-2\omega\dot{r} = -2\omega(-v) = 2v\omega \quad \checkmark$$
>   - For equation (I):
>     $$\ddot{r} - r\dot{\theta}^2 = 0 - r(-\omega)^2 = -r\omega^2$$
>     $$2\omega r\dot{\theta} + \omega^2 r = 2\omega r (-\omega) + \omega^2 r = -2r\omega^2 + r\omega^2 = -r\omega^2 \quad \checkmark$$
>     *(Checked with a smiley face in the notes)*
> 
>   **So in the rotating frame (در دستگاه دوار داریم):**
>   $$\theta = -\omega t \rightarrow t = -\frac{\theta}{\omega}$$
>   $$r'(\theta) = R + \frac{v}{\omega}\theta$$

> **Elaboration:**
> In this section, we apply the non-inertial frame formalism to a concrete problem: a free bead sliding along a straight radial rail (or rod) that rotates with constant angular velocity $\vec{\omega} = \omega \hat{z}$.
> 
> 1. **Fictitious Force Reduction:** Since the bead is free to slide without friction along the rail ($\vec{F}=0$), the frame's origin is stationary ($\ddot{\vec{R}}_f=0$), and the rotation rate is constant ($\dot{\vec{\omega}}=0$), the only fictitious forces acting on the bead are the Centrifugal force and the Coriolis force.
> 2. **Polar Coordinate Equations of Motion:** We describe the bead's position relative to the rotating frame using polar coordinates $(r, \theta)$. Differentiating the position vector $\vec{r} = r \hat{r}$ yields the relative velocity $\vec{v}_r = \dot{r} \hat{r} + r\dot{\theta}\hat{\theta}$ and relative acceleration $\vec{a}_r = (\ddot{r} - r\dot{\theta}^2)\hat{r} + (2\dot{r}\dot{\theta} + r\ddot{\theta})\hat{\theta}$.
> 3. **Force Components:**
>    - The Centrifugal acceleration term is $-\vec{\omega} \times (\vec{\omega} \times \vec{r}) = \omega^2 r \hat{r}$ (directed radially outward).
>    - The Coriolis acceleration term is $-2\vec{\omega} \times \vec{v}_r = 2\omega r \dot{\theta} \hat{r} - 2\omega \dot{r} \hat{\theta}$.
> 4. **Equating Terms:** Equating components yields two differential equations of motion. 
> 
> **Solving via Frame Transformation:**
> Rather than solving these coupled differential equations directly, we can find a simple physical solution by observing the motion from the fixed Lab frame. In the Lab frame, a particle launched inward from radius $R$ at velocity $v$ moves in a straight line at constant speed ($r'(t) = R - vt$, $\theta' = 0$).
> 
> By transforming this simple straight-line motion into the rotating frame ($\theta = \theta' - \omega t = -\omega t$), we verify that it mathematically satisfies the rotating frame's equations of motion. 
> 
> Eliminating time $t$, the trajectory as seen by an observer rotating with the frame is:
> $$ r(\theta) = R + \frac{v}{\omega}\theta $$
> This is the equation of an **Archimedean spiral**. From the perspective of the rotating observer, the particle does not travel in a straight line; instead, the Coriolis and Centrifugal forces deflect it into a spiral path.

---

## 2. Motion Relative to the Earth (حرکت نسبت به زمین)

**Original Notes Transcription:**
> ■ **حرکت نسبت به زمین:** (Motion relative to the Earth:)
> *(Diagram shows Earth rotating with $\vec{\omega}$. A local lab frame is at latitude $\lambda$. A plumb bob is suspended with tension $\vec{T}$ and gravity $m\vec{g}$.)*
> 
> $$\vec{F}_{eff} = \vec{F} + m\vec{g}_0 - m\ddot{\vec{R}}_f - m\dot{\vec{\omega}}\times\vec{r} - m\vec{\omega}\times(\vec{\omega}\times\vec{r}) - 2m\vec{\omega}\times\vec{v}_r$$
> *(where $m\vec{g}_0$ is the true gravitational force and $\vec{F}$ is the non-gravitational force like tension $\vec{T}$.)*
> 
> - **وقتی درباره دستگاه دوار (شبیه زمین) صحبت می کنیم:**
>   (When we discuss a rotating frame (like Earth):)
>   *در چرخش زمین به دور خودش، چرخش به دور خورشید را صرف نظر می کنیم.*
>   (In Earth's rotation around itself, we neglect its rotation around the Sun.)
> 
>   1) $\dot{\vec{\omega}} = 0$
>   2) $\ddot{\vec{R}}_f = \vec{\omega} \times (\vec{\omega} \times \vec{R})$
> 
>   $$\rightarrow \vec{F}_{eff} = \vec{F} + m\vec{g}_{eff} - 2m\vec{\omega} \times \vec{v}_r$$
>   $$\vec{g}_{eff} = \vec{g}_0 - \vec{\omega} \times [\vec{\omega} \times (\vec{r} + \vec{R})] \approx \vec{g}_0 - \vec{\omega} \times (\vec{\omega} \times \vec{R}) \quad (\text{since } |\vec{r}| \ll |\vec{R}|)$$
> 
> **Boxed equations:**
> $$\vec{F}_{eff} = \vec{F} + m\vec{g}_{eff} - 2m\vec{\omega} \times \vec{v}_{rot}$$
> $$\vec{g}_{eff} \approx \vec{g}_0 - \vec{\omega} \times (\vec{\omega} \times \vec{R})$$
> 
> • **نکته:** اگر $r \sim R$ باشد، باید قانون گرانش $1/r^2$ را در نظر بگیریم.
> (Tip: If $r \sim R$, we must consider the $1/r^2$ law of gravity.)
> 
> (I) $-\omega^2 R \approx 0.034 \text{ m/s}^2 \approx 0.35\% \text{ g}$ (at the equatorial radius of the Earth / در استوای زمین)
> 
> (II) $\left|\frac{\Delta g}{g}\right| \sim 2 \left|\frac{\Delta R}{R}\right|$
> Using $\Delta R \approx 21.4 \text{ km} \rightarrow \sim 1.2 \times 10^{-2} \rightarrow \Delta g \approx 0.0183 \text{ m/s}^2$
> 
> - **خط شاقولی:** (Plumb line:)
> *(Diagram shows how centrifugal force $\vec{\omega}\times(\vec{\omega}\times\vec{R})$ shifts the local plumb line $\vec{g}_{eff}$ away from the true radial line $\vec{g}_0$.)*
> *(Diagram shows the angle of deviation $\theta$ of the plumb line from the true radial vector, reaching $\theta_{max}$ at mid-latitudes.)*
> 
> ■ **جریان های گردابی:** (Vortex currents / Cyclonic flows:)
> $$-2m\vec{\omega} \times \vec{v}_r$$
> *(Diagram shows Northern and Southern hemispheres of the Earth with Coriolis deflections.)*
> - In the Northern Hemisphere ($\omega_z > 0$):
>   *به راست منحرف می شود* (Deflected to the right)
> - In the Southern Hemisphere ($\omega_z < 0$):
>   *به چپ منحرف می شود* (Deflected to the left)

> **Elaboration:**
> This section translates the general non-inertial coordinate frame formulas specifically to the surface of the Earth, which is a rotating frame.
> 
> 1. **Effective Gravity ($\vec{g}_{eff}$):** 
>    The Earth rotates around its axis with constant angular velocity $\vec{\omega}$ (neglecting its orbital motion around the Sun for local mechanics). A particle on or near the Earth's surface experiences a true gravitational attraction $m\vec{g}_0$ toward the Earth's center. However, because of Earth's rotation, there is a centrifugal force. We group these two terms together to define the **effective gravitational acceleration**:
>    $$ \vec{g}_{eff} \approx \vec{g}_0 - \vec{\omega} \times (\vec{\omega} \times \vec{R}) $$
>    where $\vec{R}$ is the radius vector from the center of the Earth to the location on the surface.
> 
> 2. **Centrifugal Deviation (Plumb Line):**
>    The centrifugal term $-\vec{\omega} \times (\vec{\omega} \times \vec{R})$ points radially outward, perpendicular to the Earth's rotation axis. Except at the poles (where it is zero) and the equator (where it points directly opposite to gravity), this term tilts the net effective gravity vector $\vec{g}_{eff}$ away from the true radial direction toward the equator.
>    - A **plumb bob** hangs along the direction of $\vec{g}_{eff}$, not $\vec{g}_0$. This direction is called the **local vertical** or **plumb line**.
>    - The maximum deviation angle $\theta_{max}$ occurs at a latitude of $45^\circ$, where the tilt is roughly $0.1^\circ$.
>    - At the equator, the centrifugal acceleration is maximum ($-\omega^2 R \approx 0.034 \text{ m/s}^2$), reducing the effective gravity by about $0.35\%$.
>    - Because the Earth is fluid-like over geological times, this centrifugal force has caused the Earth to flatten into an oblate spheroid, with the equatorial radius being $\approx 21.4\text{ km}$ larger than the polar radius. This shape change itself causes a variation in gravity ($\Delta g \approx 0.0183 \text{ m/s}^2$).
> 
> 3. **Coriolis Force and Weather (جریان های گردابی):**
>    Any object moving with velocity $\vec{v}_r$ relative to the Earth experiences a Coriolis force $-2m\vec{\omega} \times \vec{v}_r$.
>    - **Northern Hemisphere:** The vertical component of Earth's rotation vector points upward ($\omega_z > 0$). Consequently, any moving particle is deflected to its **right**. This deflection is responsible for the counter-clockwise rotation of cyclones (low-pressure systems) in the Northern Hemisphere.
>    - **Southern Hemisphere:** The vertical component of Earth's rotation vector points downward ($\omega_z < 0$). Moving particles are deflected to their **left**, causing cyclones to rotate clockwise in the Southern Hemisphere.
