# Coupled Harmonic Oscillators: A Comprehensive Study Guide

> [!abstract] Navigation
> **Chapter:** [[Chapter 12 - Coupled Oscillations and Normal Modes]] | **Prev:** [[Note May 30, 2026]] | **Next:** [[Note Jun 6, 2026]] | [[Lecture Index|📚 All Lectures]]
>
> **Key concepts:** [[Eigenvalue Problem for Normal Modes|Eigenvalue Problem]], [[Lagrangian Mechanics|Lagrangian]] $T$ and $U$ matrices
**Topic:** Two identical masses \(M\) connected by three springs (two outer springs with stiffness \(k\), one middle spring with stiffness \(k_{12}\)). Frictionless horizontal surface.

## 1. The Physics Setup & Equations of Motion
We examine a system where two identical masses \(M\) are constrained to move on a frictionless line. They are attached to fixed walls by springs of stiffness \(k\), and to each other by a spring of stiffness \(k_{12}\).

Let \(x_1(t)\) and \(x_2(t)\) be the displacements of the left and right masses from their equilibrium positions.

### Deriving Newton's Second Law
*   **For Mass 1 (Left):**
    *   Left wall pulls: \(-k x_1\)
    *   Middle spring pulls if stretched: \(+k_{12}(x_2 - x_1)\)
    *   Equation: \(M\ddot{x}_1 = -k x_1 + k_{12}(x_2 - x_1)\)
    *   Rearranged: \(\mathbf{M\ddot{x}_1 + (k + k_{12})x_1 - k_{12}x_2 = 0}\)
*   **For Mass 2 (Right):**
    *   Right wall pulls: \(-k x_2\)
    *   Middle spring pulls: \(-k_{12}(x_2 - x_1)\)
    *   Equation: \(M\ddot{x}_2 = -k x_2 - k_{12}(x_2 - x_1)\)
    *   Rearranged: \(\mathbf{M\ddot{x}_2 + (k + k_{12})x_2 - k_{12}x_1 = 0}\)

> **Professor's Oral Note:** Notice how the equations are *coupled*. The equation for \(x_1\) depends on \(x_2\) and vice versa. You cannot solve one without the other directly.

---

## 2. Solving for the Normal Modes (Eigenfrequencies)
We use the standard complex exponential trial solution for oscillatory systems:
\[
x_1(t) = B_1 e^{i\omega t}, \quad x_2(t) = B_2 e^{i\omega t}
\]
*(Where \(B_1\) and \(B_2\) are complex amplitudes that also encode phase information).*

Substituting these into our two coupled differential equations:
1.  \(\left(-M\omega^2 + k + k_{12}\right)B_1 - k_{12}B_2 = 0\)
2.  \(-k_{12}B_1 + \left(-M\omega^2 + k + k_{12}\right)B_2 = 0\)

### Matrix Formulation
We can write this as an eigenvalue problem:
\[
\begin{pmatrix} -M\omega^2 + k + k_{12} & -k_{12} \\ -k_{12} & -M\omega^2 + k + k_{12} \end{pmatrix} \begin{pmatrix} B_1 \\ B_2 \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix}
\]

> **Professor's Oral Note:** For a nontrivial solution (meaning the masses are actually moving, \(B_1 \neq 0\) and \(B_2 \neq 0\)), the determinant of this matrix must be **zero**.
>
> **Exam Pitfall:** Always remember the "determinant equals zero" step. If you skip it, you can't find the characteristic equation.

### Finding the Frequencies
Taking the determinant:
\[
(k + k_{12} - M\omega^2)^2 - (-k_{12})^2 = 0
\]
\[
(k + k_{12} - M\omega^2)^2 = k_{12}^2
\]
Taking the square root:
\[
k + k_{12} - M\omega^2 = \pm k_{12}
\]

