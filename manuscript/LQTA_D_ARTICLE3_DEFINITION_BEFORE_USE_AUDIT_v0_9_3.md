# LQTA-D Article 3 — Definition-Before-Use Audit v0.9.3

Date: 2026-08-16
Scope: integrated Article 3 manuscript after bibliography expansion.

## Editorial rule

No manuscript-specific symbol, operator, field, source, defect, or derived quantity may be used in a derivation before it has been defined. The Abstract and Introduction may preview concepts in ordinary language, but symbolic preview is kept only when all ingredients are named in the same paragraph.

## Corrections applied in the verified v0.9.3 candidate

1. `C^0(G;R)` and `C^1(G;R)` are explicitly identified as real vertex and edge cochains before use.
2. `D_0` is defined before any decomposition involving `D_0 phi`.
3. The frozen edge inner product is introduced before the orthogonal projectors.
4. `P_ex` and `P_perp` are defined before `eta`.
5. `eta` is now defined constructively by `eta := P_perp gamma`.
6. The exact component is separately defined by `gamma_ex := P_ex gamma = gamma - eta`.
7. `phi` is introduced only after establishing that `gamma_ex` lies in `im D_0`, by choosing `D_0 phi := gamma_ex`.
8. Only after these definitions is the decomposition written:
   `gamma = P_ex gamma + P_perp gamma = D_0 phi + eta`.
   The text explicitly states that this decomposition is derived from the primitive CAL state `gamma`; it is not an independent or self-referential definition of `gamma`.
9. Local recalibration is introduced after `phi` and `eta` exist, so `phi -> phi+q` and `eta -> eta` no longer precede their definitions.
10. Derived rates `r_i := r_0 exp(phi_i)` are defined before their gauge transformation is stated.
11. The formal definition of an integrable CAL state precedes the sector hierarchy.
12. The hierarchy is corrected to the genuinely nested form:
    `homogeneous CAL ⊂ integrable CAL ⊂ general CAL`.
    Strictly nonhomogeneous integrable states are then identified as integrable states with `gamma != 0`.
13. The early triangle example no longer uses `Rcal` before `Rcal` is defined; it reports only `||eta||^2 = delta^2/3`.
14. The provenance source field `S_T` is given its own definition before the continuity equation uses it.
15. The defect quadratic matrix `K_F` is defined before it appears in `Rcal_+ = kappa^T K_F kappa`.
16. The Introduction no longer previews undefined symbols `rho`, `J_T`, `S_T`, `kappa_e`, or `Rcal`; those constructions are described verbally until their formal sections.

## Scientific impact

`NO_SCIENTIFIC_CHANGE`.

The local-rate reconstruction theorem, Hodge/cycle decomposition, provenance continuity result, support-change defect algebra, effective-resistance law, and endogenous-dynamics STOP theorem are unchanged. This is a definition-order and exposition correction only.

## Verification

The v0.9.3 candidate compiles under the existing REVTeX/JMP setup in 20 pages with no undefined citations, no undefined references, no duplicate-label warnings, and no overfull horizontal boxes. The previously known small `Overfull vbox` (~2.43 pt) remains and has no visible clipping in the inspected pages.

## Verdict

`PASS_DEFINITION_BEFORE_USE__GO_TO_FINAL_REFEREE_PASS`