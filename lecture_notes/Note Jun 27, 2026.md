# Chapter 12: Coupled Oscillations and Normal Modes - Lecture: Jun 27, 2026

## 1. Linear Vibrations of Molecules (ارتعاشات خطی مولکول)

**Original Notes Transcription:**
> **Timeline / Headings:**
> - (Side note on Procrastination / TED-Talk):
>   - قانون پارکینسون (Parkinson's Law)
>   - Gratification Monkey, Deadline, Dopamine (دوپامین), Reward (پاداش), Expectation (انتظار).
> - **ارتعاشات مولکولی** (Molecular vibrations)
> - **آونگ های جفت شده** (Coupled pendulums)
> - **ریسمان بارگذاری شده** (Loaded string) $\checkmark$
> 
> ■ **مولکول خطی :** (Linear molecule:)
> *(Diagram of a $CO_2$ molecule: $O - C - O$. The masses are $m, M, m$. Their displacements are $x_1, x_2, x_3$. They are connected by effective springs of stiffness $K$. The whole molecule can undergo Translation).*
> 
> ■ **ارتعاشات خطی (طولی) مولکول :** (Linear (longitudinal) vibrations of the molecule:)
> *(Diagram shows $CO_2$ vibrating. The Oxygen atoms move outwards while the Carbon atom moves inwards to conserve momentum).*
> 
> **مرحله اول : حذف انتقال کل مولکول :**
> (Step 1: Eliminating the total translation of the molecule:)
> 
> **(i)** To keep the center of mass stationary:
> $$m(x_1 + x_3) + M x_2 = 0 \rightarrow x_2 = - \frac{m}{M}(x_1 + x_3)$$
> Taking the time derivative:
> $$\rightarrow \dot{x}_2 = - \frac{m}{M}(\dot{x}_1 + \dot{x}_3)$$
> 
> **(ii)** Kinetic Energy:
> $$T = \frac{1}{2} m \dot{x}_1^2 + \frac{1}{2} M \dot{x}_2^2 + \frac{1}{2} m \dot{x}_3^2$$
> Substituting $\dot{x}_2$:
> $$\rightarrow T = \frac{1}{2} m \dot{x}_1^2 + \frac{1}{2} m \dot{x}_3^2 + \frac{1}{2} M \left( - \frac{m}{M} \right)^2 (\dot{x}_1 + \dot{x}_3)^2$$
> $\rightarrow \text{mixing } \dot{x}_1 \dot{x}_3$ (cross terms appear, coupling the velocities).
> 
> **(iii)** Potential Energy:
> $$U = \frac{1}{2} K (x_2 - x_1)^2 + \frac{1}{2} K (x_3 - x_2)^2$$
> $\rightarrow$ همیشه جفت شدگی (Always coupled).
> *(Note: A graph shows a parabola $U \sim x^2$ indicating the "Effective Spring Description").*

> **Elaboration:**
> The lecture shifts from the mechanics of macroscopic rigid bodies to microscopic coupled oscillators, specifically modeling molecular vibrations. A Carbon Dioxide ($CO_2$) molecule is modeled as three masses connected by two identical springs. 
> 
> Since the molecule is free to move through space, its total motion includes translation (the whole molecule moving in one direction). We are only interested in internal vibrations, so we must mathematically "pin" the center of mass to zero. This constraint ($x_2 = -\frac{m}{M}(x_1+x_3)$) reduces our three variables ($x_1, x_2, x_3$) to just two ($x_1, x_3$).
> 
> However, substituting this constraint into the kinetic and potential energy equations creates "cross terms" (like $\dot{x}_1 \dot{x}_3$ and $x_1 x_3$). This means the motions of the two oxygen atoms are mathematically coupled; solving their differential equations directly would be messy.

---

## 2. Transforming Coordinates for Uncoupled Modes (تغییر مختصات برای مدهای غیر جفت شده)

**Original Notes Transcription:**
> ■ **حذف انتقال کل مولکول** (Eliminating total translation of the molecule)
> $$\{x_1, x_2, x_3\} \xrightarrow{\text{eliminating } x_2} \{x_1, x_3\}$$
> 
> ■ **انتخاب مختصات مناسب :** (Choosing suitable coordinates:)
> آیا می توانیم مختصات تعمیم یافته مناسبی را پیشنهاد کنید که محاسبات را ساده تر کند :
> (Can we suggest suitable generalized coordinates that simplify the calculations:)
> 
> Let's define new coordinates $q_1, q_2$:
> $$\{x_1, x_3\} \rightarrow \{q_1, q_2\}$$
> $$\begin{cases} q_1 \equiv x_3 + x_1 \\ q_2 \equiv x_3 - x_1 \end{cases} \rightarrow \begin{cases} x_3 = (q_1 + q_2) / 2 \\ x_1 = (q_1 - q_2) / 2 \\ x_2 = - \frac{m}{M} q_1 \end{cases}$$
> 
> ■ اگر بخواهیم فضای کنیم ، انرژی جنبشی و پتانسیل را در این مختصات جدید محاسبه کنید :
> (If we substitute these, calculate the kinetic and potential energy in these new coordinates:)
> 
> *(Diagram of two longitudinal modes:)*
> *Mode 1 (Symmetric stretch): $q_2 \neq 0, q_1 = 0$. The oxygen atoms move outward synchronously.*
> *Mode 2 (Asymmetric stretch): $q_1 \neq 0, q_2 = 0$. Both oxygen atoms move right, while the carbon moves left.*
> 
> در راستای محور طولی : (Along the longitudinal axis:)
> $$T = \frac{m}{4} \dot{q}_2^2 + \frac{(mM + 2m^2)}{4M} \dot{q}_1^2$$
> $$U = \frac{(2m + M)}{2M} K q_1^2 + \frac{1}{4} K q_2^2$$
> 
> ■ با این تغییر متغیر دو مد کاملاً مجزا (غیر جفت شده) داریم : 
> (With this change of variable, we have two completely separated (uncoupled) modes:)
> 
> $$\omega_1^2 = \frac{(2m + M)}{mM} K \quad \text{(Asymmetric mode frequency)}$$
> $$\omega_2^2 = \frac{K}{m} \quad \text{(Symmetric mode frequency)}$$
> 
> The general solution is a superposition:
> $$q_j = \sum_r a_{jr} \eta_r \rightarrow \begin{cases} \text{دامنه} \text{ (Amplitude)} \\ \text{فاز} \text{ (Phase)} \\ \text{ضرایب تعیین} \text{ (Determining coefficients)} \end{cases}$$
> (دارای شرط بهنجارش - Has normalization condition)
> 
> $$\begin{cases} q_1 = a_{11} \eta_1 + a_{12} \eta_2 \\ q_2 = a_{21} \eta_1 + a_{22} \eta_2 \end{cases}$$
> به دلیل انتخاب مختصات مناسب (Due to the choice of suitable coordinates):
> $$a_{12} = a_{21} = 0$$

> **Elaboration:**
> To untangle the coupled equations, we perform a clever change of variables, moving from physical coordinates ($x_1, x_3$) to "Normal Coordinates" ($q_1, q_2$).
> 
> We define $q_1 = x_3 + x_1$ and $q_2 = x_3 - x_1$. 
> - If only $q_2$ changes, the two oxygen atoms move in opposite directions symmetrically, while the center carbon remains perfectly still. 
> - If only $q_1$ changes, both oxygen atoms move in the same direction, forcing the carbon atom to move in the opposite direction to keep the CM fixed.
> 
> When we rewrite $T$ and $U$ in terms of $q_1$ and $q_2$, the cross terms miraculously disappear! The kinetic and potential energies are now sums of independent squares. This proves that $q_1$ and $q_2$ represent the **Normal Modes** of the system. The system behaves as two completely independent, uncoupled harmonic oscillators with frequencies $\omega_1$ and $\omega_2$.

---

## 3. Transverse Vibrations (ارتعاشات عرضی مولکولی)

**Original Notes Transcription:**
> ■ **ارتعاشات عرضی مولکولی** (Transverse molecular vibrations)
> *(Diagram of the $CO_2$ molecule bending. The central Carbon atom moves downwards ($y_2$) while the two Oxygen atoms move upwards ($y_1, y_3$). The bond angle bends by $\alpha$.)*
> 
> **(i)** Potential Energy from bending:
> $$U(\theta) = \frac{1}{2} K_\theta \theta^2 \rightarrow U = \frac{1}{2} (K b^2) \alpha^2 \quad (\text{where } K_\tau = K b^2)$$
> The bending angle $\alpha$ is related to displacements by:
> $$\alpha = \frac{(y_1 - y_2) + (y_3 - y_2)}{b}$$
> 
> **(ii)** Kinetic Energy:
> $$T = \frac{1}{2} m \dot{y}_1^2 + \frac{1}{2} m \dot{y}_3^2 + \frac{1}{2} M \dot{y}_2^2$$
> 
> **(iii)** Center of Mass Constraint:
> انتقال عرضی مرکز جرم را صفر فرض می کند . (Assumes zero transverse translation of the center of mass.)
> $$y_2 = - \frac{m}{M} (y_1 + y_3)$$
> 
> **(iv)** Symmetry Constraint (no pure rotation):
> *(Diagram shows total rotation is excluded).*
> $$y_1 = y_3$$
> 
> ■ با احتساب این قیود داریم : (Taking these constraints into account we have:)
> $$T = \frac{m}{M}(M + 2m)\dot{y}_1^2$$
> $$U = \frac{1}{2}(Kb^2)\alpha^2 \quad \text{where} \quad \alpha = \frac{2y_1}{bM}(2m + M)$$
> 
> *Boxed equation for bending mode frequency:*
> $$\omega_3^2 = \frac{2(M+2m)}{mM} K' \quad (\text{where } K_\tau = K' b^2)$$

