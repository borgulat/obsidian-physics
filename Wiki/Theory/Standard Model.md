## Lagrangian

Gauge part:
$$
\mathcal{L}_\text{gauge} =
-\frac{1}{4}B_{\mu\nu}B^{\mu\nu}
-\frac{1}{4}W_{\mu\nu}W^{\mu\nu}
-\frac{1}{4}G_{\mu\nu}G^{\mu\nu}
+\frac{\theta}{32\pi^2}G_{\mu\nu}\tilde{G}^{\mu\nu}
$$
- For discussion of theta terms see below

Fermion kinetic part:
$$
\mathcal{L}_{FKO}=\sum_f \bar{\psi}_f\, i\,\slashed{D}\,\psi_f
$$
- where $f$ runs over all fermions ($Q_{L;1,2,3},\ L_{L;1,2,3},\ u_{R;1,2,3},\ d_{R;1,2,3},\ l_{R;1,2,3}$).

Scalar sector:
$$
\mathcal{L}_\text{scalar} = (D_\mu\phi)^\dagger(D^\mu\phi) + \mu^2\phi^\dagger\phi - \lambda (\phi^\dagger\phi)^2
$$

Yukawa sector:
$$
\mathcal{L}_\text{Yukawa} =
  (\bar{L}\ Y_l\ l_R + \bar{Q}\ Y_d\ d_R)\phi 
\quad + \quad (\bar{L}\ Y_\nu\ \nu_R + \bar{Q}\ Y_u\ u_R) \phi^C
\quad + \quad\text{h.c.}
$$
- The charge conjugated Higgs field is $\phi^C=i\sigma_2\phi^*$
- The $Y$ are $3\times3$ Yukawa matrices in flavor space
- For massless neutrinos, set $Y_\nu=0$

#### Accidental symmetries
These are additional global symmetries not required by construction
- Baryon number: $\text{U}(1)$ for quark doublets and singlets
- Lepton number: $\text{U}(1)$ for lepton doublets and singlets
	- This splits into 3 separate $\text{U}(1)$ for each lepton flavor if neutrinos are massless since then there are no Yukawa terms mixing different lepton flavors

#### Theta terms

- Theta terms originate from topology:
	- The theta term integrates to a boundary term
	- The boundary of $\mathbb{R}^4$ at infinity is $S^3$
	- At this boundary, any gauge field with group $G$ becomes a map $G\rightarrow S^3$
		- These maps are classified by the homotopy group $\pi_n(S^3)$ where $n$ is the dimension of an $n$-spherical sub-group of $G$.
	- We have $\pi_1(S^3)=0$, $\pi_2(S^3)=0$,  $\pi_3(S^3)=\mathbb{Z}$
	- Thus, any group which has $\text{SU}(2)$ as a subgroup has a nontrivial mapping to the space-boundary and at least a $\mathbb{Z}$-valued topological quantum number
- U(1)
	- Theta term has no physical consequences since $\pi_1(S^3)=0$
- SU(2)
	- Theta term could be physical since $\pi_3(S^3)=\mathbb{S}$
	- The anomaly allows one to exchange the theta term for a complex phase in the Yukawas
	- Since only the left-handed doublets are affected by SU(2), the right-handed singlets can be used to eliminate the complex phase in the yukawas
	- Thus, there is no physical consequence
- SU(3)
	- Since SU(2) is a subgroup of SU(3), the theta term has non-trivial topology
	- Since QCD conserves parity (acts on the doublets and singlets in the same way), one might replace the theta term by a phase in the Yukawas, but this phase cannot be removed from there
	- Thus, the QCD theta term is physical


#### EW Boson masses

The W boson can be written as
$$
W_\mu = W_\mu^1 I^1 + W_\mu^2 I^2 + W_\mu^3 I^3
$$
with the Pauli matrices $I^i$. The W charge is directly given by $I^3$, but it does not commute with $I^1$ and $I^2$, so one expresses them instead of charge-eigenvectors, $I^{1,2}\sim I_+ \pm I_-$, leading to
$$
W_\mu = W_\mu^+ I^+ + W_\mu^- I^- + W_\mu^3 I^3
$$
One can then rewrite the Higgs FKO as
$$
(D_\mu\phi)^\dagger(D^\mu\phi) \ni \frac{1}{4} g_2^2v^2 W^+_\mu W^-_\mu 
+ \frac{1}{2} (B_\mu,\ W_\mu^3)
\begin{pmatrix}
g_1^2 & g_1g_2 \\
g_1g_2 & g_2^2
\end{pmatrix}
\begin{pmatrix}
B_\mu \\
W_\mu^3
\end{pmatrix}
$$