We arrive at our two characteristic frequencies:
1.  **Case 1 (\(+k_{12}\)):** \(k + k_{12} - M\omega^2 = k_{12} \implies M\omega^2 = k \implies \mathbf{\omega_2 = \sqrt{\frac{k}{M}}}\)
2.  **Case 2 (\(-k_{12}\)):** \(k + k_{12} - M\omega^2 = -k_{12} \implies M\omega^2 = k + 2k_{12} \implies \mathbf{\omega_1 = \sqrt{\frac{k + 2k_{12}}{M}}}\)

> **Professor's Oral Note:** Notice that \(\omega_1\) (the out-of-phase frequency) is always larger than \(\omega_2\) (the in-phase frequency) because \(k+2k_{12} > k\).

---

## 3. Physical Interpretation (Amplitude Ratios)
Let's plug our frequencies back into the matrix to find the relationship between \(B_1\) and \(B_2\).

### Mode 1: The Out-of-Phase Mode (\(\omega = \omega_1\))
Plugging \(\omega_1^2 = (k+2k_{12})/M\) into the first equation:
\[
(k+k_{12} - (k+2k_{12}))B_1 - k_{12}B_2 = 0 \implies (-k_{12})B_1 - k_{12}B_2 = 0
\]
\[
\mathbf{B_1 = -B_2}
\]
*   **Visual:** The masses move in opposite directions with equal magnitude.
*   **Physical Intuition:** When they move towards each other or away from each other, the middle spring \(k_{12}\) stretches or compresses by **2 times** the displacement of a single mass. The force exerted by the middle spring is \(k_{12}(2x_1)\). This acts in addition to the outer springs.
*   **Equivalent System:** This mode acts exactly like a **single mass \(M\) attached to a spring with stiffness \(k_{\text{eff}} = k + 2k_{12}\)**. Thus, \(\omega_1 = \sqrt{\frac{k+2k_{12}}{M}}\).

### Mode 2: The In-Phase Mode (\(\omega = \omega_2\))
Plugging \(\omega_2^2 = k/M\) into the first equation:
\[
(k+k_{12} - k)B_1 - k_{12}B_2 = 0 \implies (k_{12})B_1 - k_{12}B_2 = 0
\]
\[
\mathbf{B_1 = B_2}
\]
*   **Visual:** The masses move in the exact same direction with equal magnitude.
*   **Physical Intuition:** The distance between the two masses never changes. Therefore, the middle spring \(k_{12}\) is **never stretched or compressed**. It is effectively invisible to the motion.
*   **Equivalent System:** This mode acts exactly like a **single mass \(M\) attached to only the outer spring \(k\)** (the two masses move as one rigid body). Thus, \(\omega_2 = \sqrt{\frac{k}{M}}\).

---

## 4. Normal Coordinates (The Decoupling Trick)
Instead of dealing with \(x_1\) and \(x_2\), which are coupled, we can define new coordinates that uncouple the equations immediately.

Let's define **Normal Coordinates**:
\[
\eta_1(t) \equiv x_1(t) - x_2(t) \quad \text{(Relative motion)}
\]
\[
\eta_2(t) \equiv x_1(t) + x_2(t) \quad \text{(Center of mass/Common motion)}
\]

And their inverse relations for returning to the original positions:
\[
x_1 = \frac{1}{2}(\eta_1 + \eta_2), \quad x_2 = \frac{1}{2}(\eta_2 - \eta_1)
\]

> **Professor's Oral Note:** If this transformation works, taking the second derivative is easy: \(M\ddot{x}_1 = \frac{1}{2}M(\ddot{\eta}_1 + \ddot{\eta}_2)\) and so on.

### Deriving the Uncoupled Equations
Substitute \(x_1\) and \(x_2\) into our original equations. After adding and subtracting the two original equations correctly, you will find:

\[
\mathbf{M\ddot{\eta}_1 + (k + 2k_{12})\eta_1 = 0} \implies \omega_1^2 = \frac{k+2k_{12}}{M}
\]
\[
\mathbf{M\ddot{\eta}_2 + (k)\eta_2 = 0} \implies \omega_2^2 = \frac{k}{M}
\]

