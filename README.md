# Discussion
或许可以在这里提出各种数学问题，可惜不支持 Latex.

## 素数和扭结 Primes and Knots

- [Mazur’s knotty dictionary](http://www.neverendingbooks.org/mazurs-dictionary)
- [What is the knot associated to a prime?](http://www.neverendingbooks.org/what-is-the-knot-associated-to-a-prime)
- [Who dreamed up the primes=knots analogy?](http://www.neverendingbooks.org/who-dreamed-up-the-primesknots-analogy)
- [the birthday of the primes=knots analogy](http://www.neverendingbooks.org/the-birthday-of-the-primesknots-analogy)

## 局部类域论的证明概览 Approaches to Local Class Field Theory
by [Yiqi Xu](https://github.com/YiqiXu)

与整体类域论（GCFT）相似，也存在许多局部类域论（LCFT）的证明。上同调证明在上世纪50年代出现后逐渐固化为教科书里的标准证明，这一过程一直持续到21世纪初。在此期间，几乎每本介绍局部类域论的书给出的证明都不完全一致，所以笔者的总结是基于基本思路和方法的。尽管笔者尽了最大努力，限于眼界和知识有限，以下总结可能仍然不完整，欢迎补充和评论。以下列表主要依据主要文献的出版（或公开）时间排序。  

0. 历史上，LCFT 首先是从 GCFT 推出的，可以参考 Hasse 30年代初的论文（德语），链接稍后补充。
1. ***Central Simple Algebras*** 历史上第一个独立的证明是基于 central simple algebras 和 Brauer group of a local field。可以参考Schmidt，Hasse，Chevalley 30年代初各自的论文（德语或法语），链接稍后补充。
    - [Number Theory 2: Introduction to Class Field Theory](https://bookstore.ams.org/mmono-240) 第8章给出该方法一个较现代的介绍。他们的证明简化了原始证明，但是非常非常简略。
2. ***Galois Cohomology*** 上同调证明出现在五六十年代，现在的教科书证明之一。参考大多类域论的教科书，不赘述。
3. ***Lubin-Tate Theory*** 现在的教科书证明之二。参考大多类域论的教科书，不赘述。方法 2. 和 3. 如此不同，就我所知，至今没有人能解释这两者的联系。Iwasawa 写过一个关于 Lubin-Tate 的日语小册子，英译版为 [Local Class Field Theory](https://books.google.de/books/about/Local_Class_Field_Theory.html?id=iJ7vAAAAMAAJ&redir_esc=y).
4. ***Kawada-Satake Method*** 主要思路基于Artin-Witt-Schreier theory. 
    > Yukiyosi Kawada and Ichiro Satake, Class formations. II, J. Fac. Sci. Univ. Tokyo Sect. IA Math.  (1956), 353–389.  

    该证明只有 Fesenko 还不时强调其重要性，虽然只能证明 char p 情形，但很简单。由于难以获得原始论文，现代文献请参考 [Generalised Kawada-Satake method for Mackey functors in class field theory](https://doi.org/10.1007/s40879-018-0245-x).
5. ***Hazewinkel-Serre Method*** Hazewinkel在他的博士论文给出了新的证明，先证明the case of ramified abelian extesnions，再扩展到一般情况。正式发表为 [Local class field theory is easy](https://doi.org/10.1016/0001-8708(75)90156-5). Iwasawa 也为此写过一本日语小册子，中文版《局部类域论》冯克勤译，暂无英文版。
6. ***Neukirch Mechanism*** Neukirch 为类域论的公理化做过许多工作，此过程中他也给出了新证明，他的方法可以理解为先the case of unramified abelian extesnions，再扩展到一般情况。所以 Fesenko 认为 Neukirch‘s mechanism 应该和 Hazewinkel-Serre method 结合起来，事实也确实如此，两者构造的 “Artin map” 互逆，进一步简化了证明。Fesenko 一直在强调 Neukirch mechanism 的重要性，笔者同意他的观点，无奈近二十年的发展几乎为零。Neukirch 的工作同时阐明了一点，上同调不是类域论的核心。他在这方面的工作主要集中在下列文献中：
    - [Neubegründung der Klassenkörpertheorie](https://doi.org/10.1007/BF01162780)（德语）
    - [Class Field Theory](https://doi.org/10.1007/978-3-642-82465-4) 
    - [Algebraische Zahlentheorie](https://doi.org/10.1007/978-3-540-37663-7)（德语）
    - [Micro primes](https://doi.org/10.1007/BF01459755) 这是 Neukirch 去世前最后一篇论文。
7. ***Local Tate Duality*** 一般 local Tate duality 由 LCFT 推出，但是后者可以被独立证明，所以可以反过来。参考 [Une approche nouvelle de la dualité locale de Tate](https://doi.org/10.1007/PL00004476)（法语）. 这个证明可以算作Galois representations over local fields的应用。
8. ***Fargues' Geometrization Program*** Fargues 从他的几何化猜想出发给出了新证明，可参考[Simple connexité des fibres d'une application d'Abel-Jacobi et corps de classe local](https://doi.org/10.24033/asens.2418)（法语）. Fargues 认为他的证明优于其他所有证明，笔者持保留态度。
9. ***Isocrystals*** Crew 利用 isocrystal 的性质给出了一个新证明，请参考 [Weil groups and F-isocrystals](https://arxiv.org/abs/1710.05707). 该证明和证明 2. 大同小异。Crew 基于这篇文章还写过讲义 [Local Class Field Theory](https://people.clas.ufl.edu/rcrew/files/LCFT.pdf).
10. ***K-theory*** [A K-theoretic approach to Artin maps](https://arxiv.org/abs/1703.07842).

Fesenko 作为这个领域为数不多的专家，写过一篇概览 [Class Field Theory, its three main generalisations, and applications](https://doi.org/10.4171/EMSS/45), 可作为补充。

我们自然有以下问题：
- 是否有一个框架可以统一以上所有方法？
- 是否可以推广到整体域？（对于大多数答案是肯定的）
- 是否可以推广到高维？
- 是否可以推广到 non-abelian 情形？

甚至几乎没有人猜想高维 non-abelian Artin map 长什么样，以及高维 non-abelian existence theorem 如何陈述。
这两种方法会相互促进的。表示论显然不能解决所有问题，比如 Shafarevich conjecture ，即使 global Langlands 被完全证明了，我们也很难直接了解 if commutator subgroup of the absolute Galois group of Q is free，而我们如果能证明 global non-abelian Artin map is isomorphism，这个问题会简化很多。

## 为什么 Langlands 只关心曲线而不关心高维簇？
comment on why is it that we only consider curves and not higher dimensional varieties. The point is that while function fields of curves are very similar to number fields, the fields of functions on higher dimensional varieties have a very different structure. For example, if X is a smooth surface, then the completions of the field of rational functions on X are labeled by pairs: a point x of X and a germ of a curve passing through x. The corresponding complete field is isomorphic to the field of formal power series in two variables. At the moment no one knows how to formulate an analogue of the Langlands correspondence for the field of functions on an algebraic variety of dimension greater than one, and finding such a formulation is a very important open problem. There is an analogue of the abelian class field theory , i.e. higher class field theory, but not much is known beyond that.

## 啥不能弄到 $GL_3$?
看到之前说的为什么不搞到GL_3。我觉得可以补充一点，当然我不确定这是主要困难）在Galois那边有一个困难的地方，就是难以显式地找出(potentially) semistable/crystalline lift to char 0. 因为local-global compatibility, 来自automorphic representation的Galois representation 会有一定的p-adic Hodge thy 的要求。然后这个要求很难显式地从F_p提升到Q_p, 因为难以计算的H^1 obstruction(在très ramifieé case) 我之前想做这个 我导师表示最好不要做，这个基本不可能做.可以参考这个 这是可能Galois方面的满足一定p-adic Hodge条件的lifting里面最强的结果了。 https://youtu.be/18CxluFd69A   https://mathoverflow.net/questions/74472/what-makes-langlands-for-n-2-easier-than-langlands-for-n2   https://mathoverflow.net/questions/43377/automorphic-forms-on-gl3   可以到 $GL_3$! https://www.galoisrepresentations.com/2017/06/23/new-results-in-modularity-part-i/

## $R\simeq T$?
有个很重要的事实 就是 Hecke 代数可以写成一些eigensystem的积，那么局部化了之后就是eigensystem over \bar \rho 很自然地，根据泛性质就存在了一个映射R—>T;然后 容易严重它的满的 所以本质上TW方法就是证明它也是单的;patching 干了什么呢？它提供了一个东西，T在上面有个自然的作用。我们让R通过满射R—>T也作用在上面。Patching argument告诉我们R的作用是自由的 从而得到R——>T也是单的;关键就是那个东西怎么构造呢？其实用到了Hida thy的想法。先提升level, 再去不动点或者余不动点回归level。具体是写成一堆东西的极限。这个Toby Gee在AWS 2013他的最后两讲很形象地画了不少图 .