The mass matrix can be diagonalized with the transformation
$$
\begin{pmatrix}
B_\mu \\ A_\mu
\end{pmatrix}
=
\begin{pmatrix}
\cos\theta_W & \sin\theta_W \\
-\sin\theta_W & \cos\theta_W
\end{pmatrix}
\begin{pmatrix}
A_\mu \\ Z_\mu
\end{pmatrix}
$$
resulting in masses
$$
M_W = \frac{1}{2}g_2v \ ,\qquad
M_Z = \frac{1}{2}v\sqrt{g_1^2+g_2^2} \ , \qquad
\cos\theta_W = \frac{M_W}{M_Z} \ .
$$


#### CKM and PMNS matrices

We want to transform the Yukawa terms to the mass basis where we have no flavor mixing. We only consider the quark part,
$$
\mathcal{L}_\text{Yukawa, quarks} =
  \bar{Q}\ Y_d\ d_R\phi 
\quad + \quad \bar{Q}\ Y_u\ u_R \phi^C
\quad + \quad\text{h.c.}
$$
where after EWSB we have
$$
\phi = \begin{pmatrix}
\phi^+ \\
v+H+i\chi
\end{pmatrix}
$$
where H is the physical real Higgs field and $v$ is it's VEV. We are only interested in the terms of the Yukawas including the VEVs, so only the lower components of the $Y_d$ term and the upper components of the $Y_u$ term:
$$
\mathcal{L}_\text{Yukawa, quarks} \ \ni \
\bar{d}_L\ Y_d\ d_R + \bar{u}_L\ Y_u\ u_R
$$
The Yukawa matrices can be diagonalized with singular value decomposition to $Y_{x}=U_x^\dagger M_x V_x$ where $M_x$ is a diagonal real mass matrix.

The FKO derivative terms are flavor-diaonal, so they are left invariant under flavor rotations. We can thus use flavor rotations to eliminate the transformation matrices. 
- For the down-type Yukawas we do
	- $\bar{d}_L \rightarrow \bar{d}_L U_d$
	- $d_R \rightarrow V_d^\dagger d_R$
- And for the up-type ones we do
	- $\bar{u}_L \rightarrow \bar{u}_L U_u$
	- $u_R \rightarrow V_u^\dagger u_R$

This changes the W-interactions in the FKOs
$$
\mathcal{L}_{FKO}=\sum_f \bar{\psi}_f\, i\,\slashed{D}\,\psi_f
$$
given by
$$
(\bar{u}_L,\ \bar{d}_L) =
i\gamma^\mu
\begin{pmatrix}
0 & W^+_\mu \\
W^-_\mu & 0
\end{pmatrix}
\begin{pmatrix}
u_L \\ d_L
\end{pmatrix}
\sim \bar{u}_L\ \slashed{W}^+ d_L + \bar{d}_L\ \slashed{W}^- u_L
$$
Here diagonalization of the Yukawas results in
$$
\bar{u}_L\ (U_u U_d^\dagger)\ \slashed{W}^+ d_L \quad + \quad 
\bar{d}_L\ (U_u U_d^\dagger)^\dagger\ \slashed{W}^- u_L
$$
where $(U_u U_d^\dagger)=V_\text{CKM}$. The matrices $V_u$ and $V_d$ do not appear here since the FKOs of the right-handed particles are SU(2)-singlets.

If the up-type quarks were massless (no Yukawa terms), we would only require $U_d,\ V_d$ to remove the Yukawas and $U_u$ can be used to diagonalize the W-interactions, so there would be no flavor-changing processes. This also happens for massless neutrinos.

**Feynman rules:** "Ascend to the stars" as a general rule for the CKM matrix elements in W-interactions:
- Go against fermion line.
- If we ascend from down-type to up-type, there is a star.
- If we descend from up-type to down-type, there is no star.

**The CKM matrix has 3 CP-even and 1 CP-odd parameters:**
- We can do relative phase shifts of all quarks. For $n$ generations there are $2n$ quarks. However, for relative shifts the global phase is irrelevant, so this leaves $2n-1$ phase shifts.
- The CKM matrix is unitary, $V_\text{CKM}\in \text{U}(N)$, so it has $N^2$ real parameters. Considering the generators (which are antihermitian, so the diagonal is purely imaginary), there are
	- 3 off-diagonal real parameters
	- 3 off-diagonal imaginary parameters
	- 3 diagonal imaginary parameters
