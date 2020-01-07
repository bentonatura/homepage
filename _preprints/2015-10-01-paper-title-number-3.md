---
title: "A scaling-invariant algorithm for linear programming whose running time depends only on the constraint matrix"
collection: preprints 
permalink: /preprints/scaling_invariant_lls
excerpt: 'We find a scaling-invariant layered least squared algorithm for linear programming'
date: 2019-12-12
arxiv: 'https://arxiv.org/abs/1912.06252'
pdf: 'files/scaling_invariant.pdf'
# citation: 'Your Name, You. (2015). &quot;Paper Title Number 3.&quot; <i>Journal 1</i>. 1(3).'
coauthors: Daniel Dadush, Sophie Huiberts, and L&aacute;szl&oacute; A. V&eacute;gh 
---

[Download paper here](https://arxiv.org/abs/1912.06252)

Following the breakthrough work of Tardos (Oper. Res. '86) in the bit-complexity
model, Vavasis and Ye (Math. Prog. '96) gave the first exact algorithm for
linear programming in the real model of computation with running time depending
only on the constraint matrix. For solving a linear program (LP)
$\max\, c^\top x,\:  Ax = b,\:  x \geq 0,\:  A \in \R^{m \times n}$, Vavasis and Ye
developed a primal-dual interior point method using a _layered least
squares_ (LLS) step, and showed that $O(n^{3.5} \log
(\bar{\chi}_A+n))$ iterations suffice to solve (LP) exactly, where $\bar{\chi}_A$ is a condition measure
controlling the size of solutions to linear systems related to $A$. 

Monteiro and Tsuchiya (SIAM J. Optim. '03), noting that the central path is
invariant under rescalings of the columns of $A$ and $c$, asked whether there
exists an LP algorithm depending instead on the measure $\bar{\chi}^\ast_A$,
defined as the minimum $\bar{\chi}_{AD}$ value achievable by a column rescaling $AD$ of
$A$, and gave strong evidence that this should be the case. We resolve
this open question affirmatively. 

Our first main contribution is an $O(m^2 n^2 + n^3)$ time algorithm which works
on the linear matroid of $A$ to compute a nearly optimal diagonal
rescaling $D$ satisfying $\bar{\chi}\_{AD} \leq n(\bar{\chi}^\ast)^3$. This
algorithm also allows us to approximate the value of $\bar{\chi}\_A$ up to a
factor $n (\bar{\chi}^\ast)^2$. This result is in (surprising) contrast to that of
Tun&ccedil;el (Math.  Prog. '99), who showed NP-hardness for approximating
$\bar{\chi}\_A$ to within $2^{\mathrm{poly}(\mathrm{rank}(A))}$. The key insight for
our algorithm is to work with ratios $g\_i/g\_j$ of circuits of $A$ &mdash; i.e.,minimal linear dependencies $Ag=0$ &mdash; which allow us to approximate the
value of $\bar{\chi}\_A^\ast$ by a maximum geometric mean cycle computation in what we
call the _circuit ratio digraph_ of $A$.   

While this resolves Monteiro and Tsuchiya's question by appropriate
preprocessing, it falls short of providing either a truly scaling invariant
algorithm or an improvement upon the base LLS analysis. In this vein, as our
second main contribution we develop a _scaling invariant_ LLS algorithm,
which uses and dynamically maintains improving estimates of the circuit ratio
digraph, together with a refined potential function based analysis for LLS
algorithms in general. With this analysis, we derive an improved $O(n^{2.5} \log
n\log (\bar{\chi}^\ast_A+n))$ iteration bound for optimally solving (LP) using
our algorithm. The same argument also yields a factor $n/\log n$ improvement on the
iteration complexity bound of the original Vavasis-Ye algorithm.
