# Common Independent Sets in Graphs with Different Forbidden Cliques

**Manuscript:** *Common independent sets in $K_{s_1}$-free, $\ldots$, $K_{s_k}$-free graphs.*

[Read the LaTeX manuscript](./common_independent_sets_mixed_cliques.tex) ·
[Research webpage](https://lanchao-wang.github.io/drafts/mixed-off-diagonal-ramsey-20261009/) ·
[Publications](https://lanchao-wang.github.io/publications.html)

## Overview

This is a preliminary research manuscript on **multicolour off-diagonal Ramsey numbers**
$r(s_1,\ldots,s_k,t)$ for fixed integers $k\ge 1$ and
$s_1,\ldots,s_k\ge 3$.

The equivalent graph problem is to construct graphs
$G_1,\ldots,G_k$ on a common vertex set, where each $G_i$ is
$K_{s_i}$-free, while the union $G_1\cup\cdots\cup G_k$ has
a small independence number.

## Main result

Put $S=\sum_{i=1}^k(s_i-2)$.
The manuscript claims that for every fixed $k$, fixed
$s_1,\ldots,s_k\ge3$, and every $\varepsilon>0$, there is a
constant $c_{\boldsymbol{s},\varepsilon}>0$ such that
for all sufficiently large $t$,

$$
r(s_1,\ldots,s_k,t)\ge
c_{\boldsymbol{s},\varepsilon}
\frac{t^{S+1}}{(\log t)^{S+\varepsilon}}.
$$

Combined with the cited upper bound of He and Wigderson,
this gives the proposed logarithmic-exponent asymptotic

$$
r(s_1,\ldots,s_k,t)=
\frac{t^{S+1}}{(\log t)^{S+o(1)}}.
$$

Examples of the general formula include:

- The mixed three-colour Ramsey number
  $r(3,4,t)=t^4/(\log t)^{3+o(1)}$.
- The three-colour Ramsey number
  $r(4,4,t)=t^5/(\log t)^{4+o(1)}$.
- The four-colour Ramsey number
  $r(3,4,5,t)=t^7/(\log t)^{6+o(1)}$.

All the small clique sizes and the number of colours are **fixed**;
the statement does not address parameters growing with $t$.

## Relation to previous work

For each forbidden clique size $s_i\ge4$, the manuscript
uses Bradač's ordered flag digraph $D^*(s_i-1,q)$.
The external one-colour compression input is taken from
OpenAI's formalized *SharpLogRamsey* source, with the
corresponding dimension specialization.

The quoted compression theorem requires an orthogonal-rectangle
occupancy condition. The manuscript uses a rectangle-peeling
argument to remove that condition for the needed finite-cover
reduction. It then introduces projection-closed covering families
to carry the reduction through several colours.

For forbidden clique sizes $s_i=3$, the manuscript uses a
triangle-free independent-set counting result of
Andrades, Campos and Morris. The final upper bound
is attributed to He and Wigderson.

## Outline of the argument

1. **Ordered flag graphs.** Encode each $K_{s_i}$-free graph by
   a labelling into the projective flag digraph. Common independent
   sets become simultaneous forward independent tuples.
2. **Entropy upper bound.** Bound the entropy of a forward independent
   tuple in terms of $(s_i-1)m\log q$ and its covering complexity.
3. **External compression theorem.** Quote the selected-step theorem
   with its full occupancy and excess-cost hypotheses; specialize it
   to finite covering families.
4. **Rectangle occupancy removal.** Split inputs between
   concentrated rectangle lists and dispersed tuples, controlling
   entropy under adaptive subsequence selection.
5. **Triangle-free colours.** Use independent-set counts uniform
   over the lengths encountered during the induction.
6. **Multicolour induction.** Lower the covering-complexity level
   one colour at a time using projection-closed covers, ending
   in an entropy contradiction.

## External compression input

The manuscript cites a fixed version of the OpenAI formal source,
revision
[adc7f1241b42e322a6451854ab7e4b4c146bf78a](https://github.com/openai/math/tree/adc7f1241b42e322a6451854ab7e4b4c146bf78a/lean/OAI/Combinatorics/SharpRamsey).

The principal cited declaration is
[SelectedStep.lean: eventually_selected_step](https://github.com/openai/math/blob/adc7f1241b42e322a6451854ab7e4b4c146bf78a/lean/OAI/Combinatorics/SharpRamsey/Marking/SelectedStep.lean).
Related entropy-cost bounds are cited from
[ExcessCost.lean](https://github.com/openai/math/blob/adc7f1241b42e322a6451854ab7e4b4c146bf78a/lean/OAI/Combinatorics/SharpRamsey/Marking/ExcessCost.lean).

The external compression argument is **quoted, not independently reproved**.

## Keywords and related searches

Off-diagonal Ramsey numbers; multicolour Ramsey numbers; multicolor Ramsey
numbers; generalized Ramsey numbers; mixed Ramsey numbers;
$r(s_1,\ldots,s_k,t)$; $r(s_1,s_2,t)$;
$r(3,4,t)$; $r(4,4,t)$; $r(3,4,5,t)$;
Ramsey numbers with fixed small cliques;
$K_s$-free graphs; $K_4$-free graphs;
common independent sets in graphs with different forbidden cliques;
independence number of the union of $K_s$-free graphs;
ordered flag graphs; Bradač digraph; projective geometry;
probabilistic combinatorics; extremal graph theory;
Shannon entropy; entropy method; entropy compression;
single-colour compression; orthogonal rectangles; rectangle occupancy;
rectangle peeling; projection-closed covering families;
He--Wigderson upper bound; Andrades--Campos--Morris;
OpenAI SharpLogRamsey.

## Status

**Preliminary, unrefereed manuscript.** Source revision: October 8, 2026;
posted in this repository on October 9, 2026.
The mathematical proof and its application of external results have
not been independently verified. Corrections and reports of
possible errors are welcome.

## AI assistance

This manuscript was produced by GPT-6 under the author's guidance.
