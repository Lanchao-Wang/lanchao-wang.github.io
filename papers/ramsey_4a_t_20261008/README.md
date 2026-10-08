# Common Independent Sets in a Fixed Number of $K_4$-Free Graphs

[Read the manuscript (LaTeX source)](./ramsey_4a_t_blackbox_20261008.tex) ·

## Overview

Let $r(4,\ldots,4,t)$ denote the multicolour off-diagonal Ramsey number
in which $4$ occurs a fixed number $a$ of times, followed by $t$.
Equivalently, the lower-bound problem asks for $a$ $K_4$-free graphs
on a common vertex set whose union has no independent set of size $t$.

The manuscript uses Bradač's ordered flag construction and a one-colour
entropy-compression input to treat an arbitrary fixed number of
$K_4$-free colour classes.

## Main result

For every fixed integer $a\geq 1$ and $\varepsilon>0$, the
manuscript establishes, subject to the external compression theorem and
the verification status described below, a constant
$c_{a,\varepsilon}>0$ such that for all sufficiently large $t$,

$$
r(\underbrace{4,\ldots,4}_{a\text{ copies}},t)
\geq c_{a,\varepsilon}
\frac{t^{2a+1}}{(\log t)^{2a+\varepsilon}}.
$$

Together with the known upper bound of He and Wigderson, this yields
the claimed logarithmic-exponent asymptotics

$$
r(\underbrace{4,\ldots,4}_{a\text{ copies}},t)
=\frac{t^{2a+1}}{(\log t)^{2a+o(1)}}.
$$

Special instances include

- the three-colour off-diagonal Ramsey number
  $r(4,4,t)=t^5/(\log t)^{4+o(1)}$;
- the four-colour off-diagonal Ramsey number
  $r(4,4,4,t)=t^7/(\log t)^{6+o(1)}$.

These are consequences of a single statement for every fixed $a$;
the theorem does **not** allow $a$ to grow with $t$.

## Relation to previous work

The graph construction is based on Bradač's digraph $D^*(3,q)$.
For each label map $\phi$, the associated graph $G_\phi$ is
$K_4$-free, and its independent sets correspond to *forward
independent* ordered tuples of projective flags.

The one-colour compression input is taken from OpenAI's formalized
SharpLogRamsey source, specifically the dimension-four specialization
of its selected-step theorem. That theorem has an orthogonal-rectangle
occupancy hypothesis. The manuscript separates the cited theorem
from the additional deductions needed in the multicolour setting.

The matching upper-bound exponent is from He and Wigderson; it is not
claimed as a new result.

## Main ideas

### Flag graphs and common independent sets

One uses $a$ label maps to construct $a$ graphs on the same vertex
set. A common independent set gives one forward independent tuple
for each colour. Their joint entropy is bounded below by the
number of possible original labellings.

### A one-colour entropy estimate

Bradač's marking/tree argument controls the number of forward
independent tuples inside products with small coordinate domains.
It gives an entropy bound of the form

$$
H(X)\leq 3m\log q+O(m)+B,
$$

where $B$ is the covering complexity.

### Orthogonal rectangles and occupancy removal

The compression theorem requires each orthogonal rectangle to meet
the selected tuple in only $O(\log q)$ positions. A greedy
rectangle-peeling argument splits a tuple into a structured part and
a dispersed part. The structured part has a direct low-complexity
cover; the dispersed part satisfies the occupancy condition.
Entropy estimates justify passage to the selected subsequences.

### Projection-closed covering families

A product is a Cartesian product of coordinate label domains. A
covering family is *projection-closed* if it contains every
coordinate projection of each product. This permits an adaptively
selected subsequence in one colour to be used simultaneously in all
the other colours without increasing their covering complexities.

### The multicolour induction

The resulting reduction decreases the complexity exponent for one
colour at a time. An induction on the sum of the $a$ complexity
indices ends with an entropy contradiction.

## External theorem and scope of verification

The external compression input is cited from the fixed OpenAI source
revision
[adc7f1241b42e322a6451854ab7e4b4c146bf78a](https://github.com/openai/math/tree/adc7f1241b42e322a6451854ab7e4b4c146bf78a/lean/OAI/Combinatorics/SharpRamsey):

- [SelectedStep.lean: eventually_selected_step](https://github.com/openai/math/blob/adc7f1241b42e322a6451854ab7e4b4c146bf78a/lean/OAI/Combinatorics/SharpRamsey/Marking/SelectedStep.lean)
- [ExcessCost.lean: excessCost_linear and twoExpensive_linear](https://github.com/openai/math/blob/adc7f1241b42e322a6451854ab7e4b4c146bf78a/lean/OAI/Combinatorics/SharpRamsey/Marking/ExcessCost.lean)

The manuscript states the external input, derives a finite-cover
consequence, removes its rectangle-occupancy hypothesis, and then
runs the $a$-colour induction. It does **not** reproduce an
independent proof of the external compression argument.

## Keywords and related search terms

Multicolour Ramsey numbers; multicolor Ramsey numbers; off-diagonal
Ramsey numbers; generalized off-diagonal Ramsey theory;
$r(4,4,t)$; $r(4,4,4,t)$; $r(4,\ldots,4,t)$;
three-colour Ramsey number $r(4,4,t)$;
four-colour Ramsey number $r(4,4,4,t)$;
$K_4$-free graphs; common independent sets;
independence number of a union of $K_4$-free graphs;
Bradač's $D^*(3,q)$ digraph; ordered flag graphs;
finite projective geometry; projective flags;
Shannon entropy; entropy compression; flag compression;
one-colour compression; orthogonal rectangles;
rectangle occupancy; rectangle peeling;
projection-closed covering families;
probabilistic combinatorics; extremal graph theory;
He--Wigderson Ramsey bound; OpenAI SharpLogRamsey.

## AI assistance

AI tools assisted in the development and revision of the manuscript.
The cited external compression theorem is taken from OpenAI's
formalized source. The full argument, including its new deductions,
has not been independently verified as of this version.
