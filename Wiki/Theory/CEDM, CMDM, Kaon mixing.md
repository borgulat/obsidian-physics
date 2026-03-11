# Relevance and program

- Neutron was first system where an intrinsic EDM has been tried to measure
- Current experimental **upper bound 6 orders of magnitude larger** than SM prediction
- Contributions from several operators below the EW scale (low energies since neutron is a low-energy bound state). The **flavor-diagonal sources** are:
	- Dimension 4: Theta term
	- Dimension 5: CEDM
	- Dimension 6: 3-gluon operator ("Weinberg operator")
- There are also **flavor off-diagonal sources**:
	- CKM matrix (SM): CP-violating complex phase in flavor-changing interactions
	- CP-violating flavor-changing 4-quark operators (originating from integrating out EW particles for LEFT or from BSM physics)

- To constrain the contributions to the nEDM (i.e. the Wilson coefficients) we need high-precision neutron matrix elements.

## Baryogenesis

**Baryon to photon density ratio:**
 - $\eta=(n_B-n_\bar{B})/n_\gamma \approx 10^{-10}$ (Planck 2018)  measures baryon asymmetry and the numerator makes it invariant under the scale factor of the universe. Calculate from:
	- predictions of the light nuclei abundances in **Big-Bang Nucleosynthesis** (BBN) models
		- Higher baryon density -> more nuclear burning -> less left-over deuterium
	- independently, from the **CMB angular power spectrum** (i.e. temperature as function of direction in sky)
		- In the early universe baryons and photons were tightly coupled and formed a fluid in which acoustic waves caused overdensities
		- Baryons add inertia to the fluid, changing the moments in the power spectrum
 
**Sakharov conditions**
1. B-violation: Nature needs to allow excess of matter
2. CP-violation: Otherwise, excess of matter and excess of matter possible and would cancel on average
3. Out of **thermal equilibrium**:
	- In thermal equilibrium the reverse of every process is equally probable (otherwise the system would change -> it would still be in the thermalization process) -> no excess of matter creatable
	- Expansion of the universe and EW SB phase transition provide non-equilibrium states
		- Problem: EW SB with observed Higgs mass is a second-order transition which does not create bubbles with a discontinuous boundary (which is needed; matter excess are caused by CP-violating boundary reflection rates)
		- Possible solution: Extended Higgs sector
	- Problem for BSM scenarios: If they generate baryons at GUT scale, anomalous B-violation in SM would wash this out
		- In SM, B and L numbers (more generally, the baryon and lepton currents) are anomalously non-conserved (just as the axial current in QCD). Only B-L is conserved.
		- The vacua corresponding to fixed B and L can transition via sphalerons at high temperatures

## nEDM

#### Discrete Symmetries & Non-relativistic limit

The QFT description of EDM and MDM is given by
$$
\mathcal{L} = \mu\,\bar{\psi}(\sigma\cdot F)\psi + id\, \bar{\psi}(\gamma_5\sigma\cdot F)\psi
$$
where the MDM is CP-even and the EDM is CP-odd. 
The non-relativistic limit results in
$$
H = \mu\, \vec{J}\cdot\vec{B} + d\, \vec{J}\cdot\vec{E}
$$
**Caveats:**
- In the non-relativistic limit there is no consistent definition of C since it swaps the $(0,1/2)$ and $(1/2,0)$ representations (fundamental & anti-fundamental) of the SU(2) factors of the Lorentz Group.
- Since in the non-relativistic limit, the Lorentz Group is broken, there is no C symmetry. In the table below I thus just defined C:=PT (since P, T are still defined).
- Analogously, I define CP:=T and get the expected transformations for the MDM (CP-even) and EDM (CP-odd) 

| Quantity                  | P   | T   | C:=PT |     | CP:=T | CPT (assumed) |
| ------------------------- | --- | --- | ----- | --- | ----- | ------------- |
| $\vec{J}$                 | +   | -   | -     |     | -     | +             |
| $\vec{B}$                 | +   | -   | -     |     | -     | +             |
| $\vec{E}$                 | -   | +   | -     |     | +     | +             |
| **$\vec{J}\cdot\vec{B}$** | +   | +   | +     |     | **+** | +             |
| **$\vec{J}\cdot\vec{E}$** | -   | -   | +     |     | **-** | +             |
| $H$                       | /   | /   | /     |     | /     | +             |
For the neutron, we can picture this like this:
![[Pasted image 20260301151827.png|205]]
- B transforms the same as J, so  $\vec{B}\cdot \vec{J}$  is P-even and T-even.
- E transforms opposite to  J, so  $\vec{E}\cdot \vec{J}$  is P-odd  and T-odd (and thus CP-odd).

