# Advanced Analytical Dynamics: Generalized Small Oscillations & Orthogonality

> [!abstract] Navigation
> **Chapter:** [[Chapter 12 - Coupled Oscillations and Normal Modes]] | **Prev:** [[Note Jun 6, 2026]] | **Next:** [[Note Jun 13, 2026]] | [[Lecture Index|📚 All Lectures]]
>
> **Key concept:** [[Eigenvalue Problem for Normal Modes|Orthogonality of normal modes]]

> **Context:** In previous lectures, we solved the two-mass, three-spring system using Newton's laws. Now, we are abstracting this into a **Generalized Lagrangian Theory** that works for *any* vibrating system (molecules, pendulums, rotating shafts, etc.) by using matrices. We will also prove the critical property of **Mode Orthogonality**.

---

## 1. The Generalized Theory of Small Oscillations
### 1.1 Generalized Coordinates & Equilibrium
Let \(q_1, q_2, ..., q_n\) be the **Generalized Coordinates** (e.g., angles, radial distances, \(x, y\) positions) describing the system.
*   **Equilibrium Position:** Let \(q_j^0\) be the coordinates at equilibrium. We will redefine our coordinates as small deviations from equilibrium: \(\eta_j = q_j - q_j^0\). (For simplicity in these notes, we will assume the equilibrium is at \(q_j = 0\)).
*   **Small Oscillations:** The system undergoes small motions where \(q_j\) and \(\dot{q}_j\) remain small.

