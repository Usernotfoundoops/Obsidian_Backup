1. We can obtain any Self-Adjoint operator from their corresponding Unitary Operator.
2. Only applicable to 1 PUG ($U_k = e^{ikA}$), where k is the parameter.
3. H (Hamiltonian Op.) is the generator of Time Evolution Operator $U_k$
4. $\hat{p}$ (Momentum Op.)is the generator of Translation Operator $T_\delta$ in Hilbert Space
5. We use power -ve for e in Unitary Op cause that's how it works in physics. The exp oscillates instead of growing exponentially. 
6. ![[Pasted image 20260315124957.png|419]]
Math:
## Recovering H and p using Stone's Theorem

$$A\psi = -i\frac{d}{dk}\bigg|_{k=0} U_k\psi$$
### Example 1 — Hamiltonian H from time evolution $U_t$

$$U_t = e^{-iH\frac{t}{\hbar}}$$

Substitute into Stone's theorem with $k = t$:

$$A\psi = -i\frac{d}{dt}\bigg|_{t=0} e^{-iH\frac{t}{\hbar}}\psi$$

Differentiate the exponential:

$$= -i \cdot \left(\frac{-iH}{\hbar}\right)\psi$$

$$= \frac{(-i)(-i)}{\hbar}H\psi$$

$$= \frac{i^2 \cdot (-1)}{\hbar} \cdot (-1) H\psi = \frac{-H}{\hbar}\psi$$

Generator $A = -\frac{H}{\hbar}$ $\implies$ **H appears** ✓

The negative sign and $\hbar$ are convention — physics defines $U_t = e^{-iHt/\hbar}$ to give oscillating solutions in Schrödinger equation.

### Example 2 — Momentum p from translation $T_{\vec{\delta}}$ (Check rough note for easy solving[Day1-2])

$$(T_{\vec{\delta}}\psi)(\vec{x}) = \psi(\vec{x} - \vec{\delta})$$

Substitute into Stone's theorem with $k = \delta$:

$$A\psi = -i\frac{d}{d\delta}\bigg|_{\delta=0} \psi(\vec{x} - \delta)$$

By chain rule:

$$= -i \cdot (-1)\frac{d}{dx}\psi(\vec{x})\bigg|_{\delta=0}$$

$$= \frac{-i \cdot (-1) \cdot \hbar}{\hbar}\frac{d}{dx}\psi(\vec{x})$$

$$= \frac{1}{i\hbar} \cdot (-\hbar)\frac{d}{dx}\psi = \frac{\hbar}{i}\frac{d}{dx}\psi$$

Generator $A = \frac{\hbar}{i}\frac{\partial}{\partial x} = p_x$ $\implies$ **p appears** ✓
