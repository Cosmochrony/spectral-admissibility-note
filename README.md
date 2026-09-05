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
\delta_{\mathrm{pair}}
\;\Longrightarrow\;
\beta^* \approx 0.126$.

i.e. **bounded flux** $\Rightarrow$ **admissibility envelope** $\Rightarrow$
**Weil-sector capacity** $\Rightarrow$ **capacity exponent** $\Rightarrow$
**cascade exponent**.

The transfer segment is *unconditional* with respect to the fibre structure of
$\Pi$ (closed in **O24**): no free parameter is adjusted to produce $\beta^*$.
The group-theoretic extensions are not: the $\mathfrak{su}(2)$ identification is
conditional on a supplied carrier, and the $SU(3)$ extension is withdrawn.
The value $\beta^* \approx 0.126$ matches the phenomenological window
$\beta^* \in (0.09, 0.13)$ derived from the charged-lepton mass ratios
$m_e : m_\mu : m_\tau$, making the sub-programme the primary quantitative
connection between the projective framework and Standard Model observables
via the structural relation $\beta^* \approx 1/(\delta_{\mathrm{pair}} + \tfrac{1}{2})$.

## Position in the Programme

The Cosmochrony corpus is organised into three branches:

- **Branch I** — axiomatic primitive: four axioms (A1–A4) derive
  $\mathrm{Heis}_3(\mathbb{Z}/q\mathbb{Z})$ and its Weil representation as theorems.
- **Branch II** — the spectral admissibility sub-programme (this note): the
  **computational engine** of the corpus.
- **Branch III** — derives quantum mechanics, spacetime geometry, gauge
  structure, and fermionic matter from Branch I axioms and Branch II spectral data.

Branch II takes the algebraic output of Branch I and produces the two inputs
Branch III depends on:

1. the admissible sector as the spin-$\tfrac{1}{2}$ representation of $SU(2)$,
   embedded via the admissibility thread $Q_8 \subset 2I \subset SU(2)$;
2. the value $\beta^* \approx 0.126$ and its interpretation as the scaling
   exponent of Hilbert–Schmidt norm growth in the minimal admissible
   non-abelian sector $\mathfrak{su}(2)$.

## Constituent Papers

The sub-programme comprises **five precursor papers** and **thirty-two
O-series papers**, organised into internal phases:

| Phase | Papers | Central output | Status |
|---|---|---|---|
| Precursors | SpAdm, SpCap, SpGram, 3Gen | $Q_8 \subset 2I$, binary maximality | P/S |
| LPS phase | SpRel, O1–O8 | $\beta \leq 1$; geometric obstruction | P |
| Heisenberg transition | O9–O15 | exact $\hat\delta_{\mathrm{exact}} \approx 4.5$; no-go | P |
| Pair + transfer | O16–O24 | $c_{\mathrm{BI}} \to \delta_{\mathrm{pair}} \to \beta^*$, unconditional | P |
| Numerical + sector | O25–O30 | $\delta_{\mathrm{corr}}$ diagnostic; $r_{\mathrm{eff}} = 3$ | N/C |
| SU(3) / colour | O31–O32 | O31 withdrawn; O32 measurements stand | O |

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
3. **Numerical campaign at $q = 401$.**
   The campaign at $q \in \{29, 61, 101, 151, 211, 307\}$ is complete;
   $q = 401$ is the sole remaining numerical task, constraining the convergence
   rate of $n_1(q)/q$ and providing a fifth data point for the
   $R_{\mathrm{var}}(q) \propto q^{-1}$ scaling prediction.

## Status

The $SU(2)$ sector is **carried by a conditional chain, not closed**: its carrier
is supplied by O23 and O26 Hypothesis 4.4 is open. The numerical campaign is
complete for $q \in \{29, 61, 101, 151, 211, 307\}$.
The extension to $SU(3)$ is **open**: O31 version 2.0 withdraws the colour-group
derivation and every derivation of a gauge factor.

## Build

```bash
bash compile.sh
```

This runs `pdflatex → bibtex → pdflatex → pdflatex` on
`tex/SpectralAdmissibilityNote.tex` and produces
`out/SpectralAdmissibilityNote.pdf`.
