# Advanced Dynamics: Mode Orthogonality & Normal Coordinates

> [!abstract] Navigation
> **Chapter:** [[Chapter 12 - Coupled Oscillations and Normal Modes]] | **Prev:** [[Note Jun 8, 2026]] | **Next:** [[Note Jun 20, 2026]] | [[Lecture Index|📚 All Lectures]]

> **Context:** In this final lecture on small oscillations, we move beyond simply calculating frequencies. We formalize the rigorous mathematical properties of the normal modes. Specifically, we prove that the **Normal Modes are Orthogonal**, and we use this property to define **Normal Coordinates** (\(\eta_r\)). Once you shift to these normal coordinates, the original system of \(n\) coupled differential equations completely decouples into \(n\) independent simple harmonic oscillators. This is the ultimate goal of this chapter.

---

## 1. Recap: The General Matrix Framework
From our previous notes, we established the Lagrangian for a system with \(n\) generalized coordinates \(q_j\) in equilibrium:

1.  **Kinetic Energy:** \(T = \frac{1}{2} \sum_{j,k} m_{jk} \dot{q}_j \dot{q}_k\)
2.  **Potential Energy:** \(U = \frac{1}{2} \sum_{j,k} A_{jk} q_j q_k\)
    *(Where \(A_{jk}\) is the stiffness/Hessian matrix).*

By applying Euler-Lagrange, we arrived at the equations of motion:
\[
 \sum_{j} \left( A_{jk} q_j + m_{jk} \ddot{q}_j \right) = 0 
\]

Assuming a harmonic trial solution \(q_j(t) = a_j e^{i(\omega t - \delta)}\), we reduce the problem to the **Generalized Eigenvalue Problem**:
\[
 \sum_{j} \left( A_{jk} - \omega^2 m_{jk} \right) a_j = 0 
\]
To find the allowed frequencies \(\omega\), we solve the **Characteristic Equation**:
\[
 \det|A_{jk} - \omega^2 m_{jk}| = 0 
\]

---

## 2. The Physics of Orthogonality (The Formal Proof)
Because the eigenvalue problem is fundamentally linear, the general physical solution \(q_j(t)\) is a **linear superposition** of all \(n\) normal modes:
\[
 q_j(t) = \sum_{r=1}^n a_{jr} \cos(\omega_r t - \delta_r) 
\]
*(Where \(r\) is an index for a specific mode, and \(a_{jr}\) is the amplitude of coordinate \(j\) in mode \(r\)).*

### 2.1 Proving Modes Are Orthogonal (Key Exam Derivation)
The professor provides a step-by-step derivation proving that two different normal modes, \(r\) and \(s\), cannot "overlap" in kinetic energy space. This results in a **Mass-Weighted Orthogonality Condition**.

**Step 1:** Write the eigenvalue equation for two distinct modes, \(r\) and \(s\):
*   (Eq I) For mode \(s\): \( \omega_s^2 \sum_{k} m_{jk} a_{ks} = \sum_{k} A_{jk} a_{ks} \)
*   (Eq II) For mode \(r\): \( \omega_r^2 \sum_{k} m_{jk} a_{kr} = \sum_{k} A_{jk} a_{kr} \)

**Step 2:** Multiply Eq I by \(a_{jr}\) and sum over all \(j\). Multiply Eq II by \(a_{js}\) and sum over all \(j\):
*   \( \omega_s^2 \sum_{j,k} m_{jk} a_{jr} a_{ks} = \sum_{j,k} A_{jk} a_{jr} a_{ks} \)
*   \( \omega_r^2 \sum_{j,k} m_{jk} a_{js} a_{kr} = \sum_{j,k} A_{jk} a_{js} a_{kr} \)

**Step 3:** Subtract the two equations. Because **the Mass Matrix \(m_{jk}\) and the Stiffness Matrix \(A_{jk}\) are symmetric** (meaning \(m_{jk} = m_{kj}\) and \(A_{jk} = A_{kj}\)), the double sums on the right-hand side (potential energy terms) are mathematically identical and cancel out!

\[
 (\omega_r^2 - \omega_s^2) \sum_{j,k} m_{jk} a_{jr} a_{ks} = 0 
\]

**Step 4:** Since we are looking at two *different* modes, their frequencies are distinct (\(\omega_r \neq \omega_s\)). Therefore, the sum must equal zero:
\[
 \mathbf{\sum_{j,k} m_{jk} a_{jr} a_{ks} = 0} \quad \text{for } r \neq s 
\]
This is the formal definition of **Orthogonality of Normal Modes**.

---

## 3. Normalization & The Identity Matrix Trick
### 3.1 Defining the Kronecker Delta
To solve for unknown coefficients later, we need our amplitude vectors (\(a_{jr}\)) to be normalized. The professor introduces the **Kronecker Delta (\(\delta_{rs}\))** normalization:
\[
 \mathbf{\sum_{j,k} m_{jk} a_{jr} a_{ks} = \delta_{rs}} 
\]
*(Where \(\delta_{rs} = 1\) if \(r=s\), and \(0\) if \(r \neq s\).)*
> **Professor's Oral Tip:** In terms of vector/matrix multiplication, if we treat \(a_r\) as a column vector and \(a_s\) as a column vector, this equation is simply: \(\mathbf{a_r^T M a_s = \delta_{rs}}\). (You don't need matrix math notation, but it helps to visualize the orthogonality in 3D space).

