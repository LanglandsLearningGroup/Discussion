# Discussion
或许可以在这里提出各种数学问题，可惜不支持 Latex.

## 素数和扭结
<!-- wp:paragraph -->
<p>1 Mazur’s knotty dictionary <a href="http://www.neverendingbooks.org/mazurs-dictionary">http://www.neverendingbooks.org/mazurs-dictionary</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>2 What is the knot associated to a prime? <a href="http://www.neverendingbooks.org/what-is-the-knot-associated-to-a-prime">http://www.neverendingbooks.org/what-is-the-knot-associated-to-a-prime</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>3 Who dreamed up the primes=knots analogy? <a href="http://www.neverendingbooks.org/who-dreamed-up-the-primesknots-analogy">http://www.neverendingbooks.org/who-dreamed-up-the-primesknots-analogy</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>4 the birthday of the primes=knots analogy <a href="http://www.neverendingbooks.org/the-birthday-of-the-primesknots-analogy">http://www.neverendingbooks.org/the-birthday-of-the-primesknots-analogy</a></p>
<!-- /wp:paragraph -->

## 局部类域论的证明
1 历史上，局部类域论首先是从整体类域论推出的，可以参考 Hasse 30年代初的论文（德语）。很重要的是，在上同调证明成为教科书里的标准证明前，几乎每本书的证明都不太一样，所以我的总结是基于基本思路的。
2 历史上第一个独立的证明是基于 central simple algebras 和 Brauer group of a local field。可以参考Schmidt，Hasse，Chevalley 30年代初各自的论文（多为德语）。
3 上同调证明出现在五六十年代，现在的标准证明之一。关于这个证明，请参考https://bookstore.ams.org/mmono-240，他们的证明简化了原始证明，但是非常非常简略。
4 Lubin-Tate theory, 现在的标准证明之二。3 和 4 如此不同，就我所知，至今没有人能解释这两者的联系。我的直觉是，这两者发生在不同的topoi之中。
5 Hazewinkel's proof: https://www.sciencedirect.com/science/article/pii/0001870875901565 被埋没的证明，Iwasawa为此写过一本小册子，有中文版，冯克勤译，暂无英文版。Iwasawa也写过一个关于Lubin-Tate的小册子，和上一本同名，也叫"局部类域论"，有英文版。
6（只能证明char p情形）Using Artin–Schreier–Witt theory to prove the char p case Yukiyosi Kawada and Ichiro Satake, Class formations. II, J. Fac. Sci. Univ. Tokyo Sect. IA Math.  (1956), 353–389. 只有Fesenko记得的证明，虽然只能证明char p情形，但很简单。参考https://doi.org/10.1007/s40879-018-0245-x
7 local Tate duality: 一般是从local CFT推出local Tate duality，但是后者可以被独立证明，所以可以反过来。参考 Herr, L. Une approche nouvelle de la dualité locale de Tate. Math Ann 320, 307–337 (2001). https://doi.org/10.1007/PL00004476 这个证明可以算作Galois representations over local fields的应用。
8 Neukirch's mechanism  Neukirch, J. Neubegründung der Klassenkörpertheorie. Math Z 186, 557–574 (1984). https://doi.org/10.1007/BF01162780  https://doi.org/10.1007/978-3-642-82465-4  https://doi.org/10.1007/978-3-540-37663-7  Neukirch, J. Micro primes. Math. Ann. 298, 629–666 (1994). https://doi.org/10.1007/BF01459755 Neukirch最后一篇论文，还没来得及发展自己的理论就去世了。现在除了Fesenko也几乎没人在乎了。
9 Fargues' geometrization program https://arxiv.org/abs/1705.01526
10 Using isocrystals: 参考R. Crew https://arxiv.org/abs/1710.05707 这个证明显然和 2 有很多联系。Crew基于这篇文章还写过lecture notes， 可以参考https://people.clas.ufl.edu/rcrew/files/LCFT.pdf
11 K-theoretic and higher categorical approach: D. Clausen https://arxiv.org/abs/1703.07842
12 Fesenko作为这个领域为数不多的专家，写过一篇总结https://www.maths.nottingham.ac.uk/plp/pmzibf/232.pdf

## 为什么 Langlands 只关心曲线而不关心高维簇？
comment on why is it that we only consider curves and not higher dimensional varieties. The point is that while function fields of curves are very similar to number fields, the fields of functions on higher dimensional varieties have a very different structure. For example, if X is a smooth surface, then the completions of the field of rational functions on X are labeled by pairs: a point x of X and a germ of a curve passing through x. The corresponding complete field is isomorphic to the field of formal power series in two variables. At the moment no one knows how to formulate an analogue of the Langlands correspondence for the field of functions on an algebraic variety of dimension greater than one, and finding such a formulation is a very important open problem. There is an analogue of the abelian class field theory , i.e. higher class field theory, but not much is known beyond that.

甚至几乎没有人猜想高维non-abelian Artin map长什么样，以及高维non-abelian existence theorem如何陈述。
这两种方法会相互促进的。表示论显然不能解决所有问题，比如Shafarevich conjecture，即使global Langlands被完全证明了，我们也很难直接了解if commutator subgroup of the absolute Galois group of Q is free，而我们如果能证明global non-abelian Artin map is isomorphism，这个问题会简化很多。

## 啥不能弄到 $GL_3$?
看到之前说的为什么不搞到GL_3。我觉得可以补充一点，当然我不确定这是主要困难）在Galois那边有一个困难的地方，就是难以显式地找出(potentially) semistable/crystalline lift to char 0. 因为local-global compatibility, 来自automorphic representation的Galois representation 会有一定的p-adic Hodge thy 的要求。然后这个要求很难显式地从F_p提升到Q_p, 因为难以计算的H^1 obstruction(在très ramifieé case) 我之前想做这个 我导师表示最好不要做，这个基本不可能做.可以参考这个 这是可能Galois方面的满足一定p-adic Hodge条件的lifting里面最强的结果了。 https://youtu.be/18CxluFd69A   https://mathoverflow.net/questions/74472/what-makes-langlands-for-n-2-easier-than-langlands-for-n2   https://mathoverflow.net/questions/43377/automorphic-forms-on-gl3   可以到 $GL_3$! https://www.galoisrepresentations.com/2017/06/23/new-results-in-modularity-part-i/

## $R\simeq T$?
有个很重要的事实 就是 Hecke 代数可以写成一些eigensystem的积，那么局部化了之后就是eigensystem over \bar \rho 很自然地，根据泛性质就存在了一个映射R—>T;然后 容易严重它的满的 所以本质上TW方法就是证明它也是单的;patching 干了什么呢？它提供了一个东西，T在上面有个自然的作用。我们让R通过满射R—>T也作用在上面。Patching argument告诉我们R的作用是自由的 从而得到R——>T也是单的;关键就是那个东西怎么构造呢？其实用到了Hida thy的想法。先提升level, 再去不动点或者余不动点回归level。具体是写成一堆东西的极限。这个Toby Gee在AWS 2013他的最后两讲很形象地画了不少图 .



