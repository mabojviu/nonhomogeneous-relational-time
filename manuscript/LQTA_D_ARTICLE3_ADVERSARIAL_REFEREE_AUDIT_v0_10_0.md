# LQTA-D Article 3 — Adversarial Referee Audit v0.10.0

Date: 2026-08-16
Manuscript: *Nonhomogeneous Relational Time in Finite Event Networks: Integrability, Holonomy, and Collective Temporal Memory*
Audit mode: hostile-but-reasonable mathematical referee; internal consistency, scope, proof sufficiency, terminology, and reproducibility.

## Final verdict after repair

`PASS_WITH_SUBMISSION_LEVEL_CHECKS`

Scientific core: **survives**.
No frozen scientific result was reversed. The audit did, however, identify one genuine scope error in the manuscript-level STOP theorem and several places where the exposition was stronger than the proved statement. All have been repaired in v0.10.0.

## Major findings and repairs

### 1. STOP theorem required a nontrivial cycle sector — repaired

The previous theorem claimed nonuniqueness of the non-exact update map on an arbitrary connected carrier. The radial witness family only proves nonuniqueness when `beta_1(G) >= 1`. On a tree, `ker D_0^T = {0}`, so all memory-update maps satisfying `U(0)=0` coincide on that trivial sector.

The theorem is now explicitly restricted to connected carriers with `beta_1(G) >= 1`. A separate sentence states that the tree sector has no non-exact memory degree of freedom, while the broader ontology still supplies no rule selecting relation births, deletions, or other realized events.

### 2. Gauge representative versus gauge-invariant content — repaired

The manuscript now defines gauge equivalence explicitly by `gamma ~ gamma_tilde` iff their difference lies in `im D_0`. The intrinsic obstruction is the equivalence class modulo exact cochains. The frozen unit inner product selects `eta = P_perp gamma` as the unique orthogonal representative of that class. Homogeneous and strictly nonhomogeneous exact representatives are explicitly identified as belonging to the same zero obstruction class; their distinction is metrological/representational.

### 3. Inner-product dependence of `eta`, `rho`, and `R` — repaired

The manuscript now separates inner-product-independent content (exactness, gauge class, closed-cycle periods) from frozen-inner-product-dependent content (orthogonal representative `eta`, local allocation `rho_i`, and norm `R`).

### 4. Provenance continuity scope — repaired

The branch current is unique only after supplying the realized `Delta rho`, a rooted provenance tree, and the root-source convention. The manuscript now calls root localization a declared accounting convention, not a physical source-localization theorem. The continuity result is stated as a history-conditioned representation whose uniqueness is conditional on those supplied data.

### 5. Single-edge effective-resistance law — proof added

Appendix A now contains a new-edge leverage lemma deriving the single-edge law from `L_+ = L_- + b_e b_e^T`, the rank-one inverse formula on the constant-orthogonal subspace, and the exact projector.

### 6. Cycle criterion — proof added

A path-integration proof now establishes vanishing cycle periods iff exactness.

### 7. Cycle-birth defect proposition — proof added

Gauge invariance and the integrability criterion for `kappa_e` are now demonstrated explicitly.

### 8. Graph assumptions behind `rho_i` — repaired

The carrier is declared finite and loopless; parallel CAL relations may remain distinct edges. Incidence in `rho_i` is explicitly orientation-independent.

### 9. Nested-sector notation — repaired

The hierarchy now uses `subseteq`, because on a tree integrable CAL equals general CAL.

### 10. “Generator” terminology — repaired

User-visible prose now uses **autonomous CAL update law/map**, avoiding the suggestion of an infinitesimal continuous-time generator.

## Additional repairs

- Orthogonal `O` maps are described as state-space degeneracy witnesses, not proposed endogenous laws.
- The support-change section states explicitly that the detailed defect algebra is restricted to relation births with a fixed vertex set.
- The positive-definiteness theorem for `K_F` now refers specifically to the frozen unit edge inner product.
- The empty proof appendix has been replaced by substantive derivations.
- The placeholder claim-lineage appendix has been replaced by an explicit audit-lineage map.
- Introduction, Discussion, and Conclusion were harmonized with the repaired provenance and STOP scopes.

## Residual submission-level checks

These are not scientific blockers:

1. Re-verify final journal/preprint metadata for the newest 2025–2026 references immediately before submission.
2. Ensure the cited status/title of the preceding LQTA-D/T article matches its final public record.
3. Re-check current AIP/JMP wording/location requirements for AI-assisted research disclosure and author declarations at submission time.
4. The compiled PDF has no overfull horizontal boxes or undefined references/citations. The claim-lineage map produces only harmless underfull-box warnings due to narrow cells; visual inspection shows no clipping or overlap.

## Scientific status after audit

`STRUCTURAL_KINEMATIC_CORE_SURVIVES_ADVERSARIAL_REFEREE_AUDIT`

The strongest safe manuscript-level claims are:

- CAL exactness is equivalent to existence of a complete positive local-rate representation.
- The gauge obstruction is captured by cycle periods and, under the frozen inner product, by the orthogonal representative `eta`.
- `R = ||eta||^2` is a gauge-invariant norm of that representative, not an energy or entropy.
- Provenance yields a unique branchwise accounting current only relative to a supplied rooted provenance tree and root-source convention.
- Relation births from a connected integrable ancestor admit an exact positive defect quadratic form and the single-edge effective-resistance law.
- The same defect-local source interpretation does not extend to an arbitrary nonintegrable parent.
- On carriers with `beta_1 >= 1`, the frozen structural ontology does not select a unique autonomous update law for the non-exact CAL state.

## Final recommendation

`GO_TO_SUBMISSION_PREPARATION_AFTER_BIBLIOGRAPHIC_AND_PUBLISHER_POLICY_CHECKS`