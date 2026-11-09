# The two-point strain–direction pairing on unmodified Navier–Stokes expands to \( C_{\mathrm{CZ}} M(t)\,|\delta\xi|^2 \). The replacement by an \( M \)-independent \( -\gamma \) remains the regularity problem.

**Author:** Benjamin Stanley Frohman  
**Date:** 8 November 2026  

## Abstract

On unmodified 3D incompressible Navier–Stokes, after expansion of the geometric kernel via the Biot–Savart law and Calderón–Zygmund representation of the strain, the two-point pairing satisfies
\[
\delta\xi\cdot\bigl(S(x)\xi(x)-S(y)\xi(y)\bigr)=C_{\mathrm{CZ}}M(t)\,|\delta\xi|^2+R_{\mathrm{A}}+R_{\mathrm{B}}+R_{\mathrm{C}}.
\]
The leading factor is sharp on intermediate-axis alignment. Remainders (A)–(C) do not cancel it uniformly in \( M(t) \). The replacement of this factor by an \( M \)-independent \( -\gamma \) is equivalent to the regularity problem and is not performed here.

## 1. Standing objects

Let \( u \) be a classical solution of the 3D incompressible Navier–Stokes equations on \( \mathbb{R}^3 \) or \( \mathbb{T}^3 \),
\[
\partial_t u+(u\cdot\nabla)u=-\nabla p+\nu\Delta u,\qquad\nabla\cdot u=0,
\]
with vorticity \( \omega=\nabla\times u \). On \( \{\omega\neq 0\} \) write
\[
\xi=\frac{\omega}{|\omega|},\qquad M(t)=\|\omega(\cdot,t)\|_{L^\infty},\qquad S=\tfrac12\bigl(\nabla u+(\nabla u)^\top\bigr).
\]
The vorticity equation is unmodified:
\[
\partial_t\omega+(u\cdot\nabla)\omega=S\omega+\nu\Delta\omega.
\]
Fix two points \( x,y \) on a high set \( \{|\omega|\ge K\} \) and set \( \delta\xi=\xi(x)-\xi(y) \). The torus differs from \( \mathbb{R}^3 \) by a smooth periodic correction to the Biot–Savart kernel; that correction is absorbed into remainder (A) and does not change the singular structure.

## 2. Algebraic identity and kernel expansion

The two-point algebraic identity is
\[
S(x)\xi(x)-S(y)\xi(y)=S(x)\,\delta\xi+(S(x)-S(y))\xi(y),
\]
hence
\begin{equation}
\delta\xi\cdot\bigl(S(x)\xi(x)-S(y)\xi(y)\bigr)=S(x):\delta\xi\otimes\delta\xi+\delta\xi\cdot\bigl(S(x)-S(y)\bigr)\xi(y). \tag{\(\dagger\)}
\end{equation}
Because \( |\xi|=1 \), one has \( \delta\xi\perp(\xi(x)+\xi(y))/2 \), so \( \delta\xi \) is tangent to \( S^2 \) to first order.

Write \( K(r)\omega \) for the matrix kernel of the Calderón–Zygmund representation of \( S \), so \( S(x)=\mathrm{P.V.}(K*\omega)(x) \). Then both summands expand as principal-value integrals against the Biot–Savart kernel. The quadratic form \( S(x):\delta\xi\otimes\delta\xi \) is controlled by \( C_{\mathrm{CZ}}M(t)\,|\delta\xi|^2 \), and that size is attained for some orientations of \( \delta\xi \) relative to the eigenframe of \( S(x) \).

## 3. Named remainders (A)–(C) — closed

Fix a cutoff \( \rho>0 \) and split the integration in \( z \) into near (\( |z-x|\le\rho \) or \( |z-y|\le\rho \)) and far. Split \( \omega(z) \) into the high piece \( 1_{|\omega|\ge K}\omega \) and the low piece \( 1_{|\omega|<K}\omega \).

**(A) Far field.** On \( |z-x|\ge\rho \) and \( |z-y|\ge\rho \) the kernels \( K(x-z) \) and \( K(y-z) \) are smooth in \( (x,y) \). The difference \( K(x-z)-K(y-z) \) is \( O(|x-y|/|z-x|^4) \). After pairing with \( \delta\xi \) and using \( \|S\|_\infty\le C_{\mathrm{CZ}}M \),
\[
|R_{\mathrm{A}}|\le C_{\mathrm{CZ}}M(t)\,|\delta\xi|^2+C_\rho\,|\delta\xi|\,\|\omega\|_{L^1}.
\]
The \( L^1 \) term is controlled by the energy class and does not grow with \( M \). The first summand does.

