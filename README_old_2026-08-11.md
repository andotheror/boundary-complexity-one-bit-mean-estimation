# The Boundary Complexity of One-Bit Mean Estimation

## Abstract

One bit can encode an arbitrary measurable subset of the sample space, so communication alone does not describe the complexity of a binary quantizer. We study the missing geometric resource. Each of $n$ Gaussian samples has mean $\theta\in[-L,L]$ and known variance $\sigma^2$. Before seeing data, a one-shot protocol fixes a binary query whose one-set is a union of at most $q$ intervals. We prove the exact sample complexity 

$$n_q^\star(\varepsilon,\delta) \asymp \log\\\\\\!\left(1+\frac{L}{\sigma}\right) + \left(1\vee\frac{L}{q\sigma}\right) \frac{\sigma^2}{\varepsilon^2}\log\frac1\delta.$$

 The lower bound follows from a boundary-information inequality. A $q$-component bit has only $O(q/\sigma)$ Fisher information after integration over the unknown mean. A continuous hard-center prior and product Hellinger affinity turn this global budget into the high-confidence factor $L/(q\sigma)$. The argument also yields a conservation law for heterogeneous queries: achieving error $\delta$ requires total effective boundary mass at least $\Omega((\sigma^2/\varepsilon^2)\log(1/\delta))$. For the upper bound, every query draws a shifted grid and an independent threshold inside each of $q$ cells. The union of the threshold suffixes is one bit with at most $q$ components. Its Gaussian response functions form a random feature map whose squared metric is 

$$\Theta\\\\\\!\left(\min\left\\\\\\{\frac{|\theta-\theta'|^2}{h\sigma}, \frac{|\theta-\theta'|}{h},1\right\\\\\\}\right), \qquad h\asymp \sigma\vee\frac{L}{q}.$$

 A two-resolution least-squares decoder and one-dimensional peeling attain the lower bound without interaction or an extra resolution logarithm. Thus disconnected boundaries interpolate sharply between ordinary thresholds and unrestricted oscillatory one-bit queries.

## Contributions

- We determine the minimax one-shot sample complexity for every component budget $q$, including the localization and high-confidence terms.
- We prove an integrated boundary-information inequality and a heterogeneous boundary conservation law.
- We construct a finite $q$-component random-grid query family with an exact three-regime response metric.
- We give a fully noninteractive two-resolution decoder whose analysis avoids an extra $\log(L/\varepsilon)$ factor.

## Keywords

one-bit estimation, quantization, mean estimation, sample complexity, Fisher information, boundary complexity, distributed estimation, minimax rates

## Files

- `main.pdf`
- `main.tex`
- `references.bib`
- `iclr2027_conference.sty`, `iclr2027_conference.bst`, `natbib.sty`, `fancyhdr.sty`
- `main.pdf.ots`, `README.md.ots` OpenTimestamps priority proofs