- The 3 off-diagonal real parameters $\theta_{12}$, $\theta_{23}$, $\theta_{13}$ generate real rotations under $\exp$ and thus cannot contribute CP violating relative complex phases between interfering diagrams.
- The remaining 6 parameters get reduced by $2n-1=5$ phase shifts to only $1$ CP-violating complex phase $\delta$.


#### Neutrino masses

The SM cannot explain the smallness of the neutrino masses. It could be explained by the **Seesaw mechanism:**
- The right-handed neutrinos required by Dirac (Yukawa) neutrino masses $m$ are sterile (no interactions beside Yukawas)
- Since $\nu_R$ is a singlet under all gauge groups, it admits a Majorana mass term $\nu_R^T M \nu_R$
	- This violates lepton conservation
- One can include both masses. Diagonalizing the resulting mass matrix results in two masses which have to fulfill $m_1m_2=m^2$. If $m_1\sim M_\text{planck}$ the other mass would be extremely small, explaining the small neutrinos masses.


## EW symmetry breaking

At the EWSB scale $\sim 200\ GeV$ the Higgs field acquires a VEV.
- The Higgs field can be written as a positively charged upper complex component

#### Electric charge
Through EWSB, the EW group SU$(2)$$\times$U$(1)$ breaks down to U$(1)_\text{EM}$ and the corresponding charges combine into the electric charge according to the **Gell-Mann-Nishijima formula:**
$$
Q=I_z + \frac{Y}{2} = \begin{pmatrix}
(Y+1)/2 & 0 \\ 0 & (Y-1)/2
\end{pmatrix}
$$
so the upper component (up-type quarks, $\phi^+$, neutrinos) always have one unit of charge more than the lower component (down-type quarks, $v+H+i\chi$, charged leptons).

For the right-handed fermions we have $Q=Y/2$, so 
$$
Y(e_R)=-2,\qquad Y(u_R)=+4/3,\qquad Y(d_R)=-2/3\,.
$$
$$
Q(e_R)=-1,\qquad Q(u_R)=+2/3,\qquad Q(d_R)=-1/3\,.
$$


#### Symmetry breaking

Symmetry breaking breaks some generators and leaves others unbroken. The Goldstone Theorem states that
- To each broken generator (i.e. $\tau^a_{ij}v_j \neq 0$) corresponds a Goldstone boson
	- These can be removed by the longitudinal part of the now massive gauge bosons with a gauge transformation
	- If the symmetry is approximate, then the Goldstone bosons are physical, but light
		- In the case of **chiral symmetry breaking**, this explains the small masses of pions
		- The $\eta'$ meson ($u\bar{u}+d\bar{d}+s\bar{s}$) however is much heavier (~900 MeV) than the $\eta$ ($u\bar{u}+d\bar{d}-2s\bar{s}$) since it is proportional to the identity matrix in flavor space, so it corresponds to a chiral U(1) symmetry which is anomalously broken. The $\eta'$ however is in the adjoint representation of SU(3) (~$\lambda_8$)
- The unbroken generators generate the remaining symmetry (like charge in EWSB)

Yukawa interactions with a scalar field acquiring a VEV generate mass terms for the fermions.


## Parameters

There are 19 free parameters in the minimal SM (with massless neutrinos) and 7 more (total 26) with massive neutrinos:

