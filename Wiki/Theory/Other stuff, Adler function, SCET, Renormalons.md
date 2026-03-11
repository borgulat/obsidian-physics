
## Other stuff

- The top quark decays before hadronization allowing one to use on-shell mass instead of MS-bar mass


## Adler function & Decay Width

A vector boson **polarization function** is defined as
$$
\Pi_{\mu\nu}(q^2) \sim \int_x e^{iqx}\bra{0}j_\mu(0)j_\nu(x)\ket{0}
$$
and its transversal part is given by
$$
\Pi_{\mu\nu} =(q^2g_{\mu\nu}-q_\mu q_\nu)\Pi(q^2)
$$
Let $\Sigma(q^2)$ be the self-energy, i.e., the full amplitude of 1PI connected diagrams. The geometric series then implies
$$
\Pi(q^2)=\frac{1}{q^2-m^2-\Sigma(q^2)}
$$
The **Adler function** is then defined as as $d\Pi/d\log q^2$.

The photon has $m=0$ and its mass is protected, i.e., $\Sigma(p^2)$ is constrained by  $\Pi(q^2)\overset{q^2\rightarrow 0}{\sim}\frac{1}{q^2}$ .

A massive stable particle has $\Pi(q^2)\overset{q^2\rightarrow 0}{\sim}\frac{1}{q^2-m_\text{ph}^2}$ .
This can be used to define the on-shell scheme.

#### Unstable particles: Decay Width

Once $q^2$ reaches the energy threshold for production of some particle, the optical theorem implies that $\text{Im}(\Sigma)\neq 0$ and thus the pole is shifted in the $\text{Im}$ direction, creating a Breit-Wigner distribution
$$
\Pi(q^2) \sim \frac{1}{(q^2-m^2)^2+\Gamma^2m^2}
$$instead of a pole, where $\Gamma m\sim \text{Im}(\Sigma)$ . The Width is can be used to determine the mass of the decaying particle (e.g., the Z boson).


## SCET

Soft-collinear effective theory
- describes interactions of low-energy or collinear gluons and quarks
- It splits quarks and gluons into distinct modes
- It allows to factorize the soft-collinear scale from the hard scale

## IR subtraction

The Kinoshita-Lee-Nauenberg theorem states that IR divergences cancel when all contributions at a fixed order are taken into account (including degenerate initial/final states with soft/collinear particles).

At NNLO, e.g., one has `double-real + real-virtual + double-virtual` corrections. IR subtractions shifts the divergences between these contributions so they are separately finite.

## Renormalons

Renormalons are special types of divergences related to bubble-chain diagrams in the polarization functions. They lead to perturbative coefficients scaling like $c_n\sim n!$, spoiling perturbative convergence.


## QCD, Dimensional Transmutation

Start from the QCD beta function
$$
\mu\frac{d}{d\mu}a(\mu) = \beta(a)
$$
Since this is a first order ODE its solution is specified by one integration constant provided by the perturbative asymptote at $a\rightarrow0$ 
$$
\beta(a)= -\epsilon -a\sum_{n=0}^\infty a^n \beta_n
$$
The RGE can be solved: Writing $da/\beta(a)=d\mu/\mu$  we obtain
$$
\log\frac{\mu_1}{\mu_2} = \int_{a(\mu_2)}^{a(\mu_1)} \frac{dx}{\beta(x)} 
$$
Inserting the perturbative expansion, one finds
$$
\Lambda_\text{QCD}=\mu[\beta_0 g(\mu)^2)]^{-\beta_1/(2\beta_0^2)}
e^{-1/(2\beta_0 g(\mu)^2)} \exp\left\{-\int_0^{g(\mu)}dx\left[
\frac{1}{\beta(x)}+\frac{1}{\beta_0x^3}-\frac{\beta_1}{\beta_0^2x}
\right] \right\}
$$
which is independent of $\mu$ (although not manifestly).


## BRST symmetry

The full QCD Lagrangian is

$$
\mathcal{L}_\text{QCD} = -\frac{1}{4}F_{\mu\nu}^a G^{a,\mu\nu} + \bar{\psi}(i\slashed{D}-m)\psi + (\partial^\mu \bar{c}^a) D_\mu^{ab}c^b + \frac{1}{2\xi}(\partial^\mu A_\mu^a)^2
$$
The ghosts arise from the determinant of the Jacobian of the gauge-fixing condition. The Lagrangian is invariant under the BRST transformation
$$
\delta\psi=c^at^a\psi\ ,\quad \delta\bar{\psi}=\bar{\psi}t^ac^a
$$
$$
\delta A_\mu^a = D_\mu^{ab} c^b\ , \quad \delta c^a \sim f^{abc}c^bc^c\ ,\quad \delta \bar{c}^a=B^a\ ,\quad \delta B^a=0 ,
$$
where the EOM for the Nakanishi-Lautrup field imply $B^a=\partial_\mu A_\mu^a$.

One can add the BRST variations to the Lagrangian in the generating functional,
$$
\mathcal{L}_\text{BRST} = K_\mu^a \delta A_\mu^a + L^a \delta c^a
$$
where $K_\mu^a$ and $L^a$ are source terms (we ignore fermions for now). 
Making the sources BRST-invariant leads to a BRST invariant Lagrangian.

One can now define the effective action as usual as a Legendre-Transform. It satisfies the **Zinn-Justin equation**. It can be used to show that
- Counter-Terms are combinations of BRST-exact and gauge-invariant operators

