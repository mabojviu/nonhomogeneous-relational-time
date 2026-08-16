# LQTA-D Article 3 — Global Definition-Order and Notation Audit v0.1

Date: 2026-08-16
Scope: `main.tex` plus editorial passes 01–06.
Scientific status: no theorem/result reopened.

## Global verdict

`PASS_SCIENTIFIC_CONTENT__EDITORIAL_INTEGRATION_PATCH_REQUIRED`

Recommended next state:

`INTEGRATE_EDITORIAL_PASSES_WITH_DEFINITION_ORDER_AND_NOTATION_PATCH`

No analytic or numerical campaign must be repeated. All required changes are editorial, not scientific.

---

## 1. Definition-before-use audit

### 1.1 Abstract and Introduction

Status: `PASS_WITH_PREVIEW_SIMPLIFICATION`.

The Abstract and Introduction preview several symbols before the formal setup (`D_0`, `phi`, `eta`, `R`, `kappa`, `K`). Preview use is acceptable in principle, but the manuscript can be made clearer by applying a strict rule:

- Abstract: define only `gamma` symbolically; describe exact/non-exact decomposition verbally rather than introducing `D_0 phi + eta` unless all symbols are named in the same sentence.
- Introduction: symbolic preview is allowed, but every previewed object must receive one short verbal identification before first equation.
- Formal definitions begin in the Setup section and are authoritative thereafter.

Recommended minimal patch in Abstract:

Replace the explicit decomposition formula by wording equivalent to:

> `In the general case the CAL state splits orthogonally into an exact component and a gauge-invariant cycle component.`

The equation `gamma=D_0 phi+eta` can remain in the Introduction provided the text immediately identifies `D_0` as the vertex-to-edge coboundary, `phi` as a vertex potential, and `eta` as the non-exact component.

### 1.2 `beta_1`

Status: `PATCH_REQUIRED_IN_MAIN`.

The current `main.tex` uses `beta_1` in tree rigidity before giving its graph-theoretic definition. Editorial Pass 02 fixes this correctly with

`beta_1(G)=dim ker(D_0^T)=|E|-|V|+1`

for a connected carrier.

Action: integrate the Pass-02 dimension proposition before any use of `beta_1`.

### 1.3 Effective resistance

Status: `PATCH_REQUIRED`.

The minimal path-to-triangle example currently previews `R_eff` before its definition in the support-change section. This violates the desired definition order.

Action: remove the early numerical `R_eff=2` cross-check from the integrability example. Keep only:

> `The same example will be recovered later from the single-edge birth law.`

Then perform the explicit `R_eff` calculation only after the formal definition of effective resistance.

### 1.4 Structural source terminology

Status: `PATCH_REQUIRED_FOR_ORDER`.

Pass 02 defines classes named `source-positive` / `source-negative` before Pass 03 formally defines the provenance source field `S_T`.

Two safe options exist. Preferred:

1. order the final manuscript as
   - memory geometry,
   - realized change + provenance continuity,
   - fixed-carrier transition classes;
2. then state explicitly that the sign of `Delta R` equals the sign of the root source `(S_T)_{v_*}` whenever a provenance tree is supplied.

This makes the word `source` formally grounded before the named transition classes.

Alternative: rename the pre-provenance classes `R-increasing`, `R-preserving`, `R-decreasing`, and introduce `source-positive/negative` only after `S_T`. The first option preserves the frozen terminology more closely.

### 1.5 Generic divergence in the current-ambiguity paragraph

Status: `PATCH_REQUIRED`.

Pass 03 uses

`J' = J + h,  div h = 0`

on a generic cyclic routing carrier, but only `div_T` on the rooted provenance tree has been formally defined.

Action: either define a generic incidence divergence operator before this paragraph, or avoid introducing a second untyped divergence. Preferred wording:

> `On a cyclic routing graph, adding any circulation in the kernel of its incidence divergence leaves the same vertex balance.`

No new symbol is necessary.

### 1.6 Changing-support coboundaries and projectors

Status: `PATCH_REQUIRED`.

Pass 04 introduces `D_0^-`, `D_0^+`, `P_{perp,+}` etc. without an explicit one-line definition that they are the coboundary/projector associated with `G_-` and `G_+`.

