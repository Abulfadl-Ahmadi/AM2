# Chapter 10: Motion in Non-Inertial Reference Frames - Lecture: May 2, 2026

> [!abstract] Navigation
> **Chapter:** [[Chapter 10 - Non-Inertial Reference Frames]] | **Prev:** [[Note Apr 27, 2026]] | **Next:** [[Note May 4, 2026]] | [[Lecture Index|📚 All Lectures]]
>
> **Key concepts:** Rotating frames, fictitious forces (Coriolis, centrifugal)

## 1. Introduction and Vector Definitions (تعاریف اولیه و دستگاه های مختصات)

**Original Notes Transcription:**
> **Timeline:** Congress $\rightarrow$ China $\rightarrow$ Hit & Run Hollywood $\rightarrow$ World Cup 2026
> **Egocentric**
> 
> - **اقتصاد دانان رسمی:** (Official economists:)
>   1 month $\sim$ 1 year $\leftarrow \times 2 \left( 50 \$ / \text{b} \rightarrow 100 \$ / \text{b} \right) \times 5 \left( 300,000 \text{ barrel/day} \rightarrow 1.5 \text{ million b/d} \right)$
> 
>   SWIFT $\rightarrow$ transaction $\rightarrow$ INSTEX $\rightarrow \sim 10 \text{ million } \$$ $\infty$ ☹
>   CIPS
> 
> ■ **فرمالیزم کارکردن در دستگاه نالخت:** (Formalism of working in non-inertial frames:)
> - **تعاریف اولیه:** (Initial definitions:)
>   Let the fixed (inertial) system be the Lab frame with coordinates $(x'_1, x'_2, x'_3)$ and origin $O'$.
>   Let the moving (non-inertial) system be the rotating frame with coordinates $(n_1, n_2, n_3)$ and origin $O$.
>   The position vector of a particle $P$ is:
>   - $\vec{r}'$ in the Lab frame.
>   - $\vec{r}$ in the rotating/moving frame.
>   - $\vec{R}$ is the vector from origin $O'$ to origin $O$.
> 
>   $$\vec{r}' = \vec{R} + \vec{r}$$
> 
> - **نکته حیاتی (ریاضی):** (Vital mathematical tip:)
>   For a rotating vector $\vec{V}$ with constant magnitude ($|\vec{V}| = \text{const}$):
>   $$\rightarrow \frac{d\vec{V}}{dt} = \vec{\omega} \times \vec{V}$$

> **Elaboration:**
> The lecture begins with a brief macro-economic tangent outlining oil prices, trade mechanisms (SWIFT, INSTEX, and China's CIPS), and their global timescales, before introducing the core mechanics topic: **Non-Inertial Reference Frames**.
> 
> When analyzing motion in classical mechanics, Newton's Laws are only valid in inertial frames (reference frames that are not accelerating or rotating). To describe motion in a non-inertial frame, we establish two coordinate systems:
> 1. A **fixed (Inertial) frame** (e.g., the Lab frame) with origin $O'$.
> 2. A **moving (Non-Inertial) frame** with origin $O$, which can translate (represented by $\vec{R}(t)$) and rotate (with angular velocity $\vec{\omega}(t)$) relative to the inertial frame.
> 
> The position vector of a particle $P$ relative to the inertial frame $\vec{r}'$ is simply the vector sum of the position of the moving frame's origin $\vec{R}$ and the position of the particle relative to the moving frame $\vec{r}$.
> 
> Additionally, a vital mathematical lemma is introduced: if a vector $\vec{V}$ has a constant length ($|\vec{V}| = \text{const}$) but is rotating with angular velocity $\vec{\omega}$, its rate of change in the fixed frame is given by the cross product $\vec{\omega} \times \vec{V}$. This is because the change in $\vec{V}$ is purely directional and perpendicular to both $\vec{\omega}$ and $\vec{V}$.

---

## 2. Time Derivatives in Rotating Frames (مشتق زمانی در دستگاه های دوار)

**Original Notes Transcription:**
> **\* پرونده امروز ما** (Today's case/agenda)
> **• ریاضی:** (Mathematics)
> $$\vec{r}'(t) \leftarrow \left(\frac{d\vec{r}'}{dt}\right)_{fixed} \leftarrow \frac{d^2\vec{r}'}{dt^2} \leftarrow \text{قوانین نیوتن (لخت)}$$
> $$\Downarrow$$
> $$\frac{d^2\vec{r}'}{dt^2} \rightarrow \frac{d^2\vec{r}}{dt^2} \rightarrow \text{قوانین نیوتن اصلاح شده}$$
> 
> **قدم ۱) سؤال:** فرض کنید بردار $\vec{r} = \text{const}$ در دستگاه دوار داریم.
> *(برای سادگی فرض کنید $\vec{R} = 0$)*
> $$\{x_i\} \rightarrow \{x_1, x_2, x_3\} = \text{const}$$
> $$\rightarrow \left(\frac{d\vec{r}}{dt}\right)_{fixed} = \vec{\omega} \times \vec{r}$$
> 
> **قدم ۲) سؤال:** اگر $\vec{r}$ در دستگاه دوار نیز دارای تغییرات باشد، رابطه به چه صورت تصحیح می شود؟
> $$\left(\frac{d\vec{r}}{dt}\right)_{fixed} = \left(\frac{d\vec{r}}{dt}\right)_{rot} + \vec{\omega} \times \vec{r}$$
> *طوری می نویسیم که پایه های فضا دارای مشتق نباشند.*
> 
> **نکته:** اگر همین را برای هر بردار دلخواه $\vec{Q}$ بنویسیم چگونه خواهد بود:
> $$\left(\frac{d\vec{Q}}{dt}\right)_{fixed} = \left(\frac{d\vec{Q}}{dt}\right)_{rot} + \vec{\omega} \times \vec{Q}$$
> 
> **Proof/Derivation:**
> $$\vec{Q} = \sum_i Q_i \hat{e}_i$$
> $$\rightarrow \frac{d\vec{Q}}{dt} = \sum_i \dot{Q}_i \hat{e}_i \text{ (I)} + \sum_i Q_i \dot{\hat{e}}_i$$
> Since the basis vectors $\hat{e}_i$ are rotating:
> $$\dot{\hat{e}}_i = \vec{\omega} \times \hat{e}_i \text{ (II)}$$
> 
> **• نکته:** به طور خاص اگر $\vec{Q} = \vec{\omega}$ را در نظر بگیریم، داریم:
> $$\left(\frac{d\vec{\omega}}{dt}\right)_{fixed} = \left(\frac{d\vec{\omega}}{dt}\right)_{rot}$$
> *چرا که $\vec{\omega} \times \vec{\omega} = 0$ !*

> **Elaboration:**
> The primary mathematical challenge is establishing how time derivatives of vectors differ when observed from the inertial (fixed) frame versus the rotating frame.
> 
> In Newton's second law, acceleration is the second time derivative in the fixed frame ($\frac{d^2\vec{r}'}{dt^2}$). We want to express this in terms of derivatives in the rotating frame ($\frac{d^2\vec{r}}{dt^2}$).
> 
> 1. **Step 1 (Stationary Vector in Rotating Frame):** If a particle is at rest in the rotating frame ($\vec{r} = \text{const}$ relative to rotating axes), it still moves as observed from the fixed frame due to rotation. Its velocity in the fixed frame is purely $\vec{\omega} \times \vec{r}$.
> 2. **Step 2 (Moving Vector in Rotating Frame):** If the particle is also moving relative to the rotating axes, its velocity in the fixed frame must include the rate of change as seen in the rotating frame, leading to the **Transport Theorem**:
>    $$ \left(\frac{d\vec{r}}{dt}\right)_{fixed} = \left(\frac{d\vec{r}}{dt}\right)_{rot} + \vec{\omega} \times \vec{r} $$
> 
> We prove this by writing any vector $\vec{Q}$ in terms of the rotating unit basis vectors $\hat{e}_i$: $\vec{Q} = \sum Q_i \hat{e}_i$. Differentiating this gives two terms:
> - **Term I:** The derivative of the scalar components $\sum \dot{Q}_i \hat{e}_i$, which is exactly $\left(\frac{d\vec{Q}}{dt}\right)_{rot}$.
> - **Term II:** The derivative of the basis vectors $\sum Q_i \dot{\hat{e}}_i$. Because the basis vectors rotate with angular velocity $\vec{\omega}$, their derivatives are $\dot{\hat{e}}_i = \vec{\omega} \times \hat{e}_i$. Summing this up yields $\vec{\omega} \times \vec{Q}$.
> 
> Interestingly, if we apply this to the angular velocity vector itself ($\vec{Q} = \vec{\omega}$), the rotation term vanishes ($\vec{\omega} \times \vec{\omega} = 0$). Thus, the angular acceleration $\dot{\vec{\omega}}$ is identical in both the fixed and rotating frames.