### 1.2 Kinetic Energy Matrix (\(M_{jk}\))
The kinetic energy \(T\) of the system is generally quadratic in velocities:
\[
T = \frac{1}{2} \sum_{j,k} m_{jk}(q) \dot{q}_j \dot{q}_k
\]
Where \(m_{jk}(q)\) might depend on positions (e.g., a pendulum's mass matrix depends on the length).

**How to find \(M_{jk}\) (Professor's oral derivation):**
If the Cartesian coordinates of particle \(\alpha\) are \(x_{\alpha,i}\), then \(\dot{x}_{\alpha,i} = \sum_j \frac{\partial x_{\alpha,i}}{\partial q_j} \dot{q}_j\).
Substituting this into \(T = \frac{1}{2} \sum_\alpha m_\alpha \dot{x}_{\alpha,i}^2\), we get:
\[
M_{jk} = \sum_\alpha m_\alpha \sum_i \frac{\partial x_{\alpha,i}}{\partial q_j} \frac{\partial x_{\alpha,i}}{\partial q_k}
\]
> **Exam Tip:** This is a crucial definition formula. If an exam asks for the Mass Matrix of a complex mechanism (like a double pendulum), use this chain rule to find the components.
> **Oral Explanation:** Because \(q_j\) is small, we evaluate this Mass Matrix at the equilibrium point \(q_j=0\). The complex terms vanish, leaving us with a **constant symmetric matrix** \(M_{jk}\).
> \[
T \approx \frac{1}{2} \sum_{j,k} M_{jk} \dot{q}_j \dot{q}_k
\]

### 1.3 Potential Energy Matrix (\(A_{jk}\) or Stiffness Matrix)
The potential energy \(U(q_1, ..., q_n)\) can be expanded in a Taylor series around equilibrium (\(q_j=0\)):
\[
U(q) \approx U_0 + \sum_j \left. \frac{\partial U}{\partial q_j} \right|_{0} q_j + \frac{1}{2} \sum_{j,k} \left. \frac{\partial^2 U}{\partial q_j \partial q_k} \right|_{0} q_j q_k
\]
*   **Why the first term vanishes:** \(U_0\) is a constant. Energy shifts don't affect motion.
*   **Why the second (linear) term vanishes:** At equilibrium, the generalized force is zero: \(Q_j = - \frac{\partial U}{\partial q_j} = 0\). 
*   **The Stiffness Matrix:** We define the constant **Stiffness Matrix** \(A_{jk} = \left. \frac{\partial^2 U}{\partial q_j \partial q_k} \right|_{0}\).
Therefore, for small oscillations:
\[
U \approx \frac{1}{2} \sum_{j,k} A_{jk} q_j q_k
\]

> **Professor's Oral Note (Stability):** For the equilibrium to be *stable*, the potential energy must curve upwards in all directions. Mathematically, this means the matrix \(A_{jk}\) must be **Positive Definite**. If \(A_{jk}\) has negative eigenvalues, the equilibrium is a saddle point or local maximum, and the system will fall apart, not oscillate!

### 1.4 Lagrangian and Equations of Motion
The Lagrangian is \(L = T - U\).
\[
L = \frac{1}{2} \sum_{j,k} M_{jk} \dot{q}_j \dot{q}_k - \frac{1}{2} \sum_{j,k} A_{jk} q_j q_k
\]
Applying the Euler-Lagrange equation \(\frac{d}{dt}\left(\frac{\partial L}{\partial \dot{q}_k}\right) - \frac{\partial L}{\partial q_k} = 0\), we obtain the generalized equations of motion:
\[
\mathbf{\sum_{j} \left( A_{jk} q_j + M_{jk} \ddot{q}_j \right) = 0}
\]
*(Note: This is a system of \(n\) coupled second-order differential equations).*

---

## 2. Solving for Normal Modes (The Eigenvalue Problem)
### 2.1 Trial Solution
We look for harmonic normal modes. We assume a complex exponential form:
\[
q_j(t) = a_j e^{i\omega t}
\]
*(Where \(a_j\) is the complex amplitude and \(\omega\) is the angular frequency)*.
Substituting this into our EOM:
\[
\sum_{j} A_{jk} a_j e^{i\omega t} - \omega^2 \sum_{j} M_{jk} a_j e^{i\omega t} = 0
\]
Canceling \(e^{i\omega t}\):
\[
\mathbf{\sum_{j} \left( A_{jk} - \omega^2 M_{jk} \right) a_j = 0}
\]

### 2.2 The Characteristic Equation
This is a generalized matrix eigenvalue problem. For a non-trivial solution (\(a_j \neq 0\)), the determinant of the coefficients must be zero:
\[
\mathbf{\det\left( A_{jk} - \omega^2 M_{jk} \right) = 0}
\]
Solving this \(n \times n\) determinant yields an \(n\)-th degree polynomial in \(\omega^2\). The result gives us **\(n\) natural frequencies**: \(\omega_1, \omega_2, ..., \omega_n\).

> **Exam Tip:** Do not skip the "determinant = 0" step! Setting the determinant to zero is the mathematical engine that produces the allowed frequencies of the system.

---

## 3. Specific Example: Two-Mass, Three-Spring System
Let's apply these abstract matrices to the exact physical system we studied in our very first set of notes. 

**Generalized Coordinates:** \(q_1 = x_1\) and \(q_2 = x_2\).

1.  **Kinetic Matrix (\(M_{jk}\)):**
    \[
T = \frac{1}{2}M\dot{x}_1^2 + \frac{1}{2}M\dot{x}_2^2 \implies M_{11} = M, M_{22} = M, M_{12} = M_{21} = 0
\]
    Mathematically: \(M = \begin{pmatrix} M & 0 \\ 0 & M \end{pmatrix}\).

2.  **Potential Matrix (\(A_{jk}\)):**
    *   Outer springs: \(\frac{1}{2}kx_1^2 + \frac{1}{2}kx_2^2\).
    *   Middle spring: \(\frac{1}{2}k_{12}(x_1 - x_2)^2 = \frac{1}{2}k_{12}(x_1^2 - 2x_1x_2 + x_2^2)\).
    *   Summing them: \(U = \frac{1}{2}(k+k_{12})x_1^2 + \frac{1}{2}(k+k_{12})x_2^2 - k_{12}x_1x_2\).
    *   Resulting Stiffness Matrix: \(A = \begin{pmatrix} k+k_{12} & -k_{12} \\ -k_{12} & k+k_{12} \end{pmatrix}\).

3.  **Solving the Determinant:**
    \[
 \det \left( \begin{pmatrix} k+k_{12} & -k_{12} \\ -k_{12} & k+k_{12} \end{pmatrix} - \omega^2 \begin{pmatrix} M & 0 \\ 0 & M \end{pmatrix} \right) = 0 
\]
    \[
 \det \begin{pmatrix} k+k_{12} - M\omega^2 & -k_{12} \\ -k_{12} & k+k_{12} - M\omega^2 \end{pmatrix} = 0 
\]
    This produces our exact solutions from the previous guide:
    \[
 \omega_1 = \sqrt{\frac{k+2k_{12}}{M}} \quad \text{(Mode: \(a_1 = -a_2\))} 
\]
    \[
 \omega_2 = \sqrt{\frac{k}{M}} \quad \text{(Mode: \(a_1 = a_2\))} 
\]

---

## 4. General Physical Solution & Orthogonality (CRUCIAL for Exams)
### 4.1 General Solution
Since the differential equations are linear, the general solution is the **sum over all normal modes**:
\[
q_j(t) = \sum_{r=1}^n a_{jr} \cos(\omega_r t - \delta_r) 
\]
*(Taking the real part of \(e^{i(\omega_r t - \delta_r)}\))*. 
Here, \(a_{jr}\) is the amplitude of coordinate \(j\) in the \(r\)-th normal mode, and \(\delta_r\) is the phase shift.

### 4.2 Proof of Mode Orthogonality
The professor provides a detailed derivation proving that the normal modes are **orthogonal with respect to the Mass Matrix**. This is a highly likely 10-point derivation question on the final exam.

**The derivation steps from the notes:**
Write the eigen-equation for two distinct modes, \(r\) and \(s\):
1.  \(\omega_r^2 \sum_j M_{jk} a_{jr} = \sum_j A_{jk} a_{jr}\)  *(Equation I)*
2.  \(\omega_s^2 \sum_j M_{jk} a_{js} = \sum_j A_{jk} a_{js}\)  *(Equation II)*

Now, multiply Equation I by \(a_{ks}\) and sum over \(k\), and multiply Equation II by \(a_{kr}\) and sum over \(k\):
1.  \(\omega_r^2 \sum_{j,k} M_{jk} a_{jr} a_{ks} = \sum_{j,k} A_{jk} a_{jr} a_{ks}\)
2.  \(\omega_s^2 \sum_{j,k} M_{jk} a_{js} a_{kr} = \sum_{j,k} A_{jk} a_{js} a_{kr}\)

Because \(M_{jk}\) and \(A_{jk}\) are **symmetric matrices** (\(M_{jk} = M_{kj}\)), we can swap the indices on the right-hand side of Eq II. Thus, the right sides of Eq I and Eq II are identical. If we subtract them:
\[
(\omega_r^2 - \omega_s^2) \sum_{j,k} M_{jk} a_{jr} a_{ks} = 0
\]

Since we assumed two *different* modes (so \(\omega_r \neq \omega_s\)), the sum must be zero:
\[
\mathbf{\sum_{j,k} M_{jk} a_{jr} a_{ks} = 0} \quad \text{for } r \neq s
\]

> **Professor's Oral Explanation (Why this matters):** 
> Orthogonality means the modes are mathematically independent. Just like the X-axis is perpendicular to the Y-axis in Cartesian space, Mode 1 is perpendicular to Mode 2 in "Normal Mode Space". This property is used to **find the coefficients \(a_{jr}\)** when solving for specific initial conditions. It ensures there is no energy "leakage" between different natural vibration modes.

---

## 5. Final Summary & Professor's Exam Pitfalls

| Concept | Mathematical Definition | Oral Exam Tip |
| :--- | :--- | :--- |
| **Mass Matrix (\(M_{jk}\))** | \(\sum_\alpha m_\alpha \sum_i \frac{\partial x_{\alpha,i}}{\partial q_j} \frac{\partial x_{\alpha,i}}{\partial q_k}\) | **If \(M_{jk}\) is non-diagonal**, you chose poor coordinates (e.g., using \(x,y\) for a pendulum instead of \(r,\theta\)). It makes the determinant math harder! |
| **Stiffness Matrix (\(A_{jk}\))** | \(\frac{\partial^2 U}{\partial q_j \partial q_k} \bigg|_0\) | The linear term \(\frac{\partial U}{\partial q_j}\) vanishes at equilibrium (zero force). Ensure \(A_{jk}\) is **Positive Definite** for a stable equilibrium (meaning it curves upward like a bowl). |
| **Characteristic Equation** | \(\det(A - \omega^2 M) = 0\) | The determinant yields the polynomial. The roots are the squares of the allowed frequencies \(\omega^2\). |
| **Mode Orthogonality** | \(\sum_{j,k} M_{jk} a_{jr} a_{ks} = 0\) (for \(r \neq s\)) | **This is the golden proof!** If an exam asks you to prove modes are independent, write the equations for two modes, multiply by the other's amplitude, subtract, and use symmetry to show the sum is zero. |