| #   | Parameter                | Value                                                                                | Description    | Alternative                                                | Measurement                                                                                             |
| --- | ------------------------ | ------------------------------------------------------------------------------------ | -------------- | ---------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| 1   | $m_e$                    | $0.5\, \text{MeV}$                                                                   | electron mass  | $y_e=\sqrt{2}m_e/v$                                        | Cyclotron frequency                                                                                     |
| 2   | $m_\mu$                  | $105\, \text{MeV}$                                                                   | muon mass      | $y_\mu=\sqrt{2}m_\mu/v$                                    | Kinematic reconstruction from decays                                                                    |
| 3   | $m_\tau$                 | $1776\,\text{MeV}$                                                                   | tau mass       | etc.                                                       | Kinematic reconstruction from decays                                                                    |
| 4   | $m_u$                    | $2\,\text{MeV}$                                                                      | up mass        |                                                            | Hadron mass splittings<br>Pion decay constants                                                          |
| 5   | $m_d$                    | $5\,\text{MeV}$                                                                      | down mass      |                                                            | ""                                                                                                      |
| 6   | $m_s$                    | $93\,\text{MeV}$                                                                     | strange mass   |                                                            | ""                                                                                                      |
| 7   | $m_c$                    | $1.2\,\text{GeV}$                                                                    | charm mass     |                                                            | Quarkonium spectra <br>($J/\psi,Υ$)                                                                     |
| 8   | $m_b$                    | $4\,\text{GeV}$                                                                      | bottom mass    |                                                            | ""                                                                                                      |
| 9   | $m_t$                    | $172\,\text{GeV}$                                                                    | top mass       |                                                            | Kinematic reconstruction of $t\bar{t}$ events                                                           |
| 10  | $m_H$                    | $125\,\text{GeV}$                                                                    | Higgs mass     | $\lambda=m_H^2/(2v^2)$                                     | Higgs resonance reconstruction<br>$h\rightarrow 2\gamma / 2Z \rightarrow 4l$                            |
| 11  | $v$                      | $246\,\text{GeV}$                                                                    | Higgs VEV      | $\mu^2=\lambda v^2$                                        | $G_F$ from muon decay (via $G_F\rightarrow M_W \rightarrow v$)                                          |
| 12  | $\theta_{12}^\text{CKM}$ | 13.1°                                                                                | CMK angle      |                                                            | Semileptonic decay rates (BaBar, Belle, LHCb)<br>$V_{us}:\ K\rightarrow\pi l \nu$                       |
| 13  | $\theta_{23}^\text{CKM}$ | 2.4°                                                                                 | CKM angle      |                                                            | $V_{cb}:\ B\rightarrow D l \nu$                                                                         |
| 14  | $\theta_{13}^\text{CKM}$ | 0.2°                                                                                 | CKM angle      |                                                            | $V_{ub}:\ B\rightarrow\pi l \nu$                                                                        |
| 15  | $\delta^\text{CKM}$      | 0.995=57°                                                                            | CKM phase      |                                                            | B-oscillation (time dependent decay rates)<br>                                                          |
| 16  | $g_1$                    | $g_1(m_Z)=0.3$<br>$\alpha(0)=1/137$<br>$\alpha(m_Z)=1/127$                           | U(1) coupling  | $\alpha=g_1g_2/(4\pi(g_1^2 + g_2^2))$                      | Electron MDM                                                                                            |
| 17  | $g_2$                    | $g_2(m_Z)=0.65$<br>$\theta_W=28.2°$<br>$m_W=80\, \text{GeV}$<br>$m_Z=91\ \text{GeV}$ | SU(2) coupling | $\theta_W=\text{tan}^{-1}(g_1/g_2)$<br>$m_W$, $m_Z$, $G_F$ | Total Z & W decay widths in LEP $e^+e^-\rightarrow Z \rightarrow \bar{f}f$ ;<br>Muon lifetime for $G_F$ |
| 18  | $g_3$                    | $g_3(m_Z)=1.221$<br>$\alpha_s(m_Z)=0.12$                                             | SU(3) coupling | $\alpha_s=g_3^2/(4\pi)$, $\Lambda_\text{QCD}$              | Hadronic Tau decay width;<br>Jet rates (2-/3-jet fractions);<br>Lattice QCD                             |
| 19  | $\theta_\text{QCD}$      | $<10^{-10}$                                                                          | QCD theta term |                                                            | nEDM                                                                                                    |

| #   | Parameter                 | Value                                                                                                                      | Description | Alternative | Measurement                                                                            |
| --- | ------------------------- | -------------------------------------------------------------------------------------------------------------------------- | ----------- | ----------- | -------------------------------------------------------------------------------------- |
| 20  | $\theta_{12}^\text{PMNS}$ | 33.4°                                                                                                                      | PMNS angle  |             | Neutrino oscillation (Solar neutrinos)                                                 |
| 21  | $\theta_{23}^\text{PMNS}$ | 49.1°                                                                                                                      | PMNS angle  |             | Neutrino oscillation (atmosphere)                                                      |
| 22  | $\theta_{13}^\text{PMNS}$ | 8.54°                                                                                                                      | PMNS angle  |             | Neutrino oscillation (nuclear reactors)                                                |
| 23  | $\delta^\text{PMNS}$      | 197°                                                                                                                       | PMNS phase  |             | $\nu_\mu\rightarrow\nu_e$ vs. $\bar{\nu}_\mu\rightarrow\bar{\nu}_e$ asymmetry          |
| 24  | $m_{\nu_e}$               | $\delta m_{12}^2 = 10^{-5}\ \text{eV}$<br>$\delta m_{23}^2 = 10^{-3}\ \text{eV}$<br>$\delta m_{13}^2 = 10^{-3}\ \text{eV}$ |             |             | Neutrino oscillation<br>($\nu_e$ survival from Sun and atmosphere)<br>Super-Kamiokande |
| 25  | $m_{\nu_\mu}$             |                                                                                                                            |             |             | ""                                                                                     |
| 26  | $m_{\nu_\tau}$            |                                                                                                                            |             |             | ""                                                                                     |
**Quark mass hierarchy:**
![[Pasted image 20260306124854.png|223]]

