**Notable colliders:**
- Rutherford experiment: Scattering of $\alpha$ particles from gold nuclei
	- Proved the usability of scattering techniques
- Tevatron (...2011)
	- Circular $p^+p^-$ synchrotron at Fermilab
	- Discovered top quark & Higgs evidence
- SLAC (still operating)
	- Linear $e^+e^-$ collider at Stanford
	- Discoveries:
		- $\tau$ lepton and neutrino
		- Quark structure of nucleons
		- BaBar experiment (B mesons) found CP violation in agreement with SM
- LHC

**Comparison of accelerator types:**

| Type        | Pro                                                                                            | Con                                                                    |
| ----------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| Linear      | No beam bending and resulting energy loss, constant output of particles                        | Particles only accelerated once, thus lower energies than synchrotrons |
| Cyclotron   | Constant frequency, easy to build                                                              | Not scalable as the synchrotron                                        |
| Synchrotron | Scalable due to separated components, high energies since particles accelerated multiple times | Energy loss by synchrotron radiation                                   |


## Cyclotron

- Two semicircular electrodes inside a homogeneous magnetic field.
- In the gap between the electrodes the charged particles are accelerated
- The electrodes have an alternating current with constant frequency:
$$
F_\text{centripetal}=mr\omega^2, \quad F_\text{Lorentz}=q\omega rB
$$
$$
\Rightarrow \quad \omega = \frac{qB}{m}, \quad f=\frac{qB}{2\pi m}
$$
- Breaks down at relativistic speeds, then the frequency must change over time

## Synchrotron

- Particles accelerated in closed loop, with magnetic fields for bending the beam synchronized to their kinetic energy
- Consider bunches of (cross-sectional area $A$) of particles containing $N_A$ and $N_B$ particles colliding at frequency $f$
	- **Instantaneous Luminosity:** $L=\frac{N_A N_B}{At}$
		- Describes number of particle encounters per time and beam cross-sectional area
		- Important measure for collider capability
		- LHC: $10^{34}\ \text{cm}^{-2}\text{s}^{-1}$
	- **Integrated Luminosity:** Total particle encounters per beam cross-sectional area
		- Usually measured in $\text{pb}^{-1}=10^{36}\,\text{cm}^{-2}$ 
	- **Cross section:** $\sigma=N_\text{scatter}/(tL)=\frac{AN}{N_A N_B}$ 
		- This is the number of scattering events $N_\text{scatter}$ per time per luminosity
		- Or: Fraction of the beam cross-sectional area, corresponding to the scattering events per particle encounters
- Components:
	- **Dipole magnets:** Keep particles on proper path
	- **Quadrupole magnets** (and higher multipoles): Focus beam
	- **RF cavity:** Acceleration using a standing wave in the cavity
	- **Undulators:** Produce EM radiation by passing particles through static alternating magnetic field


## CMS
**Compact Muon Solenoid**

**Main goals:**
- Explore physics at TeV scale, search for BSM evidence
- Study heavy ion collisions
- Discover Higgs (achieved together with ATLAS)
- Further study Higgs properties

![[Pasted image 20260224123612.png]]

#### Components
Going from the beam to the outside:
- **Silicon Trackers:**
	- Principle:
		- Silicon is a semiconductor: The Fermi-Level (maximal ground state energy of an electron) lies between the valence band (which is full and the electrons cannot move) and the conduction band (which is empty). Thus, electron excitations produce electrons in the conduction band and holes in the valence band which can propagate.
		- Semiconductor detector: Particles create electron-hole pairs in silicon (semiconductor) which travel to electrodes at which a voltage is applied and produce a measurable current
		- There are pixels and strips
	- Use:
		- Reconstruct initial and secondary vertices
		- Measure finite particle lifetimes (e.g. b and tau)
		- Reconstruct intermediate particles (from trajectories not leading to initial vertex for example)
		- Measure momentum and charge from curvature of trajectory
- **Electromagnetic Calorimeter (ECAL):**
	- Principle:
		- Incoming electrons scatter off nuclei (interaction ~$Z^2$), produce photons which create $e^+e^-$ pairs which scatter etc., until all particles have reached low enough energy for ionization being able to absorb the rest of the enegry.
		- The Energy deposited in the material causes scintillation (passing charged particles create light by exciting electrons and/or holes and then falling back into ground state) which is used to measure the energy
	- Use:
		- Measure energy of primarily EM interacting particles (electrons, positrons, photons)
		- Segmentation allows measuring the particle direction
- **Hadron Calorimeter (HCAL):**
	- Principle:
		- Hadrons pass scintillators without interaction, so here scintillator layers alternate with the steel/brass layers creating energy loss
		- Hadronic showers are created by strong interaction between incoming hadrons and nuclei, forming new hadrons which then create further showers
	- Use:
		- Measure energy and direction of hadrons (protons, neutrons, pions, kaons) 
- **Superconducting Solenoid:**
	- 4 Tesla field
- **Muon Chambers:**
	- One of the main components of CMS
	- $H\rightarrow2\mu$ one of the main Higgs signatures
	- Because $m_\mu=105\ \text{MeV} = 200\,m_e$ they lose energy more slowly in matter and pass through the EM calorimeter
	- **Drift Tubes** contain gas which is ionized by muons; the ions move to electrodes and cause a measurable current. Thus, momentum and trajectory can be measured.
- **Return Yoke:**
	- Contains and guides the field
	- Allows through only muons and weakly interacting particles

For forward-scattering:
- **Preshower:**
	- Lead and silicon strip detector
	- Sits before the endcaps and allow distinction of interesting single high-energy photons and less interesting pairs of low-energy photons
		- Most photons come from well-understood $\pi^0\rightarrow\gamma\gamma$
			- The two photons are usually close to each other and can be distinguished from the single photon by the preshower detector
		- Single high-energy photons come from heavy particle decay (like Higgs or BSM particles) or early fundamental interactions (e.g. radiated from a quark directly)
- **Endcaps:**
	- EM calorimeters at the ends of the detector


## ATLAS
**A Toroidal LHC Apparatus**

**Main goals:**
- General purpose detector
- Search for BSM physics
- Higgs
- B physics
- Internal structure of leptons and quarks

![[Pasted image 20260224171124.png]]
#### Components
- Silicon pixel and stipe detectors
- ECAL
- HCAL
- 2 Tesla superconducting solenoid surrounding the above detectors
- Muon spectrometer (momenta measured by curving in toroidal magnetic field)
- Toroidal magnet surrounding the muon spectrometer



## Parameters and Coordinates

#### Rapidity
While for velocities in SRT we have
$$
v_\text{sum} = \frac{v_1 + v_2}{1+v_1 v_2} \ ,
$$
the rapidity defined as
$$\theta = \text{artanh}(v)$$
adds as usual: $\theta = \theta_1 + \theta_2$.

#### Pseudorapidity
Other than the rapidity, this is a spatial coordinate for the angle to the beam axis. It is used since the hadron flux is constant over pseudorapidity but not over the polar angle $\vartheta$. It is defined as
$$ \eta = -\ln (\tan (\vartheta/2)) = \frac{1}{2} \ln\left(\frac{|\vec{p}|+p_\parallel}{|\vec{p}|-p_\parallel}\right) .$$