> **Elaboration:**
> Besides stretching longitudinally, the $CO_2$ molecule can also bend in the transverse direction (like a bow). 
> 
> We assign transverse coordinates $y_1, y_2, y_3$ to the three atoms. Again, we apply constraints to isolate the pure vibrational mode:
> 1. We fix the center of mass in the y-direction (eliminating pure translation).
> 2. We force $y_1 = y_3$ (eliminating pure rigid-body rotation around the center).
> 
> By substituting these constraints into the kinetic and potential energy equations, the system reduces to a single degree of freedom (governed solely by $y_1$). The resulting equation yields the fundamental frequency $\omega_3$ for the bending mode.

---

## 4. Counting Degrees of Freedom (محاسبه درجات آزادی)

**Original Notes Transcription:**
> ■ **سؤال عملی :** ۳ تا اتم $\leftarrow$ ۳x۳ = ۹ مختصات
> (Practical question: 3 atoms $\leftarrow$ 3x3 = 9 coordinates/degrees of freedom)
> 
> We must subtract the rigid body motions to find the vibrational modes:
> - ۹ - ۳ (انتقال - translation) = ۶ degrees remaining
> - ۶ - ۳ (دوران کل - total rotation) = ۳ degrees remaining
> 
> The 3 remaining degrees of freedom represent the internal vibrational modes:
> - ۳ $\rightarrow$ ۱ طولی (longitudinal mode) 
> - ۲ عرضی (transverse bending modes in two perpendicular planes)

