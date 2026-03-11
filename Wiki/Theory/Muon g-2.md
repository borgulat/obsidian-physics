
#### Theory

The magnetic dipole moment is
$$
\vec{\mu} = g \frac{Q}{2m}\vec{s}
$$
where classically, $g=1$, while the Dirac equation predicts $g=2$.

One defines the anomalous deviation $a$ from $g=2$ via $g=2(1+a)$.
Then, $a$ can be calculated perturbatively as
$$
\bra{\psi(p)}j^\mu(q)\ket{\psi(p')} \sim Q
\bar{u}(p')\left[\gamma^\mu F_1(q^2) + \sigma^{\mu\nu}q_\nu F_2(q^2)\right]u(p)
$$
where the result has been expressed in terms of **form factors / structure functions** $F_1$ (corresponding to the electric charge) and $F_2$ (corresponding to $\vec{\mu}$).
- Since $F_1$ corresponds to the electric charge which is exactly $e$, we have $F_1(0)=1$
- $F_2(0)=a$

Thus, one wants to calculate $F_2$. For this, one can project the amplitude onto the $\sigma_{\mu\nu}$ structure. The vertex receives higher-order corrections from all SM particles, including QCD.

**Predictions:**
- Perturbative first order QED correction is $a_\mu=\alpha/(2\pi)$
- A hadron loop in a photon line is at low energies and thus requires lattice calculations
	- The loop can be a photon propagator correction, then it is called **Hadronic Vacuum Polarization**
		- This can be related to the $e^+e^-\rightarrow\text{hadrons}$ rate via the optical theorem (or its ratio to muon production, the **R-Ratio**):
		 ![[Pasted image 20260306154607.png|533]]
		- Or one expands the HVP as an OPE in terms of composite operators and uses lattice expectation values of these
	- The loop can connect to the muon via three photons, called **light-by-light** scattering
	 ![[Pasted image 20260306154543.png]]
	- Here the Optical theorem cannot be used and one must resort to lattice calculations




#### Experiment

- Brookhaven National Laboratory / Fermilab
- Uses Larmor precession of muons in a storage ring


#### Current status

- The data-driven approach using the optical theorem has suffered from inconsistent data and predicted a value which deviated from the measurement
- Lattice calculations have replaced this approach since 2020 and now theory and experiment almost agree
- However, it is still unclear why the data-driven approach and lattice QCD disagree so much













