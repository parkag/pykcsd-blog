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
**Current Density** [^1] $$\vec{J}$$ is the electric current $$\Delta I$$ (moving charge) per unit area S 

$$\vec{J} = \lim_{S \rightarrow 0} \frac{\Delta I(S) \widehat{a}_{max}}{S} \left[ \frac{A}{m^2}\right], \text{ where } \Delta I = \lim_{\Delta t \rightarrow 0}\frac{\Delta Q}{\Delta t}$$ 

which is a vector.

**Charge Density** is electric charge per unit volume (or area or line)

$$ \rho_q = \lim_{V \rightarrow 0} \frac{Q}{V} \left[ \frac{C}{m^3}\right]$$

which is a scalar.

**Current Source Density** [^3] has the meaning of volume density of current entering or leaving the medium at some point in space.

 $$C(r,t) = \sum_{n=1}^N I_n(t)\delta ^3(r-r_n) \left[\frac{A}{m^3} \right]$$

and

 $$ \phi(r, t) = \frac{1}{4 \pi \sigma} \iiint \frac{ C(r', t) }{  \lvert r-r' \rvert } d^3 r' $$

# Kernel Density
Despite its name, this is not directly related to the kCSD method.

* http://www.mathworks.com/help/stats/kernel-distribution.html
* http://homepages.inf.ed.ac.uk/rbf/CVonline/LOCAL_COPIES/AV0405/MISHRA/kde.html
* http://scikit-learn.org/stable/modules/density.html
* http://en.wikipedia.org/wiki/Kernel_density_estimation


[^1]: [Current density at wikipedia](http://en.wikipedia.org/wiki/Current_density)
[^3]: [Current source density](http://www.csc.kth.se/~helinden/PettersenLindenDaleEinevoll-BookChapter-revised.pdf)

<figure>
	<img src="{{ site.url }}/images/gsoc_horizontal.jpg" width="100%">
</figure>