Action: immediately after introducing `G_-` and `G_+`, define the carrier-indexed operators.

### 1.7 Gauge action on derived rates

Status: `PATCH_REQUIRED_FOR_TRANSPARENCY`.

The gauge-invariance proof of the cycle-birth defect states that `gamma_e` and `log(r_v/r_u)` shift together, but the transformation of derived rates is not explicitly stated earlier.

Add once in Setup:

`gamma -> gamma + D_0 q`, `phi -> phi + q`, hence `r_i -> e^{q_i} r_i`.

This makes every later gauge-invariance proof immediate.

### 1.8 Provenance

Status: `PASS_WITH_GLOSSARY_SENTENCE`.

Technical event provenance is properly defined before the continuity theorem. Add one short sentence in the Introduction to prevent a reader from treating it as future causal influence:

> `Here provenance denotes realized historical/precedence structure associated with an event; it does not by itself select a future update.`

This also aligns Article 3 with the LQTA-T terminology harmonization audit.

---

## 2. Global notation audit

### 2.1 Fixed-support versus changing-support states

Status: `HIGH_PRIORITY_PATCH`.

Current drafts use superscript `-` / `+` both for before/after states on one fixed carrier and for states that live on different carriers. This visually encourages illegal expressions such as `eta^+ - eta^-` under support change.

Canonical policy:

**Fixed carrier** `G=(V,E)`:

- `gamma^- -> gamma^+`
- `eta^- -> eta^+`
- `rho^- -> rho^+`
- `Delta eta = eta^+ - eta^-`
- `Delta R = R^+ - R^-`

**Changing carrier**:

- `G_- -> G_+`
- `gamma_- in C^1(G_-;R)` and `gamma_+ in C^1(G_+;R)`
- `eta_-`, `eta_+`
- `R_-`, `R_+`
- never write `Delta eta` across carriers unless an endogenous identification has first been defined.

This typographic distinction should be enforced throughout the final manuscript.

### 2.2 Coboundary and projector indexing

Status: `PATCH_REQUIRED`.

Use consistently:

- fixed carrier: `D_0`, `P_ex`, `P_perp`;
- changing carrier: `D_{0,-}`, `D_{0,+}`, `P_{ex,-}`, `P_{ex,+}`, `P_{perp,-}`, `P_{perp,+}`.

Avoid mixed forms such as `D_0^-` and `P_{{ex},+}`.

### 2.3 Moore–Penrose pseudoinverse

Status: `HIGH_PRIORITY_PATCH`.

Current Pass 04 writes `L_-^+` for the Moore–Penrose pseudoinverse while `+` is also the post-carrier marker.

Replace by

`L_-^\dagger`.

Then

`R_eff^-(u,v)=b_e^T L_-^\dagger b_e`.

Prefer eventually `R_{eff,-}(u,v)` if the manuscript adopts carrier labels exclusively as subscripts.

### 2.4 `S` namespace

Status: `PARTIALLY_RESOLVED`.

The earlier collision between source `S` and the defect insertion map has already been fixed by Pass 04:

- provenance source field: `S_T`;
- defect insertion: `iota_F`.

Further cleanup recommended: do not introduce a second scalar symbol `S_birth^rel` unless needed. State instead:

> `For an integrable ancestor, the restricted relative birth source equals R_+.`

This keeps `S_T` as the sole mathematical object named `S` in the manuscript.

### 2.5 Update-map symbol `F_G`

Status: `PATCH_REQUIRED`.

Pass 05 uses `F_G` for an autonomous update map immediately after Pass 04 uses `F` for the set of newly born edges.

Rename the update map to

`U_G`

(or `mathcal U_G` in LaTeX).

Then use `U_lambda`, `U_O` for the witness families.

This eliminates a cross-section symbol collision.

### 2.6 Orthogonal group notation

Status: `PATCH_RECOMMENDED`.

Instead of `O(beta_1)` without first naming the dimension, write

`b := beta_1(G)`

and then `O(b)`, or say `orthogonal transformations of ker(D_0^T)`.

The latter is basis-independent and semantically strongest.

### 2.7 Equal-`R` level-set notation

