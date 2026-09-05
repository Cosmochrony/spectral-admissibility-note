This repository contains the source of the **Spectral Admissibility Presentation Note** Cosmochrony paper  
*The Spectral Admissibility Sub-Programme — Presentation Note 1*.

This work is a **structured entry point** to the spectral admissibility
sub-programme (Branch II of the Cosmochrony corpus), not a summary of results.
It maps the constituent papers, identifies the internal phases, records the
status of every result as proved, structural, numerical, conditional, or open, and states
the remaining open deliverables.

## Central Question

The non-injective projection $\Pi$ acts on the Weil representation of the
Heisenberg group $\mathrm{Heis}_3(\mathbb{Z}/q\mathbb{Z})$, decomposed into
irreducible blocks $V_c$ indexed by characters
$c \in (\mathbb{Z}/q\mathbb{Z})^\times$.
The Born--Infeld saturation constraint bounds the projective flux carried by
each mode,

$A_n \leq A^{\max}_n := c_{\mathrm{BI}} / \sqrt{\lambda_n}$,

where $\lambda_n$ is the Laplacian eigenvalue at BFS depth $n$ and $c_{\mathrm{BI}}$ is
the Born--Infeld saturation constant.

> Which combinations of Weil sectors remain admissible under this constraint,
> and what capacity exponent $\delta_{\mathrm{pair}}$ do they carry?

## Logical Chain

The sub-programme is organised around a single derivation chain:

$c_{\mathrm{BI}}
\;\Longrightarrow\;
A^{\max}_n = c_{\mathrm{BI}}/\sqrt{\lambda_n}
\;\Longrightarrow\;
\sigma^{\mathrm{can}}_{\mathrm{pair}}(n)
\;\Longrightarrow\;
\delta_{\mathrm{pair}}$.

i.e. **bounded flux** $\Rightarrow$ **admissibility envelope** $\Rightarrow$
**Weil-sector capacity** $\Rightarrow$ **capacity exponent**.

On the segment $c_{\mathrm{BI}} \to \delta_{\mathrm{pair}}$, **O24** closes the
fibre-structure conditionality under a supplied carrier, and no free parameter is
adjusted. The further step to the cascade exponent is **not** part of the chain:
the reciprocal prescription
$\beta^* \approx 1/(\delta_{\mathrm{pair}} + \tfrac{1}{2})$ has no carrier on the
Heisenberg measurement substrate, and the **Span-Growth Note** proves that the
expander-derived conversion does not transfer there. The agreement of
$\beta^* \approx 0.126$ with the phenomenological window
$\beta^* \in (0.09, 0.13)$, which O3 fixes by matching the charged-lepton
sector, is a coincidence check, not a derivation.
The group-theoretic extensions are conditional or withdrawn: the
$\mathfrak{su}(2)$ identification rests on a supplied carrier, and the $SU(3)$
extension is withdrawn.

## Position in the Programme

The Cosmochrony corpus is organised into three branches:

- **Branch I** — axiomatic primitive: admissible non-injective transitions.
  The selection of $\mathrm{Heis}_3(\mathbb{Z}/q\mathbb{Z})$ and its Weil
  representation from A1–A4 is **not** a theorem: HeisenbergStructure disproves
  that implication by a six-element countermodel, so the carrier is supplied.
- **Branch II** — the spectral admissibility sub-programme (this note): the
  **computational engine** of the corpus.
- **Branch III** — derives quantum mechanics, spacetime geometry, gauge
  structure, and fermionic matter from Branch I axioms and Branch II spectral data.

Branch II takes the algebraic output of Branch I and produces the two inputs
Branch III depends on:

1. the admissibility thread $Q_8 \subset 2I \subset SU(2)$, within which the
   spin-$\tfrac{1}{2}$ sector is selected by O26 minimality on a carrier supplied
   by O23 rather than identified here;
2. the capacity exponent $\delta_{\mathrm{pair}}$ and its interpretation as the
   scaling exponent of Hilbert–Schmidt norm growth in the minimal admissible
   non-abelian sector $\mathfrak{su}(2)$. The reciprocal $\beta^* \approx 0.126$
   is a coincidence check, not an output of the chain.

## Constituent Papers

The sub-programme comprises **five precursor papers**, the O-series papers
**O1 and O3–O33**, and **two companion notes** (Span-Growth, Critical Coverage),
organised into internal phases:

| Phase | Papers | Central output | Status |
|---|---|---|---|
| Precursors | SpAdm, SpCap, SpGram, 3Gen | $Q_8 \subset 2I$; binary maximality for $d \in \{6,12,24\}$ | P/S |
| LPS phase | SpRel, O1–O8 | geometric obstruction; no cascade-exponent bound | P/O |
| Heisenberg transition | O9–O15 | crossover slope $\approx 4.5$, unfolded $\delta_{\rm exact}=3$; cond. bound | P/C |
| Pair + transfer | O16–O24 | $c_{\mathrm{BI}} \to \delta_{\mathrm{pair}}$ fibre-conditionality closed | C |
| Numerical + sector | O25–O30 | $\delta_{\mathrm{corr}}$ diagnostic; $r_{\mathrm{eff}} = 3$ finite-data | N/C |
| SU(3) / colour | O31–O32 | O31 withdrawn; O32 measurements stand | O |
| Spectral architecture | O33 | exact doublets and protected sectors, no Standard-Model identification | P |
| Companion notes | Span-Growth, Critical Coverage | transfer failure; exact depth law | P |

Status codes: **P** = proved, **S** = structural, **N** = numerical,
**C** = conditional, **O** = open.

## Open Deliverables

Three open deliverables define the current boundary of the sub-programme:

1. **$[\mathrm{H\text{-}color}]$.**
   Two of its four levels stand, both established in **O32**: block-averaged
   equality to $O(q^{-1})$ and effective-exponent equality in the $q \to \infty$
   limit. Sector rank equality and pointwise profile equality rested on the
   superseded version of **O31**, whose current record is a withdrawal notice and
   asserts neither; they are open, and no $SU(3)$ identification follows.
2. **Spin-$\tfrac{1}{2}$ identification.**
   The carrier is supplied by O23 and selected by O26 minimality; the vector lift
   of O26 Hypothesis 4.4 is open, and no measurement of the sub-programme
   identifies $V_\rho$.
3. **Numerical campaign at full breadth.**
   The pair-level campaign runs at $q \in \{29, 61, 101, 151, 211\}$ at full
   breadth and is extended in O25 to $q \in \{307, 401, 601\}$ at reduced
   sampling, so the large-$q$ dispersion there is inflated by the reduced pair
   count. What remains is breadth rather than reach.

## Status

The $SU(2)$ sector is **carried by a conditional chain, not closed**: its carrier
is supplied by O23 and O26 Hypothesis 4.4 is open. The numerical campaign is
complete at full breadth for $q \in \{29, 61, 101, 151, 211\}$ and extended at
reduced sampling to $q \in \{307, 401, 601\}$.
The extension to $SU(3)$ is **open**: O31 version 2.0 withdraws the colour-group
derivation and every derivation of a gauge factor.

## Build

```bash
bash compile.sh
```

This runs `pdflatex → bibtex → pdflatex → pdflatex` on
`tex/SpectralAdmissibilityNote.tex` and produces
`out/SpectralAdmissibilityNote.pdf`.
