# Advanced Dynamics: The Normal Coordinate "Mission Unlocked" & Exam Algorithm

> [!abstract] Navigation
> **Chapter:** [[Chapter 12 - Coupled Oscillations and Normal Modes]] | **Prev:** [[Note Jun 13, 2026]] | **Next:** [[Note Jun 27, 2026]] | [[Lecture Index|📚 All Lectures]]
>
> ⭐ **Canonical reference for the [[Eigenvalue Problem for Normal Modes|Normal Mode Algorithm]]** -- use this as your exam checklist!

> **Context:** We have reached the "Mission Unlocked" ✅ stage (as doodled by your professor in Image 1). After proving mode orthogonality, we will now perform the ultimate decoupling trick. We will prove that **Kinetic Energy (\(T\))** and **Potential Energy (\(U\))** become simple sums of squares when written in Normal Coordinates. This makes Euler-Lagrange equations completely independent!

---

## 1. The Decoupling Magic: \(T\) and \(U\) in Normal Coordinates
We define the Normal Coordinates \(\eta_r(t)\) such that:
\[
q_j(t) = \sum_{r=1}^{n} a_{jr} \eta_r(t)
\]
Where \(a_{jr}\) are the mass-normalized eigenvectors (amplitude of coordinate \(j\) in mode \(r\)).

### 1.1 Kinetic Energy Decoupled
Starting with the general kinetic energy \(T = \frac{1}{2} \sum_{j,k} m_{jk} \dot{q}_j \dot{q}_k\):

\[
T = \frac{1}{2} \sum_{j,k} m_{jk} \left( \sum_r a_{jr} \dot{\eta}_r \right) \left( \sum_s a_{ks} \dot{\eta}_s \right)
\]
Rearranging the sums:
\[
T = \frac{1}{2} \sum_{r,s} \dot{\eta}_r \dot{\eta}_s \left( \sum_{j,k} m_{jk} a_{jr} a_{ks} \right)
\]
**The Magic Step:** Using the orthogonality and normalization condition we proved last time (\(\sum_{j,k} m_{jk} a_{jr} a_{ks} = \delta_{rs}\)), the cross-terms collapse:
\[
T = \frac{1}{2} \sum_{r,s} \dot{\eta}_r \dot{\eta}_s \delta_{rs} = \mathbf{\frac{1}{2} \sum_r (\dot{\eta}_r)^2}
\]

### 1.2 Potential Energy Decoupled
Now, substituting the same \(q_j\) into \(U = \frac{1}{2} \sum_{j,k} A_{jk} q_j q_k\):

\[
U = \frac{1}{2} \sum_{r,s} \eta_r \eta_s \left( \sum_{j,k} A_{jk} a_{jr} a_{ks} \right)
\]
Using the eigenvalue equation \(\sum_j A_{jk} a_{jr} = \omega_r^2 \sum_j m_{jk} a_{jr}\), we can simplify the inner term to \(\omega_r^2 \delta_{rs}\).
\[
\mathbf{U = \frac{1}{2} \sum_r \omega_r^2 (\eta_r)^2}
\]

### 1.3 The Independent Lagrangian
With these simplifications, the Lagrangian \(L = T - U\) becomes:
\[
L = \frac{1}{2} \sum_{r=1}^n \left( \dot{\eta}_r^2 - \omega_r^2 \eta_r^2 \right)
\]
> **Professor's Oral Note:** This is the ultimate mathematical victory! Instead of a complicated system of \(n\) *coupled* equations, the Lagrangian is now a sum of *independent* simple harmonic oscillators. 

Applying Euler-Lagrange equation for each \(\eta_r\):
\[
\frac{d}{dt}\left(\frac{\partial L}{\partial \dot{\eta}_r}\right) - \frac{\partial L}{\partial \eta_r} = 0 \implies \mathbf{\ddot{\eta}_r + \omega_r^2 \eta_r = 0}
\]

---

## 2. The 7-Step Recipe for Final Exam Problems
Your professor explicitly wrote out the algorithm for solving any multi-degree-of-freedom small oscillation problem. **Memorize this exact sequence:**

1.  **Find Equilibrium:** Set the first derivative of potential energy to zero to find equilibrium positions (\(q_{j0}\)).
2.  **Construct Matrices:** Compute the **Mass Matrix** (\(m_{jk}\)) and **Stiffness Matrix** (\(A_{jk}\)) evaluated at equilibrium.
3.  **Find Eigenvalues (Frequencies):** Solve the characteristic equation \(\det|A_{jk} - \omega^2 m_{jk}| = 0\) to find all \(\omega_r^2\).
4.  **Find Eigenvectors (Amplitudes):** Plug each \(\omega_r^2\) back into the matrix equation to find the amplitude ratios (\(a_{jr}\)).
5.  **Normalize Eigenvectors:** Scale the amplitudes so that \(\sum_{j,k} m_{jk} a_{jr} a_{kr} = 1\).
6.  **Solve Normal Coordinates:** Solve the independent oscillator equations \(\ddot{\eta}_r + \omega_r^2 \eta_r = 0\) to find \(\eta_r(t)\) with constants \(\beta_r\). (Using given Initial Conditions).
7.  **Transform Back:** Construct the final physical motion by summing the modes: \(q_j(t) = \sum_r a_{jr} \eta_r(t)\).

---

