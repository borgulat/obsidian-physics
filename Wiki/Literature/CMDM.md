# Relevance and program

- Neutron was first system where an intrinsic EDM has been tried to measure
- Current experimental **upper bound 6 orders of magnitude larger** than SM prediction
- Contributions from several operators below the EW scale (low energies since neutron is a low-energy bound state). The **flavor-diagonal sources** are:
	- Dimension 4: Theta term & complex CP-violating mass matrix. These are not Independent due to anomaly. If a quark was massless, the CP-odd terms could be rotated away.
	- Dimension 5: CEDM
	- Dimension 6: 3-gluon operator ("Weinberg operator")
- There are also **flavor off-diagonal sources**:
	- CKM matrix (SM): CP-violating complex phase in flavor-changing interactions
	- CP-violating flavor-changing 4-quark operators (originating from integrating out EW particles for LEFT or from BSM physics)

- To constrain the contributions to the nEDM (i.e. the Wilson coefficients) we need high-precision neutron matrix elements.

## Baryogenesis

**Baryon number density**
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
	- The dipole moments are parallel to the spin: $\vec{\mu}=c_\mu J$, $\vec{d}=c_d \vec{J}$
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

The current upper bound on the nEDM implies $\theta<10^{-10}$.
- This is the **strong CP problem**
- Possible solutions:
	- Peccei-Quinn mechanism (ruled out experimentally) and its variants (still possible):
		- Introduce new complex scalar field $\phi$ (in addition to Higgs)
		- $\phi$ only couples to down-type quarks, Higgs now only to up-type
		- Spontaneusly breaking a new chrial symmetry leads to the new scalar field to take a VEV which cancels out the $\theta$ term
