Scalar Product
Norm
[[Cauchy-Schwartz Inequality]]
#### Hilbert Space
- Orthonormal Basis
- Kronecker Delta Function
- Direct Sum — 5 Properties
- Tensor Product — 5 Properties
#### Operators: Linear Maps
- Maps a vector to vector: function, Matrix (complex)
- Example — Momentum Operator: maps function to function
	- Lebesgue square integral function (Momentum operator) (Property of space)
- Expectation Values: `=<Psi|A*Psi>/||Psi||²`
	- A: Bounded and Unbounded
- Variance(A) = `<A²> - <A>²`
#### Unitary Operator
- A⁺ = A⁻¹
- Reversible
- Preserve Inner Product (Same before and after applying Operator)
	- `<v,w> = <Av,Aw>`
- Quantum Theory — Symmetries, rotations
- dom(A⁺) = dom(A) = full H (Bounded)
#### Hermitian (Self-Adjoint) Operator
- A⁺ = A
- Observables, measurements
- Real eigenvalues
- dom(A⁺) = dom(A) ⊆ H (Not Necessarily)
#### Projectors
1. h ⊂ H; w ∈ h; v ∈ H
2. ||v - w|| = min
3. w = Ph(v); Ph(.) = ∑ᵢ <bᵢ, .> bᵢ = ∑ᵢ |bᵢ><bᵢ| (to pick out certain values from v)
	- e.g. v = (1,2,4); then 2D w = (1,2,0)
4. Self-adjoint (lost data)
5. P_h² = P_h, P_h⁺ = P_h
6. Hermitian Matrix = ![[Pasted image 20260312195944.png|210]]
7. Projectors: R³ → R³, Operators: R³ → R²
#### Eigenstates
1. A ∈ L(H), if ψ ∈ H and λ ∈ C
2. Aψ = λψ, where λ = eigenvalue, ψ = eigenstate
3. dim(H_λ) > 1, λ = degenerate (multiple eigenstates share one λ value)
- ==Properties
	- A⁺=A (λ=Real)
	- A⁺=A⁻¹(λ=Complex)
	- A²=I (λ=+-1)
	- A²=A (λ={0,1})
	- If $A^{-1}$ exist then $λ^{-1}$ exist
4. $A⁺=A$ and $A⁺=A^{-1}$, H = $\oplus_{\lambda \in spec_{PP}(A)}$ $H_{\lambda}$ 
5. ![[Pasted image 20260313141448.png]]
6. ![[Pasted image 20260313141524.png|286]]
7. $1 \geq P_{\Psi}(\lambda) \geq0$
8. $\sum_{\lambda} P_{\Psi}(\lambda) = 1$ 
#### Spectral Calculus:
1. What is A = f(A): YES if A=Self-Adjoint
2. $f(A) |\lambda,i_{\lambda} \rangle = f(\lambda) |\lambda,i_{\lambda} \rangle$ ; now lambda or A is a continuous spectrum inside H
==Spectral Theorem==:
3. $UAU^{-1}=\lambda$ (We diagnolize A) Q1. Why?
4. $UAU^{-1}(\oplus_{i=1}^{N} \Psi_i(\lambda)) =\oplus_{i=1}^{N}\lambda \Psi_i(\lambda)$ A1. So, $\Psi_i$ scales by eigenvalue.
5. Before A has messy basis states. i.e. so if one component in $\Psi$ changes the other component also changes.
6. We introduce $UU^{-1}$ so we rotate A into basis eigenstate. Easy Scaling.
7. No joint probability space exists for Self-Adjoint Operators/Observables even if they commute $[A,B]=0$ 
#### Principles of Quantum Theory
1. {v ∈ H, λv ∈ H for λ ∈ C\{0}} give the same physical state ([[Rays]])
2. Observables are self-adjoint
3. Spec(A) gives the probable $\lambda$ and $\langle A \rangle$ 
4. $T\Psi =U\Psi$ Where U = Unitary Time Evolution Operator; $U^+=U^{-1}$ 
5. Using time-dependent Schrödinger equation: $H(t)U(t,t_0)=ih dU(t,t_0)/dt$
6. $U(t_0,t_0)=I$; Initial condition. Do nothing. Hamiltonian Op.(Self-Adjoint drives the evolution of the unitary time evolution op.)
7. M = [2,5]; measurement outcome. X_M(A) gives Probability of getting the value inside M
8. Use a big system to make the weak $\psi$ interact and observe the change: Time evolution + projective measurement.(refer: [[Weak or Generalized Measurement]])
9. $O \leftrightarrow \hat{O}$ VERY HARD (NONTRIVIAL)
#### Further Tools
1. [[Relation between Unitary and Self-Adjoint Operators]]
2. [[Stone's Theorem]]
3. [[Extra on Tensor Product]]
4. [[Tensor Product vs Addition of Operators]] 