#### Why the neutron? / Experimental techniques

**Why the neutron?**
- We want a strong E-field to measure the EDM
- Thus, use neutral particles which are not accelerated in this field -> neutron

**Idea of nEDM experiments**
- Measure **precession of neutron spin**
- This is caused by electric and magnetic **Larmor precession**.
	- The dipole moments are parallel to the spin: $\vec{\mu}=c_\mu \vec{J}$, $\vec{d}=c_d \vec{J}$
		- Classically, $c_\mu=\gamma$ (Bohr Magneton)
	- Classically, they generate a torque 
$$\vec{M} = \vec{\mu}\times\vec{B} + \vec{d}\times\vec{E}=\vec{J}\times(c_\mu \vec{B}+c_d\vec{E})$$
	- And the angular momentum is classically related to the torque my
$$
\dot{\vec{J}} = \vec{M}= -(c_\mu \vec{B}+c_d\vec{E})\times J
$$
	- Expressing the cross product with a matrix (a rotation matrix), this means that J rotates with a frequency given by the Frobenius-Norm of the matrix. For parallel/antiparallel E and B fields, the frequency is

$$
\nu_\pm = \mu B \pm d E
$$
	- Measuring both values and knowing E, B and $\mu$, one can calculate $d$
- **Experimental requirements:**
	- Strong parallel/antiparallel E- and B-fields (15kV/cm, 1$\mu$T)
	- Extremely small EDM component ($10^{-7}$ Hz instead of 29 Hz for  MDM)
		- Need long interaction time with E
			- Use ultracold (i.e. slow) neutrons. Example (TRIUMF):
				- Produced by proton beam hitting dense target
				- Cooled by passing kinetic energy to heavy water
				- Cooled further by phonon-emission in superfluid helium
				- Resulting interaction time ~100 seconds
			- These can be reflected and thus trapped
		- High neutron flux
		- Precise control over B
	- Example experiments:
		- n2EDM (PSI, Villingen)
		- TUCAN (TRIUMF, Vancouver)
		- nEDM@SNS (Spallation Neutron Source, Oak Ridge, Tennessee)
		- beam nEDM (European Spallation Source, Sweden)
	- Electrons (storage rings) Atoms and Molecules can also be used to probe CP violation
		- **JEDI (Jülich Electric Dipole moment Investigation) looks for proton EDM at COSY**



## nEDM calculation

The nEDM appears as an interaction of the neutron with the electromagnetic field. It thus appears as a matrix element of the EM vector current between neutron states.

Covariant decomposition of this matrix element involves the structure functions / form factors:
$$
\bra{n(p_1)}J^\mu_\text{EM}\ket{n(p_2)} = \gamma^\mu F_1(p) + \sigma^{\mu\nu}p_\nu F_2(p) + \gamma_5\sigma^{\mu\nu}p_\nu F_3(p)
$$
where  $p=p_1-p_2$  and $F_2$ and $F_3$ are suppressed by $p^2=m_n$ by dimensional analysis.

The nEDM is then given by
$$
d_n \sim e\,F_3(p^2=0) \,.
$$
On the lattice, $F_3$ is calculated from $n$-point functions with insertions of the EM current and CP-violating operators between neutron states.

## nEDM Sources

- In SM the CKM matrix and $\theta$ term are only sources of CP violation

#### CKM matrix

We treat the neutron as (u,d,d) bound state. The nEDM can come from
- EDMs of single quarks $d_u$ and $d_d$ . In the nucleon, a photon can couple to all quarks according to their charges (+2/3, -1/3) and thus we get
	$$
	d_n \sim \frac{2}{3} \cdot 2d_u - \frac{1}{3}\cdot d_d
	$$
	- However...
		- At 1-loop, CKM elements are always multiplied by their conjugate and no imaginary part remains
		- At 2-loop, CKM unitarity forces the sum over all diagrams to vanish (GIM-like mechanism)![[Pasted image 20260301210634.png]]
	- The result is thus extremely suppressed (~$10^{-34}$).
	