> **Elaboration:**
> A quick sanity check using the rule of degrees of freedom. A system of 3 independent atoms in 3D space has $3 \times 3 = 9$ total degrees of freedom. 
> We subtract 3 degrees for the translation of the center of mass (moving in x, y, z), and 3 degrees for the rigid rotation of the entire molecule around its axes. 
> This leaves exactly 3 internal vibrational degrees of freedom. For a linear molecule like $CO_2$, these correspond to the symmetric stretch, the asymmetric stretch, and the bending mode (which can happen in two perpendicular planes, technically making it degenerate).

---

## 5. Successive Pendulums Example (مثال آونگ های متوالی)

**Original Notes Transcription:**
> ■ **آونگ های متوالی $\leftarrow$ تقریب درجات آزادی جفتیده (۳ - درجه آزادی)**
> (Successive pendulums $\leftarrow$ approximation of coupled degrees of freedom (3 degrees of freedom))
> 
> با در نظر گرفتن انرژی پتانسیل و جنبشی داده شده در زیر ، مدهای نرمال این سیستم را محاسبه کنید:
> (Considering the kinetic and potential energy given below, calculate the normal modes of this system:)
> 
> *(Diagram of three identical pendulums of mass $m$ and length $l$, connected by springs. Their angular displacements are $\theta_1, \theta_2, \theta_3$).*
> 
> The given energies are:
> $$T = \frac{1}{2}(\dot{\theta}_1^2 + \dot{\theta}_2^2 + \dot{\theta}_3^2)$$
> $$U = \frac{1}{2}(\theta_1^2 + \theta_2^2 + \theta_3^2 - 2\varepsilon \theta_1 \theta_2 - 2\varepsilon \theta_1 \theta_3 - 2\varepsilon \theta_2 \theta_3)$$
> 
> *(Diagrams predict three normal modes:)*
> *1. All three swing in unison.*
> *2. The outer two swing oppositely, the middle one stays still.*
> *3. The outer two swing together, the middle one swings opposite.*
> 
> ■ **قدم اول :** (Step one: Construct Matrices)
> Mass matrix $[m]$:
> $$[m] = \begin{pmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{pmatrix}$$
> 
> Potential matrix $[A]$:
> $$[A] = \begin{pmatrix} 1 & -\varepsilon & -\varepsilon \\ -\varepsilon & 1 & -\varepsilon \\ -\varepsilon & -\varepsilon & 1 \end{pmatrix}$$
> 
> ■ **قدم دوم : حل معادله مشخصه :** (Step two: Solving the characteristic equation:)
> $$\det([A] - \omega^2[m]) = 0$$
> 
> $$\begin{vmatrix} 1 - \omega^2 & -\varepsilon & -\varepsilon \\ -\varepsilon & 1 - \omega^2 & -\varepsilon \\ -\varepsilon & -\varepsilon & 1 - \omega^2 \end{vmatrix} = 0$$
> 
> Solving this determinant yields three eigenfrequencies:
> *Boxed equations:*
> $$\omega_1 = \sqrt{1 + \varepsilon}$$
> $$\omega_2 = \sqrt{1 + \varepsilon}$$
> $$\omega_3 = \sqrt{1 - 2\varepsilon}$$
> 
> ■ **قدم سوم : یافتن ویژه بردارهای نرمال :** (Step three: Finding normal eigenvectors - left for next time).

> **Elaboration:**
> The lecture concludes with an advanced example: three coupled pendulums. Because the pendulums interact with each other via springs, their potential energy matrix contains off-diagonal cross terms ($-2\varepsilon \theta_1 \theta_2$, etc.). 
> 
> To find the normal modes, we set up the eigenvalue problem $\det(A - \omega^2 m) = 0$. Solving this $3 \times 3$ determinant yields a cubic equation in $\omega^2$. We find three roots, representing the three fundamental frequencies at which the system can oscillate. Interestingly, two of the frequencies are identical ($\omega_1 = \omega_2$), indicating a "degenerate" mode.
> 
> The final step, which is to plug these frequencies back in to find the exact shape (eigenvectors) of the normal modes, is noted as the next step.
