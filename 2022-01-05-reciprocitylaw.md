---
layout: article
tags: discussion
title: 互反律
mathjax: true
permalink: reciprocitylaw.html
author: Yufan Luo
key: reciprocitylaw
---
数论的核心目标之一就是解丢番图方程：

$$ f(X_{1},\cdot,X_{r})=0 $$

## Fermat Last Theorem: For $ n>2 $, the equation $ x^{n}+y^{n}=z^{n} $ has no non-zero integer solutions.
  
The case of $ n=3 $ was proved by Euler and the case of $ n=4 $ was proved by Euler. Since $ \textbf{FLT(d)}\implies \textbf{FLT(n)} $ whenever $ d|n $, our goal becomes
  
### If $\ell\geq 5 $ is a prime, then $ a^{\ell}+b^{\ell}=c^{\ell} $ has no nonzero integer solutions.

(Frey curve) Suppose that there's a solution  $ (a,b,c) $ to the Fermat's equation. Let us consider the Frey curve $ E=E_{a^{\ell},b^{\ell},c^{\ell}}: y^{2}=x(x-a^{\ell})(x+b^{\ell}) $，it's a elliptic curve over $ \mathbb{Q} $ satisfying  (1) it's semistable with conductor $ N=\prod_{p|abc}p$ （where $ p$ runs over primes),  (2) one can construct a Galois representation $  \bar{\rho}_{E,\ell}:G_{\mathbb{Q}}=Gal(\bar{\mathbb{Q}}/\mathbb{Q})\to \text{Aut}(E(\ell))\simeq GL_{2}(\mathbb{F}_{\ell})$.
  