## 3. Complete Worked Example: 3 Identical Springs (\(k_{12} = k\))
Let's apply the recipe to the classic 2-mass setup, but with all three springs having identical stiffness \(k\).

### 3.1 Setup and Matrices (Steps 1 & 2)
Physical setup: Masses \(M\), Outer springs \(k\), Middle spring \(k\).
\[
A = \begin{pmatrix} k+k & -k \\ -k & k+k \end{pmatrix} = \begin{pmatrix} 2k & -k \\ -k & 2k \end{pmatrix}, \quad M = \begin{pmatrix} M & 0 \\ 0 & M \end{pmatrix}
\]

### 3.2 The Eigenvalue Problem (Steps 3 & 4)
Characteristic determinant:
\[
 \det \begin{pmatrix} 2k - M\omega^2 & -k \\ -k & 2k - M\omega^2 \end{pmatrix} = 0 
\]
\[
(2k - M\omega^2)^2 - k^2 = 0 \implies 2k - M\omega^2 = \pm k
\]

*   **Solution 1:** \(2k - M\omega^2 = -k \implies \mathbf{\omega_1^2 = \frac{3k}{M}}\) (Anti-symmetric mode).
*   **Solution 2:** \(2k - M\omega^2 = +k \implies \mathbf{\omega_2^2 = \frac{k}{M}}\) (Symmetric mode).

**Finding the Eigenvectors:**
*   For \(r=1\) (\(\omega_1^2 = 3k/M\)): Plugging back into the equation yields \(a_{11} = -a_{21}\). (They move in opposite directions).
*   For \(r=2\) (\(\omega_2^2 = k/M\)): Yields \(a_{12} = +a_{22}\). (They move together).

> **⚠️ Exam Trap / Professor's Oral Note:** In the original handwritten note (Image 4), the professor mistakenly wrote \(\omega_1^2 = \frac{8k}{M}\) as a quick slip, while the correct algebra yields \(\frac{3k}{M}\). **Do not panic if you see this on the exam solution!** If the middle spring is \(k\), the effective spring constant for the out-of-phase mode is \(k + 2k = 3k\). The effective spring constant for the in-phase mode is \(k\).

### 3.3 Normalizing the Amplitudes (Step 5)
We use the normalization rule: \(\sum_{jk} m_{jk} a_{jr} a_{kr} = 1\).
Let's find the unknown amplitude \(a_{11}\) for Mode 1 (\(a_{21} = -a_{11}\)):
\[
m_{11}a_{11}a_{11} + m_{22}a_{21}a_{21} + \text{cross terms}= 0 \text{ (since off-diagonals of M are 0)}
\]
\[
M(a_{11})^2 + M(-a_{11})^2 = 1 \implies 2M (a_{11})^2 = 1 \implies \mathbf{a_{11} = \frac{1}{\sqrt{2M}}}
\]
*(Note: by symmetry, \(a_{22} = \frac{1}{\sqrt{2M}}\) for Mode 2 as well).*

### 3.4 Transformation to Normal Coordinates (Step 7)
Our physical coordinates \(x_1\) and \(x_2\) are:
\[
x_1 = a_{11} \eta_1 + a_{12} \eta_2 = \frac{1}{\sqrt{2M}} (\eta_1 + \eta_2)
\]
\[
x_2 = a_{21} \eta_1 + a_{22} \eta_2 = \frac{1}{\sqrt{2M}} (-\eta_1 + \eta_2)
\]
We can solve for the Normal Coordinates inversely:
\[
\mathbf{\eta_1 = \sqrt{\frac{M}{2}} (x_1 - x_2)}
\]
\[
\mathbf{\eta_2 = \sqrt{\frac{M}{2}} (x_1 + x_2)}
\]
> **Professor's Oral Note:** You can see why \(\eta_1\) is the "Anti-symmetric" mode and \(\eta_2\) is the "Symmetric" mode. If you take \(x_1 - x_2\), you capture how far apart they are (acting against the middle spring). If you take \(x_1 + x_2\), you capture their center of mass motion (where the middle spring is useless). 

---

## 4. The "ON/OFF" Mode Switching (Physical Intuition)
In Image 6, your professor drew the system with the modes labeled as "ON" or "OFF". This is a perfect way to visualize normal coordinates in an exam setup.

*   **\(\eta_1\) ON, \(\eta_2\) OFF:** Only the anti-symmetric mode is active. The masses move perfectly opposite each other. The middle spring stretches the most. 
*   **\(\eta_2\) ON, \(\eta_1\) OFF:** Only the symmetric mode is active. The masses move exactly in unison. The middle spring length never changes. 

**The Double Pendulum Note:**
On the bottom of Image 6, the professor drew two identical simple pendulums connected by a spring. The green diagrams show:
1.  **Symmetric Mode:** Both pendulums swing outwards/inwards together. The connecting spring does not stretch. Frequency depends on gravity \(g/l\).
2.  **Anti-Symmetric Mode:** Pendulums swing in opposite directions. The connecting spring stretches, adding a restoring force. Frequency is higher. 

> **Final Exam Tip:** For any 2-DOF system (double pendulums, masses on a rigid rod, or springs), drawing the **Symmetric** and **Anti-symmetric** visual diagrams is the fastest way to guess the correct frequencies and eigenvectors before doing the complex matrix math. It allows you to cross-check your determinant result!