These are now **two independent simple harmonic oscillators**!

### General Solutions (The Final Answer)
The solutions to these uncoupled equations are:
\[
\eta_1(t) = C_1^+ e^{i\omega_1 t} + C_1^- e^{-i\omega_1 t}
\]
\[
\eta_2(t) = C_2^+ e^{i\omega_2 t} + C_2^- e^{-i\omega_2 t}
\]

Transforming back to \(x_1\) and \(x_2\) gives the general solution:
\[
\mathbf{x_1(t) = \frac{1}{2} \left[ \left(C_1^+ e^{i\omega_1 t} + C_1^- e^{-i\omega_1 t}\right) + \left(C_2^+ e^{i\omega_2 t} + C_2^- e^{-i\omega_2 t}\right) \right]}
\]
\[
\mathbf{x_2(t) = \frac{1}{2} \left[ \left(C_2^+ e^{i\omega_2 t} + C_2^- e^{-i\omega_2 t}\right) - \left(C_1^+ e^{i\omega_1 t} + C_1^- e^{-i\omega_1 t}\right) \right]}
\]

*(Note: The 4 constants \(C_1^+, C_1^-, C_2^+, C_2^-\) are purely determined by the initial conditions of the problem: 2 initial positions and 2 initial velocities).*

---

## 5. Testing Initial Conditions (Exam Application)
The professor highlighted two specific initial conditions that are very common in exam questions.

**Case 1: Symmetrical Initial Displacements (\(x_1(0) = x_2(0), \dot{x}_1(0) = \dot{x}_2(0)\))**
*   This implies \(\eta_1(0) = 0\) and \(\dot{\eta}_1(0) = 0\). Because the relative coordinate is zero, the out-of-phase mode does not participate.
*   **Result:** The constants \(C_1^+ = C_1^- = 0\). The system will oscillate purely with frequency \(\omega_2\).
*   *(What happens physically? Both masses move together, the middle spring is useless, they vibrate as if attached by the wall springs).*

**Case 2: Opposite Initial Displacements (\(x_1(0) = -x_2(0), \dot{x}_1(0) = -\dot{x}_2(0)\))**
*   This implies \(\eta_2(0) = 0\) and \(\dot{\eta}_2(0) = 0\). The center of mass coordinate is zero, so the in-phase mode does not participate.
*   **Result:** The constants \(C_2^+ = C_2^- = 0\). The system will oscillate purely with frequency \(\omega_1\).
*   *(What happens physically? The masses get squeezed and stretched towards each other, fully engaging the middle spring).*

---

## 6. Final Summary for Quick Exam Review

| Mode | Frequency (\(\omega\)) | Mass Behavior | Effective Stiffness | Note |
| :--- | :--- | :--- | :--- | :--- |
| **Mode 1 (Out-of-phase)** | \(\sqrt{\frac{k+2k_{12}}{M}}\) | \(x_1 = -x_2\) (\(B_1 = -B_2\)) | \(k_{\text{eff}} = k+2k_{12}\) | Middle spring stretches the most. |
| **Mode 2 (In-phase)** | \(\sqrt{\frac{k}{M}}\) | \(x_1 = x_2\) (\(B_1 = B_2\)) | \(k_{\text{eff}} = k\) | Middle spring doesn't move. |

**Quick Derivation Cheat Sheet for Exams:**
1.  Write EOMs: \(M\ddot{x}_1 + (k+k_{12})x_1 - k_{12}x_2 = 0\).
2.  Assume \(x \propto e^{i\omega t}\), substitute to get the matrix.
3.  Set Determinant = 0.
4.  Solve quadratic to find \(\omega_1, \omega_2\).
5.  Plug \(\omega\) back into matrix to find amplitude ratio (whether \(B_1=B_2\) or \(B_1=-B_2\)).