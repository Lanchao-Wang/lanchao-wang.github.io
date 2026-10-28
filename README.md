# Research manuscripts and drafts

This repository hosts a research webpage, published works and selected
preliminary manuscripts in graph theory, Ramsey theory and probabilistic
combinatorics.

[Research webpage](https://lanchao-wang.github.io/) ·
[Publications](https://lanchao-wang.github.io/publications.html)

## The Choice Number of Random Graphs

**Lanchao Wang and Jiasheng Zeng**

A preprint proving the Alon–Krivelevich–Sudakov conjecture on **list colouring of random graphs**. Whenever `np → ∞`, we show that, with high probability, the choice number and chromatic number of the binomial random graph `G(n,p)` are asymptotically equal:

$
\operatorname{ch}(G(n,p))=(1+o(1))\chi(G(n,p)).
$

The proof treats growing and bounded independent sets separately. It combines a uniform independent-set estimate and the Krivelevich–Vu method with a deterministic theorem converting a proper colouring with bounded colour classes into a list colouring under a uniform independent-set condition. Random vertex sampling, Kahn's matching theorem, first-moment estimates and Janson's inequality complete the argument.

[arXiv:2610.35003](https://arxiv.org/abs/2610.35003) ·
[arXiv PDF](https://arxiv.org/pdf/2610.35003) ·
[Paper overview and version history](./drafts/chromatic-choice-random-graphs-20261022/) ·
[Version comparison and keywords](./drafts/chromatic-choice-random-graphs-20261022/README.md)

**Status:** arXiv preprint; [v1 submitted October 26, 2026](https://arxiv.org/abs/2610.35003v1), 12 pages. Not yet peer reviewed.

**Archived earlier draft:** *Asymptotic equality of chromatic and choice numbers in random graphs*, revised October 20, 2026 and uploaded October 22, 2026. The [archived LaTeX source](./drafts/chromatic-choice-random-graphs-20261022/asymptotic_equality_chromatic_choice_random_graphs.tex) and [archived PDF (14 pages)](./drafts/chromatic-choice-random-graphs-20261022/asymptotic_equality_chromatic_choice_random_graphs.pdf) are retained unchanged and are **not the arXiv v1 files**.

**AI assistance:** The arXiv acknowledgements credit GPT-5.6 with developing the large-independent-set proof autonomously and GPT-6 with technical assistance on the authors' bounded-independent-set strategy. The authors wrote the final manuscript and take responsibility for it; see the [arXiv version](https://arxiv.org/html/2610.35003v1) for the full disclosure.

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