Status: `PATCH_RECOMMENDED`.

The drafts use `M_R` for a level set while the structural magnitude is already calligraphic `R`. To reduce visual overload, use

`M_c := {eta : R(eta)=c}`, `c>0`,

or retain `M_R` only after explicitly declaring `R` as a scalar level value. Preferred: `M_c`.

### 2.8 Root and child symbols in provenance tree

Status: `PATCH_RECOMMENDED`.

Pass 03 uses root `a` and child `c`, while the integrability example and scale-rescaling discussion also use `a`, `b`, `c` as scalar values/constants.

Use:

- root `v_*`;
- generic child `w`;
- parent `p(v)`.

This removes unnecessary symbol recycling.

### 2.9 Triangle-example edge values

Status: `PATCH_RECOMMENDED`.

The minimal example uses `a,b,c` while `c>0` is also the common rate-rescaling factor. For a manuscript whose purpose is conceptual clarity, use `x,y,z` for the three CAL edge values and retain `c>0` for common scale if needed.

### 2.10 Technical `provenance` versus editorial provenance

Status: `HIGH_PRIORITY_SEMANTIC_PATCH`.

The new canonical LQTA-T terminology reserves `provenance/history` for realized historical/precedence structure. Pass 06 currently uses the editorial phrase:

- `Reproducibility and claim provenance`
- `claim-provenance map`

and Pass 05 ends with `preserve this no-go as a provenance statement`.

These are now ambiguous.

Replace by:

- `Reproducibility and claim lineage`;
- `claim-lineage map`;
- `preserve this no-go as a derivational boundary` or `as part of the scientific claim lineage`.

Technical event provenance remains `provenance`.

### 2.11 `cooperation`

Status: `PASS`.

Repository search found no `cooperat*` occurrence in the Article-3 repository. No patch is needed. The term remains deprecated as an autonomous technical category according to the harmonized LQTA-T glossary.

### 2.12 `kappa` cross-article collision

Status: `REVIEW_BEFORE_FREEZE`.

Article 2 already uses

`kappa_Omega(Q)`

for collaborative reconstructibility. Article 3 uses `kappa_e` / vector `kappa` for the cycle-birth defect.

There is no within-manuscript ambiguity if Article 3 never invokes collaborative complexity, and the frozen Article-3 audits use `kappa` for the defect. Therefore no forced change is recommended.

However, for series-wide notation hygiene, the final manuscript should choose one of two policies:

A. Preserve `kappa_e` and add a one-line warning in the first defect definition that it is unrelated to Article-2 collaborative complexity; or

B. Rename the manuscript-level defect to `delta_e^{CAL}` while recording in the claim-lineage appendix that the frozen audits denote it by `kappa_e`.

Preferred for reproducibility: A, unless the final cross-article notation audit finds the collision too costly.

---

## 3. Mathematical wording precision

### 3.1 `exact and coexact`

Status: `PATCH_REQUIRED`.

Pass 06 says:

> `Exact and coexact decompositions belong to finite cochain and Hodge theory.`

The Article-3 construction on a graph uses the orthogonal splitting of edge cochains into the exact subspace `im D_0` and its orthogonal cycle/divergence-free complement `ker D_0^T`. No 2-cell coboundary/coexact sector is part of the present graph-only setup.

Replace by:

> `Exact/cycle orthogonal decompositions belong to finite cochain and graph-Hodge theory.`

or

> `Orthogonal decomposition into exact and cycle components is standard finite graph-Hodge theory.`

This is a terminology precision patch, not a theorem change.

### 3.2 STOP theorem: full CAL versus memory update

Status: `THEOREM_WORDING_TIGHTENING`.

Pass 05 proves nonuniqueness by constructing maps on `eta`, but the theorem title says no unique autonomous CAL generator. The implication is valid, but should be made explicit.

Strengthen the proof by fixing the exact component `D_0 phi` and defining full witness updates

`gamma = D_0 phi + eta -> gamma' = D_0 phi + U(eta)`.

Since multiple inequivalent `U` remain admissible even with the exact component held fixed, a fortiori the frozen theory cannot determine a unique full CAL generator.

This is a stronger presentation of the same no-go; no scientific result changes.

