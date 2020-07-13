---
title: "Revisiting Tardos's Framework for Linear Programming: Faster Exact Solutions
using Approximate Solvers"
collection: preprints 
permalink: /preprints/blackbox.html
excerpt: "Based on breakthrough work  Tardos (Oper. Res. '86), we give a substantially improved framework, in which we replace
the exact LP solves with _approximate_ ones, enabling us to
directly leverage the tremendous recent algorithmic progress for approximate
linear programming."
date: 2020-04-17
# venue: 'Symposium on Theory of Computing (STOC)'
# arxiv: 'https://arxiv.org/abs/1912.06252'
# pdf: 'files/scaling_invariant/pdf.pdf'
# citation: 'Your Name, You. (2015). &quot;Paper Title Number 3.&quot; <i>Journal 1</i>. 1(3).'
coauthors: 'Daniel Dadush, and L&aacute;szl&oacute; A. V&eacute;gh. <i>Accepted to Foundations of Computer Science (FOCS), 2020</i>' 
---
In breakthrough work, Tardos (Oper. Res. '86) gave a *proximity* based
framework for solving linear programming (LP) in time depending only on
the constraint matrix in the bit complexity model. In Tardos's
framework, one reduces solving the LP $\min \langle c, x \rangle$, $Ax=b$,
$x \geq 0$, $A \in \Z^{m \times n}$, to solving $O(mn)$ LPs in $A$
having small integer coefficient objectives and right-hand sides using
*any exact* LP algorithm.

In this work, we give a substantially improved framework, in which we
replace the exact LP solves with *approximate* ones, enabling us to
directly leverage the tremendous recent algorithmic progress for
approximate linear programming. More precisely, we show that the
fundamental "accuracy" needed to *exactly* solve any LP in $A$ is
inverse polynomial in $n$ and Stewart's $\bar{\chi}\_A$, a well-studied
condition number. Plugging in the recent algorithm of van den Brand
(SODA '20), our method computes an optimal primal and dual solution
using ${O}(m n^{\omega+1} \log
(n)\log(\bar{\chi}\_A+n))$ arithmetic operations, outperforming the
specialized interior point method of Vavasis and Ye (Math. Prog. '96)
and its recent improvement by Dadush et al (STOC '20). By applying the
preprocessing algorithm of the latter paper, the dependence can also be
reduced from $\bar\chi_A$ to $\bar{\chi}\_A^*$, the minimum value of
$\bar\chi\_{AD}$ attainable via column rescalings. Our framework is
applicable to achieve a ${\rm poly}(n)\log(\bar{\chi}_A+n)$ using
essentially any other weakly polynomial LP algorithm, such as the
ellipsoid method.

At a technical level, our framework combines together approximate LP
solutions to compute exact ones, making use of constructive proximity
theorems---which bound the distance between solutions of "nearby"
LPs---to keep the required accuracy low.