---

## 3. Velocity Transformation (محاسبه سرعت)

**Original Notes Transcription:**
> **■ پروژه اصلی:** (Main project:)
> **گام اول: محاسبه $\left(\frac{d\vec{r}'}{dt}\right)_{fixed}$:**
> $$\vec{r}' = \vec{R} + \vec{r} \rightsquigarrow \left(\frac{d\vec{r}'}{dt}\right)_{fixed} = \left(\frac{d\vec{R}}{dt}\right)_{fixed} + \left(\frac{d\vec{r}}{dt}\right)_{fixed}$$
> 
> Let:
> - $\left(\frac{d\vec{R}}{dt}\right)_{fixed} \equiv \vec{V}$ (Relative velocity of the origins of the two frames / سرعت نسبی مبداهای دو دستگاه)
> - $\left(\frac{d\vec{r}}{dt}\right)_{fixed} = \left(\frac{d\vec{r}}{dt}\right)_{rot} + \vec{\omega} \times \vec{r}$
> - Let the velocity observed in the rotating frame be $\left(\frac{d\vec{r}}{dt}\right)_{rot} \equiv \vec{v}_r$.
> - Let the velocity observed in the fixed frame be $\left(\frac{d\vec{r}'}{dt}\right)_{fixed} \equiv \vec{v}_f$.
> 
> $$\vec{v}_f = \vec{V} + \vec{v}_r + \vec{\omega} \times \vec{r}$$

> **Elaboration:**
> We apply the Transport Theorem to find the velocity of a particle in the fixed frame ($\vec{v}_f$) given its coordinates in the moving frame. 
> Differentiating the position vector relation $\vec{r}' = \vec{R} + \vec{r}$ yields:
> - The term $\frac{d\vec{R}}{dt}$ represents the translational velocity $\vec{V}$ of the moving frame's origin.
> - The term $\frac{d\vec{r}}{dt}$ is expanded using the Transport Theorem into the velocity relative to the rotating frame ($\vec{v}_r$) and the rotational velocity ($\vec{\omega} \times \vec{r}$).
> 
> Thus, the total velocity in the fixed frame is the vector sum of three components:
> 1. The translation velocity of the frame itself ($\vec{V}$).
> 2. The relative velocity of the particle inside the frame ($\vec{v}_r$).
> 3. The tangential velocity due to the rotation of the frame ($\vec{\omega} \times \vec{r}$).

---

## 4. Acceleration Transformation and Fictitious Forces (محاسبه شتاب و نیروهای مجازی)

**Original Notes Transcription:**
> **■ گام دوم: محاسبه نیروهای مجازی (لختی / اصلاحی):**
> (Step 2: Calculating virtual/fictitious forces:)
> $$\vec{F} = m\vec{a} \rightarrow \vec{F}_{tot} = m\vec{a}_f = m \left(\frac{d\vec{v}_f}{dt}\right)_{fixed}$$
> *اصرار بر دستگاه نالخت (Insisting on the non-inertial frame)*
> *کاربری اصرار دارد که در دستگاه نالخت آموزش خود را ادامه دهد:*
> 
> $$\left(\frac{d\vec{v}_f}{dt}\right)_{fixed} = \left(\frac{d\vec{V}}{dt}\right)_{fixed} + \left(\frac{d\vec{v}_r}{dt}\right)_{fixed} + \dot{\vec{\omega}} \times \vec{r} + \vec{\omega} \times \left(\frac{d\vec{r}}{dt}\right)_{fixed}$$
> 
> Let's analyze the terms:
> - $\left(\frac{d\vec{V}}{dt}\right)_{fixed} = \ddot{\vec{R}}_f$ (Translational acceleration of the frame origin)
> - (ii) $\left(\frac{d\vec{v}_r}{dt}\right)_{fixed} = \left(\frac{d\vec{v}_r}{dt}\right)_{rot} + \vec{\omega} \times \vec{v}_r = \vec{a}_r + \vec{\omega} \times \vec{v}_r$
> - (iii) $\vec{\omega} \times \left(\frac{d\vec{r}}{dt}\right)_{fixed} = \vec{\omega} \times \left[ \left(\frac{d\vec{r}}{dt}\right)_{rot} + \vec{\omega} \times \vec{r} \right] = \vec{\omega} \times \vec{v}_r + \vec{\omega} \times (\vec{\omega} \times \vec{r})$
> 
> Combining all terms:
> $$\vec{a}_f = \vec{a}_r + \ddot{\vec{R}}_f + \dot{\vec{\omega}} \times \vec{r} + 2\vec{\omega} \times \vec{v}_r + \vec{\omega} \times (\vec{\omega} \times \vec{r})$$
> 
> $$\vec{F} = m\vec{a}_f \rightarrow m\vec{a}_r = \vec{F} - m\ddot{\vec{R}}_f - m\dot{\vec{\omega}} \times \vec{r} - 2m\vec{\omega} \times \vec{v}_r - m\vec{\omega} \times (\vec{\omega} \times \vec{r})$$
> 
> Let the effective force in the rotating frame be $\vec{F}_{eff} = m\vec{a}_r$.
> $$\vec{F}_{eff} = \vec{F} - m\ddot{\vec{R}}_f - m\dot{\vec{\omega}} \times \vec{r} - 2m\vec{\omega} \times \vec{v}_r - m\vec{\omega} \times (\vec{\omega} \times \vec{r})$$
> *(Where $\vec{F}$ is the real force / نیروی واقعی)*
> 
> **نسخه تصحیح شده برای به کارگیری قانون دوم نیوتن**
> **Mission Unlocked!**
> 
> *(Diagram shows a rotating system with angular acceleration $\dot{\vec{\omega}} \neq 0$ and tangent/radial axes, illustrating tangential force throttle and radial direction)*
> 
> **■ سؤال:** (Question:)

> **Elaboration:**
> To find the acceleration in the fixed frame ($\vec{a}_f$), we differentiate the velocity equation $\vec{v}_f = \vec{V} + \vec{v}_r + \vec{\omega} \times \vec{r}$ with respect to time in the fixed frame.
> 1. Differentiating $\vec{V}$ gives the translational acceleration of the frame's origin, $\ddot{\vec{R}}_f$.
> 2. Differentiating $\vec{v}_r$ (which is defined in the rotating frame) requires applying the Transport Theorem, yielding the relative acceleration $\vec{a}_r$ plus $\vec{\omega} \times \vec{v}_r$.
> 3. Differentiating the cross product $\vec{\omega} \times \vec{r}$ yields $\dot{\vec{\omega}} \times \vec{r} + \vec{\omega} \times \left(\frac{d\vec{r}}{dt}\right)_{fixed}$. Expanding this second part gives another $\vec{\omega} \times \vec{v}_r$ term and the centripetal term $\vec{\omega} \times (\vec{\omega} \times \vec{r})$.
> 
> Summing these up, we obtain the full expression for acceleration in the inertial frame ($\vec{a}_f$). By multiplying by mass $m$ and using Newton's Second Law ($\vec{F} = m\vec{a}_f$), we can solve for $m\vec{a}_r$, which represents the apparent mass times acceleration in the rotating frame.
> 
> This defines the **Effective Force ($\vec{F}_{eff}$)** in the rotating frame, which is the real force $\vec{F}$ plus four **fictitious (or inertial) forces**:
> 1. **Translational Inertial Force** ($-m\ddot{\vec{R}}_f$): Apparent force due to the acceleration of the coordinate origin.
> 2. **Euler Force** ($-m\dot{\vec{\omega}} \times \vec{r}$): Apparent force due to angular acceleration of the frame.
> 3. **Coriolis Force** ($-2m\vec{\omega} \times \vec{v}_r$): Apparent force acting on a moving body within a rotating frame, perpendicular to both velocity and the rotation axis.
> 4. **Centrifugal Force** ($-m\vec{\omega} \times (\vec{\omega} \times \vec{r})$): Apparent force pointing radially outward, away from the rotation axis.
