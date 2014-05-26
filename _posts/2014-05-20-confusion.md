---
layout: post
title: Confusing definitions
description: "Confusing and misleading definitions"
modified: 2014-05-21
category: articles
tags: [definitions, explanation]
comments: true
share: true
---
**Definitions**

- [(Current/Charge/Current Source) Density](#currentchargecurrent-source-density)
- [Kernel Density](#kernel-density)


The pykCSD project requires good knowledge of linear algebra, calculus, statistics and (bio)electromagnetism. Trying to fully understand the Kernel Current Source Density method I found few misleading definitions more or less connected with the topic. I would like to keep them here for the future reference.

# (Current/Charge/Current Source) Density
Current Density[^1] $$\vec{J}$$ is the electric current $$\Delta I$$ (moving charge) per unit area S 

$$\vec{J} = \lim_{S \rightarrow 0} \frac{\Delta I(S) \widehat{a}_{max}}{S} \left[ \frac{A}{m^2}\right], \text{ where } \Delta I = \lim_{\Delta t \rightarrow 0}\frac{\Delta Q}{\Delta t}$$ 

which is a vector.

Charge Density is electric charge per unit volume (or area or line)

$$ \rho_q = \lim_{V \rightarrow 0} \frac{Q}{V} \left[ \frac{C}{m^3}\right]$$

which is a scalar.

Current Source Density[^3] is more like charge density.

$$C(r,t) = \sum_{n=1}^N I_n(t)\delta ^3(r-r_n) \left[\frac{A}{m^3} \right]$$

and

$$\phi(r,t) = \frac{1}{4\pi \sigma} \iiint_V \frac{C(r', t)}{\left| r-r' \rbrace} d^3 r'$$

# Kernel Density
ok2

[^1]: [Current density at wikipedia](http://en.wikipedia.org/wiki/Current_density)
[^3]: [Current source density](http://www.csc.kth.se/~helinden/PettersenLindenDaleEinevoll-BookChapter-revised.pdf)

<figure>
	<img src="{{ site.url }}/images/gsoc_horizontal.jpg" width="100%">
</figure>
