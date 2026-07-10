# Chapter 12: Coupled Oscillations and Normal Modes (Continued) - Lecture: Jun 29, 2026

> [!abstract] Navigation
> **Chapter:** [[Chapter 12 - Coupled Oscillations and Normal Modes]] | **Prev:** [[Note Jun 27, 2026]] | [[Lecture Index|📚 All Lectures]]
>
> **Key topics:** [[Eigenvalue Problem for Normal Modes|Degeneracy handling]], loaded string vibrations

## 1. Finding the Normal Modes of Coupled Pendulums (یافتن مدهای نرمال آونگ های جفت شده)

**Original Notes Transcription:**
> **Timeline / Headings:**
> - به نام هستی بخش (In the name of the life giver)
> 
> Continuing the problem of 3 coupled pendulums:
> $$T = \frac{1}{2} (\dot{\theta}_1^2 + \dot{\theta}_2^2 + \dot{\theta}_3^2)$$
> $$U = \frac{1}{2} (\theta_1^2 + \theta_2^2 + \theta_3^2 - 2\varepsilon \theta_1 \theta_2 - 2\varepsilon \theta_1 \theta_3 - 2\varepsilon \theta_2 \theta_3)$$
> *(Note: The $\frac{1}{2}(\theta_1^2 + \theta_2^2 + \theta_3^2)$ part corresponds to the "mass-term" equivalent in the potential).*
> 
> ■ **راه حل برای یافتن $\omega$ :** (Solution to find $\omega$ :)
> $$\{A\}, \{m\} \xrightarrow{\text{معادله مشخصه (Characteristic Equation)}} | \{A\} - \{m\}\omega^2 | = 0 \rightarrow \omega_r^2 = ?$$
> 
> ■ **قدم اول :** (Step one: The Matrices)
> $$\{m\} = \begin{pmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{pmatrix} \quad \text{and} \quad \{A\} = \begin{pmatrix} 1 & -\varepsilon & -\varepsilon \\ -\varepsilon & 1 & -\varepsilon \\ -\varepsilon & -\varepsilon & 1 \end{pmatrix}$$
> 
> ■ **قدم دوم : ویژه مقدارها :** (Step two: Eigenvalues / Frequencies)
> Setting the determinant to zero:
> $$(1-\omega^2)^3 - 2\varepsilon^3 - 3\varepsilon^2(1-\omega^2) = 0$$
> Solving yields:
> $$\begin{cases} \omega_1 = \sqrt{1+\varepsilon} \\ \omega_2 = \sqrt{1+\varepsilon} \end{cases} \rightarrow \text{تبهگنی (Degeneracy)}$$
> $$\omega_3 = \sqrt{1-2\varepsilon}$$
> 
> ■ **قدم سوم : ویژه حالت ها (حالت های هنجار) :** (Step three: Eigenstates (Normal states))
> We find the eigenvectors $\vec{a}_r$ by solving:
> $$\sum_j (A_{jk} - \omega_r^2 m_{jk}) a_{jr} = 0$$
> 
> **For the non-degenerate root $r = 3 \quad (\omega_3 = \sqrt{1-2\varepsilon})$:**
> For $k=1$:
> $$\sum_j (A_{j1} - (1-2\varepsilon) m_{j1}) a_{j3} = 0$$
> $$[A_{11} - (1-2\varepsilon)\overbrace{m_{11}}^{1}]a_{13} + [A_{21} - (1-2\varepsilon)\overbrace{m_{21}}^{0}]a_{23} + [A_{31} - (1-2\varepsilon)\overbrace{m_{31}}^{0}]a_{33} = 0$$
> $$+2\varepsilon a_{13} - \varepsilon a_{23} - \varepsilon a_{33} = 0 \rightarrow 2a_{13} - a_{23} - a_{33} = 0$$
> 
> For $k=2$:
> $$-a_{13} + 2a_{23} - a_{33} = 0$$
> 
> Solving these together yields:
> $$a_{13} = a_{23} = a_{33}$$
> Applying the normalization condition ($\{m\} \rightarrow \{I\}$, length = 1):
> $$\vec{a}_3 = \frac{1}{\sqrt{3}} \begin{pmatrix} 1 \\ 1 \\ 1 \end{pmatrix}$$

> **Elaboration:**
> The lecture starts by finishing the 3-coupled-pendulum problem from the previous session. We apply the standard procedure: define the $T$ matrix ($m$) and $U$ matrix ($A$), solve the secular determinant $|A - \omega^2 m| = 0$ for the normal frequencies $\omega_r$, and then plug those frequencies back into the matrix equation $(A - \omega^2 m)\vec{a} = 0$ to find the normal mode shapes (eigenvectors) $\vec{a}_r$. 
> 
> For the third frequency ($\omega_3 = \sqrt{1-2\varepsilon}$), solving the system shows that all three pendulums move with exactly the same amplitude and phase. We normalize the vector to have a magnitude of 1.

---

## 2. Dealing with Degeneracy (مساله تبهگنی)

**Original Notes Transcription:**
> ■ **قدم چهارم :** $\vec{a}_1, \vec{a}_2 = ?$ (Step four: Finding eigenvectors for degenerate roots)
> 
> **For the degenerate roots $r = 1, 2 \quad (\omega_1 = \omega_2 = \sqrt{1+\varepsilon})$:**
> For $r=1, k=1$:
> $$\sum_j (A_{j1} - (1+\varepsilon) m_{j1}) a_{j1} = 0$$
> $$(\overbrace{A_{11}}^{1} - (1+\varepsilon)\overbrace{m_{11}}^{1}) a_{11} + (A_{21}) a_{21} + (A_{31}) a_{31} = 0$$
> $$-\varepsilon a_{11} - \varepsilon a_{21} - \varepsilon a_{31} = 0$$
> $$\rightarrow a_{11} + a_{21} + a_{31} = 0 \quad \text{for } r=1 \text{ (Eq. I)}$$
> 
> Similarly for $r=2$:
> $$a_{12} + a_{22} + a_{32} = 0 \quad \text{for } r=2 \text{ (Eq. II)}$$
> 
> If we check $k=2$, it gives a redundant equation (تکراری):
> $$a_{11} + a_{21} + a_{31} = 0$$
> *(Drawing of a confused face because we have five equations for six unknowns!)*
> 
> **شرط تعامد (و بهنجار بودن) :** (+ Orthogonality condition (and normalization))
> We enforce that eigenvectors must be orthogonal to each other:
> $$\vec{a}_1 \cdot \vec{a}_2 = 0 \rightarrow a_{11} a_{12} + a_{21} a_{22} + a_{31} a_{32} = 0 \quad \text{(Eq. iii)}$$
> Normalization:
> $$a_{11}^2 + a_{21}^2 + a_{31}^2 = 1 \quad \text{(Eq. iv)}$$
> $$a_{12}^2 + a_{22}^2 + a_{32}^2 = 1 \quad \text{(Eq. v)}$$
> 
> ⚠️ پنج معادله برای شش مجهول : (Five equations for six unknowns:)
> This means we have a free choice. We can set one component to zero to simplify.
> Let's choose $a_{31} = 0$:
> $$\vec{a}_1 = \frac{1}{\sqrt{2}} \begin{pmatrix} 1 \\ -1 \\ 0 \end{pmatrix} \quad \checkmark\checkmark \text{ Level Unlocked !}$$
> Using orthogonality, we then find $\vec{a}_2$:
> $$\vec{a}_2 = \frac{1}{\sqrt{6}} \begin{pmatrix} 1 \\ 1 \\ -2 \end{pmatrix}$$
> (And we already found $\vec{a}_3 = \frac{1}{\sqrt{3}} (1, 1, 1)^T$).

> **Elaboration:**
> Degeneracy happens when two or more normal frequencies are identical (here $\omega_1 = \omega_2$). When we plug this frequency back into the matrix equation, we don't get a unique line for the eigenvector; we get an entire 2D plane of possible solutions ($a_{11} + a_{21} + a_{31} = 0$).
> 
> This means we don't have enough equations to uniquely determine $\vec{a}_1$ and $\vec{a}_2$. We only have 5 constraints (2 from the eigenvalue equation, 1 from orthogonality, and 2 from normalization) but 6 unknowns. 
> 
> The physical meaning is that *any* two orthogonal vectors in that 2D plane are valid normal modes! We are free to make an arbitrary choice for one parameter (like $a_{31} = 0$) to lock in a specific basis. The "Level Unlocked!" note celebrates overcoming this mathematical hurdle.

---

## 3. Vibrations of a Loaded String (مساله ارتعاشات ریسمان بارگذاری شده)

**Original Notes Transcription:**
> ■ **مساله ارتعاشات ریسمان بارگذاری شده :** (Problem of vibrations of a loaded string:)
> *(Diagram of a string fixed at $x=0$ and $x=L$. There are $n$ masses of mass $m$ attached at equal intervals $d$. The equilibrium position is the straight line (خط تعادل). We ignore the mass of the wire itself).*
> Boundary conditions: $q_0 = 0$ (at node 0) and $q_{n+1} = 0$ (at node n+1).
> 
> ■ **حال در این ریسمان یک اختلال را بررسی می کنیم :** (Now we examine a perturbation in this string:)
> Assumption: small displacements ($k \Delta x \ll \tau$, where $\tau$ is initial tension).
> 
> *(Diagram of three adjacent masses $j-1, j, j+1$ displaced vertically by $q_{j-1}, q_j, q_{j+1}$. The angles of the string segments are $\theta_{j, j-1}$ and $\theta_{j+1, j}$.)*
> For small angles ($\theta \ll 1$):
> $$\theta_{j, j-1} = \frac{q_j - q_{j-1}}{d}$$
> $$\theta_{j+1, j} = \frac{q_{j+1} - q_j}{d}$$
> 
> The total restoring force on mass $j$ is the sum of the tension components:
> $$F_{tot} = - \tau [ \sin \theta_{j, j-1} + \sin \theta_{j+1, j} ] \xrightarrow{\sin \theta \simeq \theta} F_j = - \frac{\tau}{d} [ 2 q_j - q_{j+1} - q_{j-1} ]$$
> *(Dimensional analysis check: $[\tau] = MLT^{-2}$, $[d] = L$, $[q] = L$. The units match).*
> 
> ■ اگر قرار باشد ، یک پتانسیل معرفی کنیم که منجر به قانون نیوتون بالا شود ، داریم :
> (If we are to introduce a potential that leads to the above Newton's law, we have:)
> $$U = \frac{\tau}{2d} \sum_{j=1}^{n+1} (q_j - q_{j-1})^2$$
> Verifying by taking the derivative:
> $$F_k = - \frac{\partial U}{\partial q_k} = - \frac{\tau}{2d} \sum_{j=1}^{n+1} 2(q_j - q_{j-1}) [ \delta_{j,k} - \delta_{j-1,k} ]$$
> (This yields the force equation above).
> 
> Kinetic Energy:
> $$T = \frac{1}{2} m \sum_{j=1}^n \dot{q}_j^2$$

> **Elaboration:**
> The lecture moves to a system with an arbitrary number of degrees of freedom ($N$ masses): a massless string under tension $\tau$ loaded with $n$ point masses. This is a crucial step towards continuum mechanics and wave equations.
> 
> By analyzing the forces on a single mass $j$, we see it's pulled by the tension from the string segments connecting it to $j-1$ and $j+1$. For small transverse displacements, the horizontal forces cancel, and the net vertical force is proportional to the difference in displacements (a discrete version of a second spatial derivative). We then construct the global Potential ($U$) and Kinetic ($T$) energy functions that describe the entire N-body system.

---

## 4. Solving the Coupled Equations for the Loaded String (حل این معادلات جفت شده)

**Original Notes Transcription:**
> ■ در نتیجه لاگرانژی سیستم به شکل زیر بدست می آید :
> (As a result, the Lagrangian of the system is obtained as follows:)
> $$L = \frac{1}{2} \sum_{j=1}^n m \dot{q}_j^2 - \frac{\tau}{2d} \sum (q_j - q_{j-1})^2$$
> 
> بدست آمده از این لاگرانژی منجر به معادله حرکت بالا می شود . 
> (The Euler-Lagrange equation from this Lagrangian leads to the above equation of motion:)
> $$m \ddot{q}_j - \frac{\tau}{d} (q_{j-1} - 2q_j + q_{j+1}) = 0$$
> 
> ■ **حل این معادلات جفت شده :** (Solving these coupled equations:)
> 
> ■ **قدم اول :** (Step one:)
> Guess a harmonic time dependence:
> $$q_j(t) = a_j e^{+i\omega t}$$
> (Where $a_j$ is the amplitude of particle $j$).
> 
> Substituting this into the equation of motion:
> $$- \frac{\tau}{d} a_{j-1} + \underbrace{\left(\frac{2\tau}{d} - m\omega^2\right)}_{\equiv \lambda} a_j - \frac{\tau}{d} a_{j+1} = 0 \quad (*)$$
> 
> که به شکل ماتریس زیر قابل بازنویسی است : (Which can be rewritten in the following matrix form:)
> $$\begin{pmatrix} \lambda & -\frac{\tau}{d} & 0 & \dots \\ -\frac{\tau}{d} & \lambda & -\frac{\tau}{d} & \dots \\ 0 & -\frac{\tau}{d} & \lambda & \dots \\ \vdots & \vdots & \vdots & \ddots \end{pmatrix} \begin{pmatrix} a_1 \\ a_2 \\ \vdots \end{pmatrix} = 0$$
> 
> این معادله را برای $n=1, n=2$ قبلاً حل کرده ایم : 
> (We have already solved this equation for n=1, n=2:)
> - $n=1 \rightarrow \omega = \sqrt{\frac{2\tau}{md}}$ (Equivalent to $\omega = \sqrt{\frac{2K}{m}}$ for a 1-mass spring system).
> - $n=2 \rightarrow \omega = \sqrt{\frac{2K \pm K}{m}}$ (Equivalent to a 2-mass spring system where $K \equiv \tau/d$).
> 
> ■ **سؤال : برای n های کلی چه کنیم ؟** (Question: What do we do for general n's?)
> با الهام از جواب های قبلی چنین جوابی پیشنهاد می کنیم : 
> (Inspired by previous answers, we suggest such an answer:)
> $$a_j = a e^{i(j\gamma - \delta)}$$
> - $a$: ضریب دلخواه مستقل از j (Arbitrary coefficient independent of $j$)
> - $j$: شماره ذره (Particle number)
> - $\gamma$: A wave number parameter.
> So the full complex answer is $q_j(t) = a_j e^{i\omega t}$.
> 
> معادله (*) با حدس بالا به شکل زیر ساده می شود : 
> (Equation (*) with the above guess simplifies as follows:)
> $$-\frac{\tau}{d} e^{-i\gamma} + \left(\frac{2\tau}{d} - m\omega^2\right) - \frac{\tau}{d} e^{+i\gamma} = 0$$
> $$\rightarrow \omega^2 = \frac{2\tau}{md} - \frac{\tau}{md}(e^{+i\gamma} + e^{-i\gamma}) = \frac{2\tau}{md} (1 - \cos\gamma)$$
> 
> Using the half-angle identity $1 - \cos\gamma = 2\sin^2(\gamma/2)$:
> $$\omega_r^2 = \frac{4\tau}{md} \sin^2 \left(\frac{\gamma_r}{2}\right) \quad \checkmark$$
> *(Note: The professor jokes here: "از آنجایی که $\gamma$ دلخواه است به نظر می رسد ، استاد دچار آسیب روانی شود ، زیرا بی نهایت $\omega^2$ یافته است ." - Since $\gamma$ is arbitrary, it seems the professor will suffer psychological damage because he has found an infinite number of $\omega^2$!)*

> **Elaboration:**
> Finding the determinant of an $N \times N$ matrix is impossible algebraically for general $N$. Instead, we use a brilliant guess inspired by translational symmetry. Since the masses are identical and equally spaced, we guess that the amplitude varies harmonically from mass to mass: $a_j \propto e^{ij\gamma}$. 
> 
> This spatial guess turns a system of $N$ coupled differential equations into a simple algebraic equation! It immediately reveals the "dispersion relation" linking the oscillation frequency $\omega$ to the spatial wave parameter $\gamma$. However, since $\gamma$ can be any number, we seemingly have infinite frequencies. Boundary conditions will fix this.

---

## 5. Applying Boundary Conditions to the General Solution (اعمال شرایط مرزی)

**Original Notes Transcription:**
> با توجه به حدس (قسمت مکانی / قسمت زمانی) داریم : 
> (According to the spatial/temporal guess we have:)
> $$a_{jr} = a_r e^{i(j\gamma_r - \delta_r)}$$
> 
> اما می دانیم (همچون قبل) قسمت حقیقی جواب بار فیزیکی است ، لذا داریم : 
> (But we know, as before, the real part of the answer carries the physical meaning, so we have:)
> $$a_{jr} = \underbrace{a_r}_{\text{حقیقی (Real)}} \cos(j\gamma_r - \delta_r)$$
> 
> ■ **حال شرایط مرزی را اعمال می کنیم :** (Now we apply the boundary conditions:)
> The string is tied down at the ends: $a_{0} = a_{n+1} = 0$.
> 
> 1. At $j=0$:
> $$a_{0r} = 0 \rightarrow a_r \cos(0 - \delta_r) = 0 \rightarrow \delta_r = \frac{\pi}{2}$$
> 
> 2. At $j=n+1$:
> $$a_{(n+1)r} = 0 \rightarrow a_r \cos((n+1)\gamma_r - \frac{\pi}{2}) = 0 \rightarrow a_r \sin((n+1)\gamma_r) = 0$$
> 
> This sine function is zero when the argument is an integer multiple of $\pi$:
> $$(n+1)\gamma_r = r\pi \rightarrow \gamma_r = \frac{r\pi}{n+1} \quad r = 1, 2, \dots, \infty \text{ (اعداد صحیح - integers)}$$
> 
> However, because of the discrete nature of the masses, values of $r > n$ just repeat the same physical shapes (aliasing). Therefore, there are exactly $n$ unique normal modes:
> $$\gamma_r = \frac{r\pi}{n+1} \quad \text{for } r = 1, \dots, n$$
> 
> ■ **جواب کلی :** (General answer:)
> $$a_{jr} = a_r \sin\left(j \frac{r\pi}{n+1}\right)$$
> 
> The full solution is a superposition of all normal modes:
> $$q_j(t) = \sum_{r=1}^n \underbrace{\beta_r' \overbrace{a_{jr}}^{\text{ضریب مقیاس (Scale factor)}}}_{\equiv \beta_r} e^{i\omega_r t}$$
> $$q_j(t) = \sum_{r=1}^n \beta_r \sin\left(j \frac{r\pi}{n+1}\right) e^{i\omega_r t}$$
> Where the frequencies are:
> $$\omega_r = 2 \sqrt{\frac{\tau}{md}} \sin\left(\frac{r\pi}{2(n+1)}\right)$$
> 
> The complex coefficient $\beta_r = \mu_r + i\nu_r$ is determined from the initial conditions ($q_j(0)$ and $\dot{q}_j(0)$) using Fourier-like sums:
> $$\mu_s = \frac{2}{n+1} \sum_{j=1}^n q_j(0) \sin\left(j \frac{s\pi}{n+1}\right)$$
> $$\nu_s = \frac{-2}{\omega_s(n+1)} \sum_{j=1}^n \dot{q}_j(0) \sin\left(j \frac{s\pi}{n+1}\right)$$

> **Elaboration:**
> The boundary conditions save us from the "infinite frequencies" problem. Tying the ends of the string down ($j=0$ and $j=n+1$) forces $\delta = \pi/2$ and quantizes the allowed values of $\gamma$. 
> 
> We find that $\gamma$ can only take specific values related to $r\pi/(n+1)$. Due to the discrete masses (aliasing), only $n$ unique modes exist, perfectly matching our $n$ degrees of freedom!
> 
> The final general solution is a sum of these $n$ normal modes. To find the exact motion of the string for a specific problem, we look at how the string was initially plucked or struck, and use the discrete orthogonality of sine waves to compute the specific coefficients $\beta_r$ (which encode both amplitude and phase). This is the discrete analog to a Fourier Series!
