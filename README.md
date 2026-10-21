# Research manuscripts and drafts

This repository hosts a research webpage, published works and selected
preliminary manuscripts in graph theory, Ramsey theory and probabilistic
combinatorics.

[Research webpage](https://lanchao-wang.github.io/) ·
[Publications](https://lanchao-wang.github.io/publications.html)

## Asymptotic equality of chromatic and choice numbers in random graphs

**Lanchao Wang and Jiasheng Zeng**

A research manuscript proving the Alon–Krivelevich–Sudakov conjecture on **list colouring of random graphs**. Whenever `np → ∞`, we show that the choice number and chromatic number of the binomial random graph `G(n,p)` are asymptotically equal:

$
\operatorname{ch}(G(n,p))=(1+o_{\mathbb P}(1))\chi(G(n,p)).
$

The proof handles growing and bounded colour classes separately. It combines uniform independent-set estimates and the Krivelevich–Vu method with a deterministic clique-partition-to-list-colouring proposition proved using random sampling of clique packings and Kahn's matching theorem. First-moment and Janson estimates complete the argument.

[Read the draft overview](./drafts/chromatic-choice-random-graphs-20261022/) ·
[Detailed research note and keywords](./drafts/chromatic-choice-random-graphs-20261022/README.md) ·
[LaTeX manuscript](./drafts/chromatic-choice-random-graphs-20261022/asymptotic_equality_chromatic_choice_random_graphs.tex) ·
[PDF manuscript](./drafts/chromatic-choice-random-graphs-20261022/asymptotic_equality_chromatic_choice_random_graphs.pdf)

**Status:** Unrefereed research manuscript. Revised October 20, 2026; uploaded October 22, 2026.

**AI assistance:** This manuscript was prepared with the assistance of ChatGPT (GPT-6) under the authors' guidance.

## Related search terms

List colouring; list coloring; choice number; chromatic number; choosability; random graphs; Erdős–Rényi graph; G(n,p); Alon–Krivelevich–Sudakov conjecture; clique partitions; Kahn's matching theorem.

---

## Current research draft

### Common independent sets in $K_{s_1}$-free, $\ldots$, $K_{s_k}$-free graphs

A preliminary research draft on **multicolour off-diagonal Ramsey numbers**
$r(s_1,\ldots,s_k,t)$ for fixed $k$ and fixed forbidden clique sizes
$s_1,\ldots,s_k\ge 3$. The draft claims that if
$S=\sum_{i=1}^k(s_i-2)$ then

$$
r(s_1,\ldots,s_k,t)=\frac{t^{S+1}}{(\log t)^{S+o(1)}}.
$$

This generalizes the earlier draft restricted to several
$K_4$-free graphs. The proof uses Bradač's ordered flag graphs,
OpenAI's cited single-colour compression theorem, a rectangle-peeling
argument, projection-closed covering families, and a triangle-free
independent-set counting result of Andrades, Campos and Morris.

[Read the draft overview](./drafts/mixed-off-diagonal-ramsey-20261009/) ·
[Detailed research note and keywords](./drafts/mixed-off-diagonal-ramsey-20261009/README.md) ·
[LaTeX manuscript](./drafts/mixed-off-diagonal-ramsey-20261009/common_independent_sets_mixed_cliques.tex)

**Status:** Unrefereed preliminary draft. Source revised October 8, 2026;
uploaded October 9, 2026. Independent mathematical verification pending.

## Search terms

Off-diagonal Ramsey numbers; multicolour Ramsey numbers;
multicolor Ramsey numbers; mixed Ramsey numbers; generalized Ramsey theory;
$r(s_1,\ldots,s_k,t)$; $r(3,4,t)$; $r(4,4,t)$;
$K_s$-free graphs; triangle-free graphs; common independent sets;
finite projective geometry; entropy compression; orthogonal rectangles;
rectangle occupancy; projection-closed covering families.

Corrections and mathematical comments are welcome.