- If we take multiple quarks into account, the nEDM becomes a 1-loop effect:
	![[Pasted image 20260301211056.png]]
	- One 1-loop contribution to the blop in the LHS diagram is the $\Delta S=1$ strong penguin diagram on the RHS
	- This diagram has a factor
		$$
		 V=V_{dt}^* V_{ts} V_{su}^* V_{ud}
		 $$
		- For the CMK elements and conjugation remember:
			- Go against fermion line.
			- If we ascend from down-type to up-type, there is a star.
			- If we descend from up-type to down-type, there is no star.
	- This factor is a Jarlskog invariant which indicates CP violation (showing this only amounts to tedious calculations)

#### Theta Term

QCD admits a term
$$
\mathcal{L}_\text{QCD} \ni \theta G_{\mu\nu}^a \tilde{G}^{a,\mu\nu}
$$
and also a complex mass matrix. However, any complex mass matrix can be rotated aways using the chiral anomaly (the axial trafo removes the complex mass matrix and inserts the topological charge instead).

Lattice calculations (which suffer from bad signal-to-noise ratio) have yielded $d_n\approx 10^{-16} \theta \, e\, \text{cm}$. The current upper bound $d_n<10^{-26}\,e\,\text{cm}$ thus implies $\theta<10^{-10}$.

- This is the **strong CP problem**
- Possible solutions:
	- Peccei-Quinn mechanism (ruled out experimentally) and its variants (still possible):
		- Introduce new complex scalar field $\phi$ (in addition to Higgs)
		- $\phi$ only couples to down-type quarks, Higgs now only to up-type
		- Spontaneusly breaking a new chrial symmetry leads to the new scalar field to take a VEV which cancels out the $\theta$ term

#### CEDM on the Lattice

Here the challenge is the complicated renormalization pattern on the lattice. This is solved by the GF with an SFTX in the usual way.

