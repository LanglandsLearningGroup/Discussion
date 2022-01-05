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

    - (Frey curve) Suppose that there's a solution  $ (a,b,c) $ to the Fermat's equation. Let us consider the Frey curve $ E=E_{a^{\ell},b^{\ell},c^{\ell}}: y^{2}=x(x-a^{\ell})(x+b^{\ell}) $，it's a elliptic curve over $ \mathbb{Q} $ satisfying  (1) it's semistable with conductor $ N=\prod_{p|abc}p$ （where $ p$ runs over primes),  (2) one can construct a Galois representation $  \bar{\rho}_{E,\ell}:G_{\mathbb{Q}}=Gal(\bar{\mathbb{Q}}/\mathbb{Q})\to \text{Aut}(E(\ell))\simeq GL_{2}(\mathbb{F}_{\ell})$.
    - (Shimura-Taniyama-Weil conjecture: Every elliptic curve over $ \mathbb{Q}$ is modular.)  For any elliptic curve $ E$ over rational number field, there exists a weight two cuspidal modular eigenform $ f_{E}(q)=\sum_{n\geq 1}a_{n}q^{n}$ such that $ a_{p}=p+1-|E(\mathbb{F}_{p})|$ for any prime $ p$. Now, appying Shimura-Taniyama-Weil conjecture to the Frey curve $ E$ in Step 1, we see that there is a modular form $ f$ such that $ \bar{\rho}_{f}=\bar{\rho}_{E,\ell}$, where $ \bar{\rho}_{f}:Gal(\bar{\mathbb{Q}}/\mathbb{Q})\to GL_{2}(\mathbb{F}_{\ell})$ is the associated Galois representation corresponding to $ f$.
    - (Serre + Ribet's work: lowering the level) The Shimura-Taniyama-Weil conjecture predicts that the representation $ \bar{\rho}_{E,\ell}$ arises from a modular form of weight two, albeit a form whose level is quite large. (it's the product of all the primes dividing $ abc $ by Step 1). Ribet proved, if this were the case, then $ \bar{\rho}_{E,\ell}$ would also be associated with a modularform mod $ \ell$ of weight $ 2$ and level $ 2$, in the way predicted by Serre's conjecture. That is, there  is a weight two new form $ g$ of conductor $ 2$ such that $ \bar{\rho}_{g}=\bar{\rho}_{E,\ell}$. But the dimension of $ S_{2}(\Gamma_{0}(2)) $ is eual to the genus of $ X_{0}(2) $, which is easily to be zero. This is a contradiction and Fermat's Last Theorem is proved. 
  