**(B) Near-field kernel increment.** On the near set,
\[
\bigl|K(x-z)-K(y-z)\bigr|\le C\frac{|x-y|}{|z-x|^4}
\]
whenever \( |z-x|\gtrsim|x-y| \); the principal-value diagonal is handled as in the usual CZ theory. Pairing against \( \delta\xi\otimes\xi(y) \) and using \( |\omega(z)|\le M(t) \) produces
\[
|R_{\mathrm{B}}|\le C_{\mathrm{CZ}}M(t)\,|\delta\xi|^2+C|x-y|\bigl(|\nabla\xi(x)|+|\nabla\xi(y)|\bigr)M(t)\,|\delta\xi|.
\]
Young’s inequality moves the second piece onto \( \varepsilon(|\nabla\xi(x)|^2+|\nabla\xi(y)|^2) \) at the price of a further \( C_\varepsilon M(t)^2|x-y|^2|\delta\xi|^2 \) term, still dependent on \( M \).

**(C) Low-vorticity set.** Replacing \( |\omega(z)| \) by \( K \) on \( \{|\omega|<K\} \) gives an integral bounded by a constant built from \( K \), \( u_0 \), and \( \nu \) only. This remainder is independent of \( M(t) \).

Collecting (A)–(C) into \( (\dagger) \),
\begin{equation}
\delta\xi\cdot\bigl(S(x)\xi(x)-S(y)\xi(y)\bigr)=S(x):\delta\xi\otimes\delta\xi+R_{\mathrm{A}}+R_{\mathrm{B}}+R_{\mathrm{C}}, \tag{\(\ddagger\)}
\end{equation}
with
\[
|R_{\mathrm{A}}+R_{\mathrm{B}}|\le C_{\mathrm{CZ}}M(t)\,|\delta\xi|^2+\varepsilon\bigl(|\nabla\xi(x)|^2+|\nabla\xi(y)|^2\bigr)+C_\varepsilon M(t)^2|x-y|^2|\delta\xi|^2
\]
and \( R_{\mathrm{C}} \) independent of \( M \). The geometric factor \( D \) of Constantin has been used only inside the scalar stretching rate. It does not change the sign of \( S:\delta\xi\otimes\delta\xi \).

## 4. Intermediate-axis 1-jet — sharpness closed

Let \( \lambda_1\ge\lambda_2\ge\lambda_3 \) be the eigenvalues of \( S(x) \) with \( \lambda_1+\lambda_2+\lambda_3=0 \). Intermediate-axis alignment means \( \xi(x) \) is aligned with the intermediate eigenvector (corresponding to \( \lambda_2 \)). A first-order tilt of size \( \beta\ll 1 \) toward the principal stretching axis produces
\[
S(x):\delta\xi\otimes\delta\xi = \lambda_1 \beta^2 + O(\beta^4).
\]
Since \( \lambda_1 \sim M(t) \) on intermediate-axis configurations that are attained for smooth divergence-free fields, the leading coefficient is of size order \( M(t) \) and positive. Scaling the strain by \( M \) replaces the constant 1 by \( M \) and keeps the sign. This is a valid time-zero snapshot: every smooth divergence-free field is an unmodified Navier–Stokes initial datum.

## 5. Explicit non-claim — closed

This note does not prove global regularity of the 3D incompressible Navier–Stokes equations. It does not discharge the Constantin–Fefferman hypothesis (or Definition 7.1). It does not replace the coefficient \( C_{\mathrm{CZ}} M(t) \) by an \( M \)-independent \( -\gamma \). Rearrangement of the identities (\(\dagger\)) and (\(\ddagger\)) does not produce that replacement. The calculation stops at \( C_{\mathrm{CZ}} M(t) \).

The intermediate-axis 1-jet shows that the leading positive term of size order \( M \) is attained. Remainders (A)–(C) do not cancel it uniformly in \( M(t) \). Any further step that upgrades the coefficient requires a genuinely new idea outside the present expansion.
