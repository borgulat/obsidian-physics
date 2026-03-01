Consider QED with effective dimension-five operators,
$$
\mathcal{L} = -\frac{1}{4}F_{\mu\nu}F^{\mu\nu}+\bar{\psi}(i \slashed{D}-m) \psi + O_\mathrm{EDM} + O_\mathrm{MDM}
$$
$$
O_\mathrm{EDM} = d \ \bpsi\, \sigma_{\mu\nu}i\gamma_5\,\psi \, F^{\mu\nu} \ ,\qquad
O_\mathrm{MDM} = \mu \ \bpsi\, \sigma_{\mu\nu}\,\psi \, F^{\mu\nu} \ ,
$$
where the EDM operator violates CP symmetry and the MDM one does not. (I neglected some constants of proportionality in the operators, like the gyromagnetic ratio).

In the non-relativistic limit this implies
$$
H = -\vec{\mu}\cdot\vec{B} - \vec{d}\cdot\vec{E}
$$
for the Hamiltonian, where
$$
\vec{\mu} = \frac{1}{2}\gamma\,\vec{\sigma} \,, \quad \vec{d}=\frac{1}{2}d\,\vec{\sigma} \,,\qquad \mathrm{where}\quad \gamma=-\frac{Qg}{2m} \quad \mathrm{for\ charged\ particles}.
$$
Note that the MDM and EDM are related to the spin operator and thus they are axial vectors (as opposed to the classical EDM which is polar). 

We can now check the transformations of the Hamiltonian and all its parts under C, P and T. We distinguish charged and uncharged particles since for charged particles the MDM flips while it does not for uncharged ones.
#### Transformations for charged particle

| Original | $Q$ | $\vec{s}$ |     | $\vec{d}$ ~ $Q\vec{s}$ | $\vec{E}$ | $\vec{d}\cdot\vec{E}$ |     | $\vec{\mu}$ ~ $Q\vec{s}$ | $\vec{B}$ | $\vec{\mu}\cdot\vec{B}$ |
| -------- | --- | --------- | --- | ---------------------- | --------- | --------------------- | --- | ------------------------ | --------- | ----------------------- |
| C        | -   | +         |     | -                      | -         | +                     |     | -                        | -         | +                       |
| P        | +   | +         |     | +                      | -         | -                     |     | +                        | +         | +                       |
| T        | +   | -         |     | -                      | +         | -                     |     | -                        | -         | +                       |
| CPT      |     | -         |     | +                      | +         | +                     |     |                          |           | +                       |
#### Transformations for uncharged particle (???)

| Original | $Q$ | $\vec{s}$ |     | $\vec{d}$ ~ $\vec{s}$ | $\vec{E}$ | $\vec{d}\cdot\vec{E}$ |     | $\vec{\mu}$ ~ $\vec{s}$ | $\vec{B}$ | $\vec{\mu}\cdot\vec{B}$ |
| -------- | --- | --------- | --- | --------------------- | --------- | --------------------- | --- | ----------------------- | --------- | ----------------------- |
| C        | 0   | +         |     | +                     | -         | -                     |     | +                       | -         | -                       |
| P        | 0   | +         |     | +                     | -         | -                     |     | +                       | +         | +                       |
| T        | 0   | -         |     | -                     | +         | -                     |     | -                       | -         | +                       |
| CPT      |     | -         |     |                       |           | -                     |     |                         |           | -                       |



Also, under T the B field and the spin change sign, but E does not. Thus
- P changes the sign of the EDM contribution and thus we get
$$
H\ \overset{P}{\longrightarrow} \ -\vec{\mu}\cdot\vec{B} + \vec{d}\cdot\vec{E}
$$
- T is antiunitary and thus changes the signs of B and the moments, but not E, and we obtain
$$
H\ \overset{T}{\longrightarrow} \ -\vec{\mu}\cdot\vec{B} + \vec{d}\cdot\vec{E}
$$
  again.
- C changes signs of E and B, but not the spin, thus
$$
H\ \overset{C}{\longrightarrow} \ +\vec{\mu}\cdot\vec{B} + \vec{d}\cdot\vec{E}
$$
We see that C, P and T are broken in this system separately and thus CP, CT and PT are broken, too.


## Sakharov conditions

The second Sakharov condition requires CP violation. Since the goal is to create an excess of matter, one might naively think that C violation is sufficient. But this is not the case since it can be counterbalanced by P violation.