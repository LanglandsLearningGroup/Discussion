---
layout: article
tags: discussion
title: Unramified Fontaine-Mazur Conjecture
mathjax: true
permalink: UnramifiedFM.html
key: UnramifiedFM
---

<p> Let $ p $ be a rational prime. Let $ \overline{\mathbb{Q}_{p}} $ be an algebraic closure of $ \mathbb{Q}_{p} $. The Unramfieid Fontaine-Mazur Conjecture states that </p>
  
### Unramified Fontaine-Mazur Conjecture
Let $ K $ be a number field and $ S $ a finite set of primes of $ K $ not containing any primes above $ p $. Let $  G_{K,S} $ be the Galois group of the maximal extension of $ K $ unramified outside $ S $. Then any continuous homomorphism $ \rho:G_{K,S}\to GL_{n}(\overline{\mathbb{Q}_{p}}) $ has a finite image.</p>
  
We can give a reformulation of Conjecture in terms of pro-$ p $ groups.
  
### Unramified Fontaine-Mazur Conjecture using pro-$ p $ groups
Let $ K $ be a number field.  Let $ K_{S}(p) $ denote the maximal $ p $-extension of $K $ in $ \overline{ \mathbb{Q}} $ which is unramified outside $ S $ (i.e. it is the compositum of all finite $ p $-power degree extensions of $ K $ unramified outside $ S $.) Put $ G_{K,S}(p)=\text{Gal}(K_{S}(p)/K) $. Then any continuous homomorphism $ \rho:G_{K,S}(p)\to GL_{n}(\overline{ \mathbb{Q}_{p}}) $ has finite image.

困难之处：
尽管我现在无法全部证明之，但是二维表示的情形是可以靠近的，我已经能证明如果rho（Frob_p）的两个特征值不同，那么它是对的；所以只需要考虑特征值相同的情形。然后我能证明，你可以假设rho的像包含一个开子集使得这个开子集的元素全是特征值不同的矩阵；你可以假设这个表示是不可约的；显然就差一个技巧转换一下就出来了；问题，它是什么？
