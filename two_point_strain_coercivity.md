# On Local Two-Point Strain Coercivity in the 3D Vorticity Equation

**Author:** Benjamin Stanley Frohman (ORCID: [0009-0006-7068-3718](https://orcid.org/0009-0006-7068-3718))  
**Affiliation:** Independent Researcher  
**Date:** September 25, 2026  
**MSC 2020:** 35Q30 (Primary), 76D03, 76D05 (Secondary)  
**Copyright:** Copyright (c) 2026 Benjamin Stanley Frohman  
**License:** Apache License, Version 2.0 (`Apache-2.0`)  
**Zenodo DOI:** [10.5281/zenodo.23627618](https://doi.org/10.5281/zenodo.23627618)

---

## Abstract

We analyze a natural local two-point strain-dissipation coercivity inequality for the three-dimensional incompressible Navier–Stokes vorticity equation on $\mathbb{T}^3$. First (**Theorem A**), we show that the conjectured local two-point coercivity bound $(\star)_\rho$ fails as a kinematic identity for general smooth divergence-free velocity fields on $\mathbb{T}^3$: by aligning the vorticity at $x$ with the intermediate strain eigenvector $e_2$ ($|\lambda_2|\ll \lambda_1$) and tilting the vorticity direction across $|x-y|\sim\rho$ toward the principal stretching eigenvector $e_1$, the local two-point dissipation $\mathcal{D}_\rho(x)$ is made arbitrarily small relative to the stretching $\mathcal{S}(x)$ while $\|\nabla\xi\|_{L^\infty}\lesssim \rho^{-1}$. Second (**Theorem B**), we audit the singular-integral closure via the Biot–Savart law and Calderón–Zygmund estimates when no *a priori* Lipschitz bound on the vorticity direction field $\xi=\omega/|\omega|$ is assumed; after absorbing the gradient of the direction field into the local two-point energy, the leading coefficient on the right-hand side is the positive constant $C_* = C_{\mathrm{CZ}} M$ rather than a negative damping constant $-\gamma$. Finally, we note that a global two-point coercivity bound without a short-range cutoff $|x-y|\le\rho$ fails even on exact stationary 2D Navier–Stokes shear flows.

---

## 1. Setting and the Candidate Coercivity Inequality

Let $u:\mathbb{T}^3\times[0,T)\to\mathbb{R}^3$ be a smooth solution of the three-dimensional incompressible Navier–Stokes equations with vorticity $\omega=\nabla\times u$ and symmetric rate-of-strain tensor $S=\tfrac12(\nabla u+(\nabla u)^T)$. Because $\operatorname{div}u=0$, the eigenvalues of $S(x)$ satisfy
$$\lambda_1(x)\ge \lambda_2(x)\ge \lambda_3(x),\qquad \lambda_1(x)+\lambda_2(x)+\lambda_3(x)=0.$$

At points where $|\omega(x)|>0$, write $\xi(x)=\omega(x)/|\omega(x)|\in\mathbb{S}^2$. The local vortex-stretching rate is
$$\mathcal{S}(x)=(S(x)\omega(x))\cdot\omega(x)=|\omega(x)|^2\,(S(x)\xi(x))\cdot\xi(x).$$

Given a cutoff scale $\rho>0$, consider the local two-point directional dissipation functional
$$\mathcal{D}_\rho(x)=|\omega(x)|^2\int_{|x-y|\le\rho}\frac{|\xi(x)-\xi(y)|^2}{|x-y|^3}\,dy$$
(or its vorticity-weighted counterpart replacing $|\omega(x)|^2$ by $|\omega(x)|\,|\omega(y)|$). A natural candidate mechanism to close the critical vorticity-stretching term without an *a priori* Constantin–Fefferman direction-Lipschitz hypothesis is the local two-point strain coercivity conjecture:

> **Candidate Inequality $(\star)_\rho$.** *There exist universal constants $\gamma>0$, $C_0\ge 0$, and $\rho>0$ such that for every smooth divergence-free field $u$ on $\mathbb{T}^3$ and every $x\in\mathbb{T}^3$,*
> $$\mathcal{S}(x)-\nu\,\mathcal{D}_\rho(x)\;\le\;-\gamma\,\mathcal{D}_\rho(x)+C_0\,|\omega(x)|^2.$$

---

## 2. Theorem A: Kinematic Failure of $(\star)_\rho$ via Intermediate-Axis Tilt

**Theorem A.** *For any $\rho>0$, $\nu>0$, and $\gamma>0$, the inequality $(\star)_\rho$ fails across the class of smooth divergence-free velocity fields on $\mathbb{T}^3$. Specifically, for any prescribed strain amplitude $\Lambda\gg 1$ and small parameter $\delta\in(0,1)$, there exist smooth divergence-free fields $u$ on $\mathbb{T}^3$ and points $x_0\in\mathbb{T}^3$ at which:*
1. *The strain eigenvalues at $x_0$ satisfy $\lambda_1(x_0)=\Lambda$, $\lambda_2(x_0)=\delta\Lambda>0$, and $\lambda_3(x_0)=-(1+\delta)\Lambda$.*
2. *The vorticity direction at $x_0$ aligns with the intermediate eigenvector $e_2$, so that*
   $$\mathcal{S}(x_0)=\delta\Lambda\,|\omega(x_0)|^2>0.$$
3. *Across the ball $|x-x_0|\le\rho$, $\xi(x)$ tilts smoothly toward $e_1$ by an angle $\theta(x)=\varepsilon\,|x-x_0|/\rho$ with $\varepsilon\ll\delta^{1/2}$, so that $\|\nabla\xi\|_{L^\infty(B_\rho(x_0))}\lesssim \varepsilon/\rho$ and*
   $$\mathcal{D}_\rho(x_0)\;\lesssim\;\varepsilon^2\,|\omega(x_0)|^2.$$

*Consequently, choosing $\varepsilon^2\ll \delta\Lambda/(\nu+\gamma)$ and $\delta\Lambda\gg C_0$ yields $\mathcal{S}(x_0)-(\nu-\gamma)\mathcal{D}_\rho(x_0) > C_0|\omega(x_0)|^2$, violating $(\star)_\rho$.*

*Proof sketch.* By local realization of divergence-free velocity fields with prescribed curl and traceless symmetric gradient at $x_0$ (via a localized vector potential $u=\nabla\times(\chi\psi)$ on $\mathbb{T}^3$), the strain matrix $S(x_0)=\operatorname{diag}(\Lambda,\delta\Lambda,-(1+\delta)\Lambda)$ and the first jet of $\omega$ near $x_0$ are independent subject only to $\operatorname{div}\omega=0$. Setting $\omega(x)=|\omega_0|\bigl(\sin(\varepsilon x_3/\rho)\,e_1+\cos(\varepsilon x_3/\rho)\,e_2\bigr)$ on $B_\rho(x_0)$ satisfies $\partial_1\omega_1+\partial_2\omega_2+\partial_3\omega_3=0$ identically because $\omega$ depends only on $x_3$ and has no $e_3$-component. At $x_0=0$, $\xi(0)=e_2$ gives $(S(0)\xi(0))\cdot\xi(0)=\delta\Lambda$, whereas $|\xi(x)-\xi(0)|\le \varepsilon|x_3|/\rho$ gives $\int_{|y|\le\rho}|y|^{-3}|\xi(y)-\xi(0)|^2\,dy\le \frac{4\pi}{3}\varepsilon^2$. Taking $\Lambda\to\infty$ at fixed $\delta,\varepsilon$ violates $(\star)_\rho$. $\square$

---

## 3. Theorem B: Audit of the Biot–Savart / Calderón–Zygmund Closure

Suppose one expresses $S(x)$ via the singular integral representation (Constantin–Fefferman 1993)
$$S(x)=\operatorname{p.v.}\int_{\mathbb{T}^3}\widehat{K}(x-y)\,|\omega(y)|\,dy + R(x),$$
where $\widehat{K}(z)$ is homogeneous of degree $-3$ with mean zero on spheres, and splits the integral into $|x-y|\le\rho$ and $|x-y|>\rho$.

**Theorem B.** *Let $M=\sup_{|x-y|\le\rho}|\omega(y)|$ and write the inner stretching contribution as*
$$\mathcal{S}_{\mathrm{in}}(x)=|\omega(x)|^2\operatorname{p.v.}\int_{|x-y|\le\rho}K_{ij}(x-y)\,\xi_i(x)\xi_j(x)\,\omega(y)\cdot(\xi(y)-\xi(x))\,dy$$
*(using the geometric cancellation $\widehat{K}(z)\xi(x)\cdot\xi(x)=0$ when $\xi(y)=\xi(x)$). Under Cauchy–Schwarz and Calderón–Zygmund estimation without an a priori Lipschitz bound on $\xi$, absorbing the directional difference into $\mathcal{D}_\rho(x)$ yields*
$$\mathcal{S}_{\mathrm{in}}(x)-\nu\,\mathcal{D}_\rho(x)\;\le\;\bigl(C_{\mathrm{CZ}}\,M-\nu\bigr)\,\mathcal{D}_\rho(x)+C(\rho,\nu)\,\|\omega\|_{L^2}^2\,|\omega(x)|^2.$$
*In particular, when $M=O(1)$ is normalized and $\nu\ll C_{\mathrm{CZ}}M$, the coefficient multiplying $\mathcal{D}_\rho(x)$ on the right-hand side is the positive quantity $C_* = C_{\mathrm{CZ}}M > 0$, not a negative damping constant $-\gamma<0$.*

---

## 4. Failure of Uncutoff Global Two-Point Coercivity on Exact 2D Flows

If the short-range cutoff $|x-y|\le\rho$ is omitted and one integrates over all of $\mathbb{T}^3$, even stationary two-dimensional Kolmogorov shear flows $u(x_1,x_2)=(\sin x_2,0,0)$ with vorticity $\omega=(0,0,-\cos x_2)$ exhibit $\xi(x)=\operatorname{sgn}(-\cos x_2)\,e_3$, which jumps by $2e_3$ across the nodal planes $\cos x_2=0$ while the vortex stretching $(S\omega)\cdot\omega\equiv 0$ vanishes identically. This confirms that any relation between stretching and directional two-point integrals is inherently three-dimensional and scale-localized.

---

## References

1. P. Constantin and C. Fefferman, *Direction of vorticity and the problem of global regularity for the Navier–Stokes equations*, Indiana Univ. Math. J. **42** (1993), 775–789.
2. J. T. Beale, T. Kato, and A. Majda, *Remarks on the breakdown of smooth solutions for the 3-D Euler equations*, Comm. Math. Phys. **94** (1984), 61–66.
3. P. Constantin, *Geometric statistics in turbulence*, SIAM Rev. **36** (1994), 73–98.
