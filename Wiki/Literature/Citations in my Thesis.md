
# Gradient Flow
### Stoffer et al. 2026
[link](https://arxiv.org/abs/2601.18883) ***One-loop matching of the LEFT to the QCD gradient flow***
- They calculate the NLO SFTX of the baryon- and lepton-number conserving LEFT using only flowed QCD (other fields are not flowed) and the HV scheme.
- Their basis includes evanescent operators relevant for the CEDM (and more)
- Note: Since $\sigma_{\mu\nu}=[\gamma_\mu,\gamma_\nu]$ and $\gamma_\mu=\bar{\gamma}_\mu+\hat{\gamma}_\mu$ , with the bar being the 4-dimensional and the hat being the $-2\epsilon$-dimensional part (which commute), we get 
$$
\{\sigma_{\mu\nu},\gamma_5\} = 
\{\bar{\sigma}_{\mu\nu},\gamma_5\}
+\{\hat{\sigma}_{\mu\nu},\gamma_5\}
= 2 \bar{\sigma}_{\mu\nu}\gamma_5\ + 2\bar{\sigma}_{\mu\nu}\gamma_5\
$$
	- Since $\gamma_5$ commutes with the first sigma (because it has two dim-4 gammas) and also with the second since $\gamma_5$ commutes with all $-2\epsilon$-dim objects

### Zwanziger, Baulieu 1981; Parisi, Wu 1981
[Zwanziger & Baulieu](https://lib-extopc.kek.jp/preprints/PDF/1981/8108/8108081.pdf), [Parisi & Wu](https://inspirehep.net/literature/9589)
They introduce a GF flow equation with gauge fixing term (also called the Zwanziger term) in the context of stochastik quantization. Physical expectation values of operators result here in the limit $t\rightarrow\infty$.

### Lüscher 2010
[link](https://arxiv.org/abs/0907.5491) ***Trivializing maps, the Wilson flow and the HMC algorithm***
Lüscher introduces the GF for trivializing maps which map fields to their strong-coupling limit. The idea was to improve the lattice algorithms.

### Lüscher, Weisz 2011
[link](https://arxiv.org/abs/1101.0963) ***Perturbative analysis of the gradient flow in non-abelian gauge theories***
Introduce the GF as known now (in analogy to the Langevin equation) for gluons. Show that flowed fields and correlation functions do not require further renormalization.

### Lüscher 2013
[link](https://arxiv.org/abs/1302.5246) ***Chiral symmetry and the Yang-Mills gradient flow***
Apply flow to fermions, calculate their flowed field renormalization through NLO.

### Lüscher 2014
[link](https://doi.org/10.1007/JHEP08(2010)071) ***Properties and uses of the Wilson flow in lattice QCD***
Calculation of the flowed gluon action density and using this for strong coupling calculations on the lattice.