The CP-odd form factor contributing to the nEDM, arising from the CEDM, has been calculated **[here](https://inspirehep.net/files/aa2042e1c936f534bf016e1754cb1789)** (Cirigliano et al. 2018), for example. They calculate a CP-violating phase of the neutron, however.

So far, lattice results still need to be improved (continuum limit, finite-volume effects) in order to use the results to, e.g., constrain BSM model parameter space.

For related results, there are sufficient results already (see **[here](https://arxiv.org/pdf/1506.04196)**):
- There they calculated tensor charges contributing to the EDMs of light quarks
- Tensor charges are charges of quark tensor bilinears $\bar{\psi}\gamma_5\sigma_{\mu\nu}\psi\,$. They correspond to quark-level CP-violating dipole operators originating from BSM models
	- This is similar to the CKM contribution to the nEDM via single quark EDMs described above
- The current results can be used to constrain BSM parameters (e.g. in Supersymmetry)




## CP violation in Kaons and CMDM contributions thereto

The CMDM appears in supersymmetric contributions to neutral Kaon oscillations, specifically in the $\epsilon'/\epsilon$ ratio.

#### Prerequisites: Eightfold Way

Since the 3 lightest quarks are much lighter that the other ones, they can be approximated as massless and then form the basis of a fundamental $SU(3)$ flavor group.
- The quarks transform in the fundamental $3$ representation
- The antiquarks transform in the antifundamental $\bar{3}$

The mesons consist of two quarks. Thus, they transform in the $\bar{3}\otimes 3=1\oplus 8$ representation.
- The singlet part $1$ corresponds to $\eta'$.
- Concerning the $8$ part with Gell-Mann-Matrices as generators:
	- Diagonal matrices correspond to the physical mesons $\pi^0$ and $\eta$
	- Off-diagonal ones combine into charge-definite states which correspond to
		- $\pi^+$, $\pi^-$
		- $K^+$, $K^-$
		- $K^0$, $\bar{K}^0$

#### Prerequisites: Parity & Kaons

**Fermions and antifermions have opposite parity.**

Thus, scalar mesons ($q\bar{q'}$) all have Parity $-1$. (Since they are bosons, their antiparticles have the same parity). Charge conjugation exchanges the constituent quarks with their antiquarks. We thus have the following properties:

| Particle    | Content                                                 | Spin | Parity | Lifetime (s) | Decay                       | Charge conjugated |
| ----------- | ------------------------------------------------------- | ---- | ------ | ------------ | --------------------------- | ----------------- |
| $\pi^+$     | $u\bar{d}$                                              | 0    | -1     | $10^{-8}$    | $\mu^++\nu_{\mu}$           | $\pi^-$           |
| $\pi^-$     | $\bar{u}d$                                              | 0    | -1     | $10^{-8}$    | $\mu^-+\bar{\nu}_{\mu}$     | $\pi^+$           |
| $\pi^0$     | $u\bar{u}-d\bar{d}$                                     | 0    | -1     | $10^{-17}$   | $2\gamma$                   | $\pi_0$           |
| $K^+$       | $u\bar{s}$                                              | 0    | -1     | $10^{-8}$    | $\mu^++\nu_{\mu}$           | $K^-$             |
| $K^-$       | $\bar{u}s$                                              | 0    | -1     | $10^{-8}$    | $\mu^-+\bar{\nu}_{\mu}$     | $K^+$             |
| $K^0$       | $d\bar{s}$                                              | 0    | -1     | NAN          | NAN                         | $\bar{K}^0$       |
| $\bar{K}^0$ | $\bar{d}s$                                              | 0    | -1     | NAN          | NAN                         | $K^0$             |
| $K_L$       | $\frac{K_{CP+}+\epsilon K_{CP-}}{\sqrt{1+\epsilon^2}}$  | 0    | -1     | $10^{-8}$    | $3\pi^0$<br>$2\pi^0$ (rare) |                   |
| $K_S$       | $\frac{\epsilon K_{CP+}+ K_{CP-}}{\sqrt{1+\epsilon^2}}$ | 0    | -1     | $10^{-11}$   | $2\pi^0$<br>$3\pi^0$ (rare) |                   |

The neutral Kaons are P-eigenstates (eigenvalue -1), but no C-eigenstates as they transform into each other:
$$
CP\ket{K_0}=-\ket{\bar{K}_0}\,,\qquad CP\ket{\bar{K}_0}=-\ket{K_0}
$$

Assuming that CP is not violated, the physical states would thus be the CP-eigenstates
$$
\ket{K_{CP+}} \sim \ket{K_0}-\ket{\bar{K}_0} \,,\qquad 
\ket{K_{CP-}} \sim \ket{K_0}+\ket{\bar{K}_0}
$$
Since  $CP\ket{\pi^0}=-\ket{\pi^0}$,  the CP-even state could only decay into $2\pi^0$ and the CP-odd one only into $3\pi^0$. But rarely, the opposite happens, implying that **the physical states violate CP.**

The actual physical states are thus mixtures of the CP-eigenstates:
$$
K_L = \frac{K_{CP+}+\epsilon K_{CP-}}{\sqrt{1+\epsilon^2}} \,,\qquad
K_S = \frac{\epsilon K_{CP+}+ K_{CP-}}{\sqrt{1+\epsilon^2}}
$$
with a small number $\epsilon\approx 10^{-3}$. Since this CP violation can only be observed in the products of the decay, it is also called **indirect CP violation**.

The SM explanation for this is that both neutral Kaons can decay into each others decay products since they transform into each other via CP-violating weak interactions involving Jarlskog-like combinations of CKM elements:
![[Pasted image 20260303164202.png|200]]

**Direct CP-violation** is seen in the $K^+$ decay into $\pi^+\pi^+\pi^-$ as well as into $\pi^+\pi^0$, which have opposite parity.

In the decays of a Kaon into pions, a strange quark must be converted into a $d$ quark (since the pions have no strangeness, while the Kaon has). This conversion includes penguin diagrams like this:
![[Pasted image 20260303172218.png|290]]

Integrating out the top quark and the W boson gives rise to the CMDM operator. BSM models modify its contributions. **This has already been used to constrain BSM models.**

For example, the CMDM appears in a 2019 **[paper](https://pdf.sciencedirectassets.com/271623/1-s2.0-S0370269319X00040/1-s2.0-S0370269319302485/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjENj%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJHMEUCIQCMYUsngtgC33OHyUGmbFSw79Zy12aMSS5Zd8HTKCN7bAIgJT1s5hWltUZSyGH7OUcx%2FK32h1SffglZ86OQwCBZOxYqvAUIof%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAFGgwwNTkwMDM1NDY4NjUiDCTOegymunoKiwDYNSqQBX1uO4FNhBv7DFO83Xz%2BVy91s%2BL6eqimyyDX%2FfDKChI%2BW1AZewBtBHYXCu%2BQ%2B5YK%2F0MiBKAtXOLii8Y0hVFFApnvdrnctpjFyjmUTnHoRSoRz%2BKORNjcX%2FZLVzapgI0o1fNCH9W713sTb8Clwt0ot9aqybSZBlB6BJvGYyUkqlxSUm6LsG5vnCegJ55P4SBkmYj7LentVyRgAWhkY6rbLofbNeUSr9O2gLcHIPDpkThTBFPO4xFTPXNIb%2FzpjPSzyJE8sj5SvNFV3SXcIr0VMkATK%2FK%2FpyQYf5HgxnkLDAapUhSei9wXNMBCUI87dZ1kxclhuyyYl5rqRiZV%2BvT4NVuD0EP9EUzslUH6RPOjrZPrK5mPdopacbEtXFQ6BVNfOcdouEJjHquyVMqMCNbVKqggcOvdoBbxR7i%2BGihno%2Fd7td9qhkXVVjnyb2yo2%2Bx7d%2BmGIzprUHDPQpf%2Bi%2BuLXexKW8PojCqKcueEP7aLPRK3E6uMuttFNeq4XDuHbdPGSAldlzKKfaOOoxeUt%2BHNNSxB9G2Fiarx86rhP5rDxCLqjYVjsXqumUT%2FUfEPT%2FfqmQUdEgSU7uU2vqKF8KwFschWgfozmgYhrHK%2BFdjVKkvY24j7bnOv1WA3xW%2FviCfURXBNn6RDsP0wPrP5nj%2FmhL1FD%2BuXDcfoeiT1WB9Mh7cDeDkPK5wecmF7bbqnbcROobWTjokDpeKvBQhH%2FDyi3js04SzpeCX%2FO%2F37PlEChD0ySD1eqt0r4VkW750fMPPz24pujavj5sWHnAykMeYLvmAV9Ew510SlO7RyV9tMc5rEoSSR8d0UhUmAJQI439lEC%2B9P8jAQdz9s2aEpqwgDPU9q3cGe3rdtS8nRKWg3WwXxMPL9m80GOrEBk%2BB%2FzMGwT3ICdEgpOxcyZUcF2G0Whs0cMp0f7wjmT2eFN5f6nXjX8tL8nesPWd3O4LZbLYjRr8yUHFYrlGv4kB37OxQLSGZ3sLzym8vTWwgO7QX6nek9EHqtLvP%2BLiESGN6K6Qtm0O8mNE0MbZpbk9ns2NA0w1IcWDCP09ERGhMrUyd70qCz%2B6IwLwClZZ92SQs8gAfvPoffBhdElIxJkgmKTQfMavJeqSEH3kM0aCzY&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20260303T162705Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTYXZQAWTP7%2F20260303%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=376bad3abbd997a696b567f1247cac75e444c08ede0fb538f516a923f42fa061&hash=373aa6f382df0c6784719103634c8aacb581f121aff385601a25283eccd4a199&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0370269319302485&tid=spdf-bd1f6011-4176-43bc-b5fb-f9aefa647468&sid=b9b8cf1b8fc58049972a26085deaadf100d2gxrqb&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&rh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=1e0a5f05560f515e0f0b&rr=9d6a01aecafd340d&cc=de)** by Buras, Aebischer et al. where they use Lattice calculations of effective operators to constrain BSM parameters. This investigation was due to some slight tensions between lattice and experimental results on $\epsilon'/\epsilon$.




## Group theory from chiral symmetry breaking


![[Pasted image 20260308120443.png]]