#### Notes for measuring the parameters

- The neutrino masses are constrained by KATRIN to be $<0.45\ \text{eV}$ (2024).
	- KATRIN filters beta-decay electrons through spectrometers to measure the intensity of the highest-energy electrons. The highest possible kinetic energy for the electron is reduced by the neutrino rest energy which can thus be measured. 
- Why B instead of K for $\delta$?
	- One could also use neutral Kaon oscillation ($\bar{d}s\leftrightarrow d\bar{s}$)
	- But in the Kaon all quarks are light, so the Kaon is dominated by $\Lambda_\text{QCD}$ which causes problems in the prediction
	- B mesons are dominated by the $b$ mass one can expand in
	- They also have the larger CKM matrix elements in the oscillation diagram, so the effect is stronger
	- Also, the transition is proportional to mass-squared differences (just like in neutrino oscillation). Combined with the CKM elements, the B mesons have larger amplitudes than the Kaons.

#### Lattice predictions of $\alpha_s$

- Phenomenological methods reconstruct $\alpha_s$ from collider processes.
- Lattice results provide the most precise determination of $\alpha_s$.


## Renormalization

The three gauge couplings behave differently under the RG. This plot shows the running of the inverse couplings dependent on $\log\mu$:
![[Pasted image 20260306101135.png|327]]
- The U(1) coupling (and the EM one as well) grows with $\mu$ (Landau pole) and is well-defined at $\mu=0$
- The SU(2) and SU(3) couplings decrease with $\mu$ (asymptotic freedom). At low energies:
	- SU(3) becomes non-perturbative around $\Lambda_\text{QCD}\sim 200\ \text{MeV}$, but actually perturbation theory is only viable at scales $>2\ \text{GeV}$.
	- SU(2) is broken at low energies, however, and the masses of the W and Z prevent SU(2) bound states, so SU(2) is still weak at low energies.

The couplings tend towards unification at $\sim 10^{13}...10^{17}\ \text{GeV}$. The Planck scale as a comparison is $10^{19}\ \text{GeV}$ and the EWSV scale is $v=10^2\,\text{GeV}$ (hierarchy problem).

#### Running of $\alpha_s$

- At the LHC $\alpha_s(m_Z)$ is measured.
- $m_Z=80\ \text{GeV}$ this is far away from the hadronic scale $m_n=932\ \text{MeV}\sim 1\ \text{GeV}$.
- So to compare this with lattice results, one has to run it using the RG flow.
	- Between the two scales there are the bottom and charm quarks
	- One thus runs
		- From $m_Z$ to $m_b$ using 5 active flavors (all except $t$)
			- Matching of 5- and 4-scheme at $m_b$
		- From $m_b$ to $m_c$ using 4 active flavors (all except $t,b$)
			- Matching of 4- and 3-scheme at $m_c$
		- From $m_c$ to $m_n$ using 3 active flavors ($u,d,s$)

Low-energy values are
- $\alpha_s(1\ \text{GeV}\sim m_n)=0.4$
- $\alpha_s(0.6\ \text{GeV}\sim m_n)=1.5$


## Unsolved problems

- Origin and smallness of neutrino masses
- Vacuum energy vs. Dark Energy

#### Strong CP problem (Fine tuning)

See CMDM.

#### Hierarchy problem

This is about contributions of a BSM $\Lambda$ scale to particle masses via loop effects, and subsequently about the strength of gravity vs the EW force:

- Gauge boson masses are protected by gauge invariance (requiring them to have zero mass in the unbroken phase)
- Fermion masses are protected by chiral symmetry requiring $\delta m \sim m \log(\Lambda/m)$
- Scalars have $\delta m \sim \Lambda$, so one would expect the Higgs mass to be of the order of the Planck scale
	- This translates to the EW force being $10^{24}$ times stronger than gravity since gravity is suppressed by the Planck mass and EW force is suppressed by the much smaller Higgs mass ($m_H/m_\text{Planck}\sim 10^{-17}$)

