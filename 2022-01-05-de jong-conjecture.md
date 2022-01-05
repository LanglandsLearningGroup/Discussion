---
layout: article
tags: discussion
title: de Jong conjecture
mathjax: true
permalink: dejongconj.html
author: Yufan Luo
key: dejongconj
---

## A conjecture of A.J. de jong
<p> Let $ X $ be an integral scheme, separated and of finite type over a finite field $ k $ of characteristic $ p $. Let $ \ell $ be a prime number different from $ p $. Assume that $ X $ is a normal scheme. Let $ \bar{\rho}:\pi_{1}(X)\to GL_{n}(\mathbb{F}_{\ell}) $ be a continuous, absolutely irreducible representation of the arithmetic \'etale fundamental group of $ X $. Let $ \mathcal{O} $ be the ring of integers of a finite extension of the fraction field of $ \mathbb{Z}_{\ell} $ inside $ \overline{\mathbb{Q}_{\ell}} $. Fix a lift $ \eta:\pi_{1}(X)\to \mathcal{O}^{\times} $ of finite order of the $ 1 $-dimensional representation $ \text{det}(\bar{\rho}) $. Then we get a deformation ring $ R_{X}^{\eta} $ for deformations of $ \bar{\rho} $ of determinant $ \eta $ and defined on $ \pi_{1}(X) $.</p>
  
<p>  In the situation above, assume 
  <ol>
  <li>the restriction $ \bar{\rho}|_{\pi_{1}(\overline{X})} $ is absolutely irreducible, and </li>
  <li>$ \ell $ does not divide $ n $.</li>
</ol>
<p> Then $ R_{X}^{\eta} $ is finite flat over $ \mathbb{Z}_{\ell} $ and it is a complete intersection ring. In particular, $ \bar{\rho} $ can be lifted to an $ \ell $-adic representation $ \rho:\pi_{1}(X)\to GL_{n}(\mathcal{O}) $.</p>

## A question

<p> Let $ X $ be a scheme over $ \mathbb{F}_{p} $. Let $ \ell $ be a prime which is not equal to $ p $. Let $ \rho:\pi_{1}(X)\to GL_{d}(\overline{\mathbb{F}_{\ell}}) $ be a representation of the arithmetic \'etale fundamental group of $ X $. We consider 'the characteristic polynomials map':
  
$$ P_{\rho}:\pi_{1}(X)\to \overline{\mathbb{F}_{\ell}}[X],~~g\mapsto P_{g}:=\text{characteristic polynomail of $ \rho(g) $}. $$
  
<p> There exists an integer $ k $ such that all $ P_{g} $ split over $ \mathbb{F}_{\ell^{k}} $. For any $ g\in G $, if $ P_{g}=\prod_{i=1}^{d}(X-\alpha_{i}) $ for some $ \alpha_{i}\in \mathbb{F}_{\ell^{d}} $, then we define
  
 $$ \tilde{P}_{g}:=\prod_{i=1}^{d}(X-\tau(\alpha_{i}))\in W(\mathbb{F}_{\ell^{k}})[X] $$
  
<p> where $ \tau: \mathbb{F}_{\ell^{d}}\to W(\mathbb{F}_{\ell^{d}}) $ is the Teichmuller representation. Fix an isomorphism of the algebraic closure of $\mathbb{Q}  $ within $ \overline{\mathbb{Q}_{\ell}} $ and $ \overline{\mathbb{Q}_{p}} $. We may regard $ \tilde{P}_{g} $ as an element in $ \overline{\mathbb{Z}_{p}}[X] $. Then we define
  
$$ Q_{g}:=\text{the image of $ \tilde{P}_{g} $ in $ (\overline{\mathbb{Z}_{p}}/p\overline{\mathbb{Z}_{p}})[X] $} $$</p>
### Question: 

Is there a representation $ \rho':\pi_{1}(X)\to GL_{d}(\overline{\mathbb{F}_{p}}) $ such that, for any $ g\in \pi_{1}(X) $, the characteristic polynomial of $ \rho'(g) $ is $ Q_{g} $?

