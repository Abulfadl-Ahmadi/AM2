Here is the comprehensive continuation of your study guide, covering the provided Pages 7 through 11. I have structured these into two major conceptual blocks: **Kinematics of Two-Body Scattering** and **Impulse & Rotational Dynamics (Sweet Spot)**, along with a concluding transition back to the formal definition of scattering cross-sections.

---

# Study Guide: Scattering Kinematics & Impulse Dynamics

## Block A: Kinematics of Two-Body Scattering (Pages 7 & 8)

> **Original Transcription (Persian):**
> *   **صفحات ۷ و ۸ - سینماتیک پراکندگی دو ذره‌ای:**
> *   *معادلات اصلی:*
>     *   $\tan\phi = \frac{\sin\theta}{\cos\theta + \frac{m_1}{m_2}}$
>     *   $\tan\xi = \cot\frac{\theta}{2}$
> *   *حالات خاص:*
>     *   (I) $m_1 = m_2 \implies \phi + \xi = \frac{\pi}{2}$
>     *   (II) $m_1 > m_2$
>     *   (III) $m_1 < m_2$
> *   *سرعت‌های مرکز جرم (CM):*
>     *   $|V_{cm}| = \frac{m_1|V_1|}{m_1+m_2}$
>     *   $|u'_1| = \frac{m_2|V_1|}{m_1+m_2}$
> *   *زاویه انحراف بیشینه:*
>     *   $\sin\phi_M = \frac{|u'_1|}{|V_{cm}|} = \frac{m_2}{m_1} \implies \phi_M = \sin^{-1}\frac{m_2}{m_1}$
> *   *مرز زاویه‌ای برای حالت $m_1 < m_2$:*
>     *   $\tan\phi = \frac{\sin\theta}{\cos\theta - \frac{m_1}{m_2}}$
>     *   $\theta_\Delta = \arccos(\frac{m_1}{m_2})$

### Expert Elaboration:
Pages 7 and 8 provide a geometric vector-based analysis of elastic scattering between two particles, specifically looking at the relationship between the **Laboratory (Lab) frame** and the **Center of Mass (CM) frame**.

*   **Geometric Relationship (Lab vs. CM Angle):**
    The formula $\tan\phi = \frac{\sin\theta}{\cos\theta + \frac{m_1}{m_2}}$ is critical. It relates the scattering angle in the Lab frame ($\phi$) to the scattering angle in the CM frame ($\theta$).
    *   $\theta$ is the angle at which particles collide if you are sitting at the center of mass.
    *   $\phi$ is the angle you observe if you are sitting stationary in the laboratory.
*   **Circle Diagrams (Page 8):** The blue circle diagrams represent the velocity vectors in the CM frame. The vector $\vec{V}_{CM}$ (center of mass velocity) is added to the relative velocity vector $\vec{u}'_1$ to find the Lab frame velocity $\vec{V}_1$.
*   **Special Cases:**
    *   **$m_1 = m_2$ (Equal masses):** This is a classic elastic collision scenario (like billiard balls). When masses are equal, the Lab frame scattering angle $\phi$ and the angle between the outgoing particles ($\xi$) always add up to $90^\circ$ ($\phi + \xi = \pi/2$).
    *   **$m_1 > m_2$ (Heavy incident, light target):** The velocity vector circle shows that the incident particle can never be scattered beyond a maximum angle $\phi_M$. The derivation $\sin\phi_M = m_2/m_1$ mathematically sets a physical limit. For example, if $m_1 = 2m_2$, the maximum possible Lab scattering angle is $30^\circ$.
    *   **$m_1 < m_2$ (Light incident, heavy target):** The target is heavy and acts like a wall. The formulas show a limit angle $\theta_\Delta$ in the CM frame. Since the heavy mass barely moves, the scattering patterns are heavily constrained. (Note: The notes briefly show that as $\theta \to \pi/2$, certain boundaries appear at $\arccos(m_1/m_2)$).

---

## Block B: Impulse & The "Sweet Spot" (Pages 9 & 10)

> **Original Transcription (Persian):**
> *   **صفحه ۹ - ضربه (Impulse):**
>     *   $F_{net} = \frac{d\vec{P}}{dt} \implies \Delta\vec{P} = \int_{t_0}^{t_0+\delta t} \vec{F}(t)dt \equiv \vec{J}$ (قانون ضربه)
>     *   $F_d = \frac{1}{2} C \rho A V^2$ (نیروی درگ)
>     *   *مثال:* $J = \Delta P = M V_{cm} \implies V_{cm} = \frac{J}{M}$ (حرکت انتقالی)
>     *   $\vec{\tau} = \frac{d\vec{L}}{dt} \implies \Delta\vec{L} = \int_{t_0}^{t_0+\delta t} \vec{\tau}(t)dt$ (ضربه چرخشی)
> *   **صفحه ۱۰ - نقطه شیرین (Sweet Spot) در چوب بیسبال:**
>     *   $|\vec{\tau}_{cm}| = |\vec{F}(t)| d$
>     *   $\int |\tau(t)|dt = (\int |F(t)|dt) d = J \times d$
>     *   $\implies J \times d = \Delta L = I_{cm} \times \Delta\omega$
>     *   $\omega = \frac{Jd}{I_{cm}}$ و $V_{cm} = \frac{J}{M}$
>     *   $V_A = V_{cm} - \omega \times \frac{l}{2} = \frac{J}{M} - \frac{Jd}{I_{cm}} \times \frac{l}{2}$ (سرعت انتهای چوب)
>     *   $V_A=0 \implies d = \frac{2I_{cm}}{Ml} = \frac{\frac{1}{12}Ml^2}{Ml/2} = \frac{l}{6}$
>     *   $d = l/6 \implies D = \frac{l}{6} + \frac{l}{2} = \frac{2l}{3}$
>     *   **Sweet Spot!**

### Expert Elaboration:
Pages 9 and 10 switch from microscopic particle scattering to macroscopic rigid body dynamics. This is a classic derivation showing the physics behind the "Sweet Spot" of a baseball bat (or any struck rod).

*   **Impulse Definition:**
    The lecture establishes that Impulse ($\vec{J}$) is the integral of a time-varying force. In real collisions (like hitting a ball), force is not constant; it spikes briefly over a small time $\delta t$. The area under the Force-Time curve is the impulse, which equals the total change in linear momentum ($\Delta\vec{P}$).
*   **Translational vs. Rotational Motion (Page 10):**
    When an external impulse is applied to a rigid body at a distance $d$ from its center of mass (CM):
    1.  **Translational:** The impulse forces the entire object's center of mass to move forward with velocity $V_{cm} = J/M$.
    2.  **Rotational:** Because the force is applied *off-center*, it creates a torque about the CM. Integrating this torque over time yields an angular impulse, resulting in an angular velocity $\omega = \frac{Jd}{I_{cm}}$.
*   **The Sweet Spot Calculation:**
    When you hit a baseball bat, the handle is gripped by a hand. You do *not* want the bat to violently vibrate or translate in your hands; you want it to rotate smoothly.
    *   The velocity of the bat's handle (the point of grip at distance $-l/2$ from the CM) is $V_{cm} - \omega(l/2)$ (Note: the direction of $\omega$ makes the end opposite to the impact move backward).
    *   For the hand to feel minimal jarring (zero velocity at the handle), we set $V_A = 0$.
    *   **Derivation:** $\frac{J}{M} - \frac{Jd}{I_{cm}}\cdot\frac{l}{2} = 0 \implies d = \frac{2I_{cm}}{Ml}$. Using $I_{cm} = \frac{1}{12}Ml^2$ for a uniform rod, we get $d = \frac{l}{6}$.
    *   **The Result:** This tells us the impact point must be $l/6$ *away* from the center of mass. The center of mass is at $l/2$ from the handle. Therefore, the total distance from the handle is $D = \frac{l}{2} + \frac{l}{6} = \frac{2l}{3}$. This point is known as the center of percussion (COP) or commonly the "sweet spot".
    *   *Note:* In a real baseball bat, the shape isn't uniform, so the $2l/3$ distance is an approximation, but the physics principle remains exact.

---

## Block C: Return to Scattering Cross-Section (Page 11)

> **Original Transcription (Persian):**
> *   **صفحه ۱۱ - تعریف سطح مقطع پراکندگی:**
> *   *تصویر:* پرتو ذرات ورودی با شدت $I$ به هدف برخورد کرده و در زاویه $\theta$ تا $\theta+d\theta$ پراکنده می‌شوند.
> *   $dN_s(\theta, \theta+d\theta)$: تعداد ذرات پراکنده شده در بازه زاویه‌ای $d\theta$.
> *   (تعریف اصلی ذکر نشده است، اما پارامترهای ورودی/خروجی مشخص شده‌اند).

### Expert Elaboration:
Page 11 serves as a transitional page. It is the conceptual setup for the first set of your notes (Pages 1-6). It graphically represents the physical setup of a scattering experiment:
*   **Incident Flux ($I$):** A parallel beam of particles hits a target. Every particle has the same impact parameter, or a distribution of impact parameters.
*   **The Target:** Represented as an atom or small molecule.
*   **Scattering:** After the interaction, the particles are deflected into various angles. The highlighted cone represents a tiny solid angle $d\Omega$ defined by the scattering angles $\theta$ and $\theta+d\theta$.
*   **Goal:** By counting the number of particles scattered into that specific angle ($dN_s$), and knowing the incoming flux ($I$), physicists can derive the **Differential Cross-Section** ($\sigma(\theta)$) studied in Pages 1 and 2. This allows us to map the invisible forces of the target particle mathematically.