### 3.2 Scaling to the "Identity Matrix" (Simplification Trick)
The professor highlights a very useful trick for simplifying the math: **Coordinate Scaling**.
Define a new set of coordinates \(\bar{q}_i = \sqrt{m_i} q_i\). 
*   In this scaled space, the kinetic energy becomes \(T = \frac{1}{2} \sum_i \dot{\bar{q}}_i^2\).
*   **Result:** This makes the Mass Matrix become the **Identity Matrix (\(M = I\))**.
*   **Simplified Orthogonality:** Now, the mass matrix vanishes from the sum, leaving us with the standard vector dot product:
\[
 \mathbf{\sum_k a_{ks} a_{kr} = \delta_{rs}} 
\]
*(This is much easier to compute and identify on exams).*

---

## 4. Kinetic Energy Decoupling (The Physical Result)
We now take the general solution and prove why it is so mathematically powerful. Let's plug our general solution into the Kinetic Energy \(T\).

*   \(\dot{q}_j(t) = \sum_r -a_{jr} \omega_r \sin(\omega_r t - \delta_r)\).
*   Substituting this into \(T = \frac{1}{2} \sum_{j,k} m_{jk} \dot{q}_j \dot{q}_k\):
\[
 T = \frac{1}{2} \sum_{r,s} \omega_r \omega_s \sin(\omega_r t - \delta_r) \sin(\omega_s t - \delta_s) \left( \sum_{j,k} m_{jk} a_{jr} a_{ks} \right) 
\]

**Here is the magic:**
Because of the orthogonality condition \(\sum_{j,k} m_{jk} a_{jr} a_{ks} = \delta_{rs}\), the cross-terms (where \(r \neq s\)) completely vanish!
The sum collapses into only terms where \(r = s\):
\[
 T = \frac{1}{2} \sum_r \omega_r^2 \sin^2(\omega_r t - \delta_r) \left( \sum_{j,k} m_{jk} a_{jr} a_{kr} \right) 
\]

> **Professor's Oral Note:** Since Kinetic Energy is always positive (\(T>0\)), and \(\omega_r^2 \sin^2(...)\) is positive, it proves that \(\sum_{j,k} m_{jk} a_{jr} a_{kr}\) must be a positive number. By setting it equal to 1 (using mass-normalized eigenvectors), we arrive at our final simplified Kinetic Energy:
\[
 T = \frac{1}{2} \sum_r \omega_r^2 \sin^2(\omega_r t - \delta_r) \quad \text{(for mass-normalized modes)} 
\]

---

## 5. Normal Coordinates (\(\eta_r\)) - The Ultimate Decoupling Trick
The final definition provided in the notes is the concept of **Normal Coordinates**.

Let \(\eta_r(t)\) be a time-dependent function representing the state of the \(r\)-th mode. The physical motion of the mass in coordinate \(q_j\) is just the sum of these modes, weighted by the amplitudes \(a_{jr}\):

\[
 \mathbf{q_j(t) = \sum_{r=1}^{n} a_{jr} \eta_r(t)} 
\]

Where:
\[
 \eta_r(t) = \cos(\omega_r t - \delta_r) 
\]
*(Or equivalently, in complex exponential form: \(\eta_r(t) = B_r e^{i \omega_r t}\))*

### Why is this the "End Goal"?
If you plug \(q_j(t) = \sum_r a_{jr} \eta_r(t)\) into your original **coupled** differential equations, the orthogonality property simplifies them into **\(n\) completely independent differential equations** of the form:
\[
 \ddot{\eta}_r + \omega_r^2 \eta_r = 0 
\]
This means instead of solving a messy \(n \times n\) matrix system to find the motion, you just solve **\(n\) simple harmonic oscillators individually**. The physics of the system becomes perfectly clear: the whole complex mechanism moves as a linear combination of \(n\) independent, non-interacting "pure tones"!

---

## 6. Final Summary & Professor's Exam Pitfalls

| Concept | Critical Formula / Definition | Exam Tip |
| :--- | :--- | :--- |
| **Mode Orthogonality** | \(\sum_{j,k} m_{jk} a_{jr} a_{ks} = 0\) (for \(r \neq s\)) | **Memorize this proof!** An exam will often ask, "Prove that the normal modes of an n-degree-of-freedom system are orthogonal." Write the two eigenvalue equations, multiply, subtract, and use matrix symmetry. |
| **Mass Normalization** | \(\sum_{j,k} m_{jk} a_{jr} a_{kr} = 1\) (for \(r=s\)) | Sets the arbitrary amplitude scaling. This makes the math simpler (\(T = \frac{1}{2}\sum \omega_r^2 \sin^2(...)\)). If you don't normalize, your final answer will be missing a constant multiplier. |
| **Change of Basis** | \(q_j(t) = \sum_r a_{jr} \eta_r(t)\) | The **Normal Coordinates transformation**. |
| **Physical Meaning** | \(\eta_r\) undergoes simple harmonic motion (\(\ddot{\eta}_r + \omega_r^2 \eta_r = 0\)). | **Crucial:** The physical coordinates \(q_j\) are *coupled*. The normal coordinates \(\eta_r\) are *perfectly decoupled*. Always solve for \(\eta_r\) first, then transform back to \(q_j\). |