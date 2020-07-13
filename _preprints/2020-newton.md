---
title: "A Strongly Polynomial Label-Correcting Algorithm for Linear Systems with Two Variables per Inequality"
collection: preprints 
permalink: /preprints/2VPI.html
arxiv: 'https://arxiv.org/abs/2004.08634'
pdf: 'files/newton/pdf.pdf'
excerpt: 'We present a strongly polynomial label-correcting algorithm for solving the feasibility of linear systems with two variables per inequality (2VPI). The algorithm is based on the Newton-Dinkelbach method for fractional combinatorial optimization and extends previous work of Madani (2002). We also obtain an acceleration of the Newton-Dinkelbach method for general fractional combinatorial optimization problems.'
date: 2020-04-17
coauthors: 'Zhuan Khye Koh, and L&aacute;szl&oacute; A. V&eacute;gh. <i>Submitted</i>' 
---

[Mobile-friendly](../files/newton/web/index.html)

[Download paper here](https://arxiv.org/abs/2004.08634)

We present a strongly polynomial label-correcting algorithm for solving the feasibility of linear systems with two variables per inequality (2VPI).
The algorithm is based on the Newton--Dinkelbach method for fractional combinatorial optimization.
We extend and strengthen previous work of Madani (2002) that showed a weakly polynomial bound for a variant of the Newton--Dinkelbach method for solving deterministic Markov decision processes (DMDPs), a special class of 2VPI linear programs.
For a 2VPI system with $n$ variables and $m$ constraints, our algorithm runs in $O(mn)$ iterations.
Every iteration takes $O(m + n\log n)$ time for DMDPs, and $O(mn)$ time for general 2VPI systems.
The key technical idea is a new analysis of the Newton--Dinkelbach method exploiting gauge symmetries of the algorithm. This also leads to an acceleration of the Newton--Dinkelbach method for general fractional combinatorial optimization problems.
For the special case of linear fractional combinatorial optimization, our method converges in $O(m\log m)$ iterations, improving upon the previous best bound of $O(m^2\log m)$ by Wang et al.~(2006).