### 3.3 Provenance continuity applicability

Status: `PATCH_RECOMMENDED`.

In the STOP proof, replace unconditional wording that provenance continuity `applies` after any witness by:

> `If the realized event is supplied with a provenance tree, the provenance-conditioned continuity theorem then applies to its resulting Delta rho.`

This preserves the conditional nature of the provenance construction.

---

## 4. Canonical notation dictionary for final integration

| Object | Final notation | Scope |
|---|---|---|
| CAL carrier | `G=(V,E)` | fixed support |
| edge cochain | `gamma in C^1(G;R)` | fixed support |
| coboundary | `D_0` | fixed support |
| vertex potential | `phi` | exact sector |
| local recalibration | `q` | gauge parameter |
| exact projector | `P_ex` | fixed support |
| non-exact projector | `P_perp` | fixed support |
| non-exact state | `eta=P_perp gamma` | memory configuration |
| cycle period | `Pi_C(gamma)` | gauge-invariant cycle datum |
| cycle rank | `beta_1(G)` | `dim ker D_0^T` |
| local allocation | `rho_i` | derived from `eta` |
| total structural magnitude | `Rcal` | `||eta||^2` |
| fixed before/after | superscripts `-`,`+` | same carrier only |
| provenance tree | `T=(V_T,E_T)` | realized history |
| provenance root | `v_*` | tree root |
| current | `J_T` | provenance-conditioned |
| provenance divergence | `div_T` | rooted tree |
| source field | `S_T` | rooted tree |
| changing carriers | `G_-`,`G_+` | distinct cochain spaces |
| changing-support coboundaries | `D_{0,-}`,`D_{0,+}` | carrier-indexed |
| changing-support projectors | `P_{perp,-}`,`P_{perp,+}` | carrier-indexed |
| new-edge set | `F` | support birth |
| defect insertion | `iota_F` | `R^k -> C^1(G_+;R)` |
| defect Gram/quadratic matrix | `K_F` | support birth |
| cycle-birth defect | `kappa_e` (provisional) | ancestor-anchored |
| graph Laplacian | `L_-` | old carrier |
| pseudoinverse | `L_-^dagger` | Moore–Penrose |
| effective resistance | `R_eff,-(u,v)` | graph-theoretic only |
| autonomous witness map | `mathcal U_G` | STOP theorem |

---

## 5. Recommended final section order

To satisfy concept-before-use as strongly as possible:

1. Introduction
2. Finite relational setup and discrete temporal ontology
3. Integrability and derived local rates
4. Cycles, holonomy, and collective temporal memory
5. Realized changes, provenance, and structural continuity
6. Fixed-carrier transition classes
7. Changing relational support
8. Restricted support-change defect algebra
9. Boundary of endogenous dynamics / STOP theorem
10. Synthetic interpretation and scope
11. Reproducibility and claim lineage
12. Conclusion
13. Appendices / claim-lineage table / witnesses

This order ensures that:

- `beta_1`, `rho`, `Rcal` are defined before transition use;
- `S_T` is defined before `source-positive/negative` terminology;
- cross-carrier notation is introduced only after fixed-carrier arithmetic is complete;
- the STOP theorem refers only to already-established constraints;
- the Discussion uses no new technical object.

---

## 6. Scientific impact

All findings are editorial or notational.

Unchanged:

- local-rate reconstruction theorem;
- homogeneous reduction;
- cycle criterion;
- tree rigidity;
- memory-sector dimension;
- `rho_i` and `Rcal` definitions;
- fixed-carrier transition identity;
- provenance-conditioned continuity theorem;
- global balance;
- bridge/cycle-birth distinction;
- ancestor-anchored defect law;
- positivity of `K_F`;
- single-edge effective-resistance law;
- zero-new-period nonintegrable-parent counterexample;
- no-go against unique endogenous autonomous dynamics;
- all frozen analytic/computational audits.

No rerun is required.

## Final recommendation

`GO_TO_INTEGRATION_WITH_GLOBAL_NOTATION_PATCH`

After integration, perform one final mechanical/visual LaTeX audit for undefined references, duplicate labels, typography, equation numbering, and compilation warnings before generating the first referee-readable PDF.