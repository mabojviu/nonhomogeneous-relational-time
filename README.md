# Nonhomogeneous Relational Time

### Structural and kinematic physics from finite relational event networks

**LQTA-D — Article 3 pre-synthesis repository**

Version `0.1.0`

Zenodo DOI: `10.5281/zenodo.21959348`

> Local clocks describe relational time only when scale comparison is globally integrable; once redundant relations carry nontrivial holonomy, temporal structure becomes collective and cannot be reduced to properties of individual clocks.

---

## Status

`READY_FOR_SYNTHESIS_AS_STRUCTURAL_KINEMATIC_THEORY__NOT_AUTONOMOUS_DYNAMICS`

This release freezes the scientific state of the **nonhomogeneous relational-time branch of LQTA-D** immediately before editorial synthesis into Article 3.

It is **not** the Article 3 manuscript.

It is a reproducible research snapshot containing the chain of mathematical audits, adjudications, no-go results, and the synthesis blueprint on which that manuscript will be based.

## Scope

The frozen branch starts from the already-closed homogeneous clock sector with a common metrological calibration `r0` and develops a nonhomogeneous theory in which local scale comparison is relational.

The central hierarchy is:

1. homogeneous sector: `gamma = 0`, with common calibration `r0`;
2. integrable nonhomogeneous sector: `gamma_ij = log(r_j/r_i)`, where the `r_i` are **derived** representatives;
3. nonintegrable sector: `gamma = D0 phi + eta`, where `eta` is not representable by any global family of local rates;
4. `Rho = ||eta||^2` measures the nonintegrable CAL component relative to the frozen cochain inner product;
5. realized fixed-carrier changes admit exact source classification and provenance-selected balance bookkeeping;
6. support changes distinguish bridge birth from cycle birth and yield a gauge-invariant cycle-birth defect `kappa_e`;
7. from an integrable ancestor, multiple support-birth defects obey a positive quadratic law `Rho_after = kappa^T K kappa`;
8. the frozen ontology does **not** select a unique autonomous CAL generator.

## Central interpretation

> Local clocks describe relational time only when scale comparison is globally integrable; once redundant relations carry nontrivial holonomy, temporal structure becomes collective and cannot be reduced to properties of individual clocks.

## Terminology continuity

- `r0` is retained as the common metrological calibration used in the homogeneous article.
- `r_i` is retained for continuity but is **not** a primitive physical field in this branch.
- In the integrable sector, `r_i` is reconstructed from CAL and is unique up to one common positive factor.
- `phi_i = log(r_i/r0)` may be used as an auxiliary logarithmic coordinate.
- Legacy autonomous `r_i/H_i` dynamics are not part of this freeze.

## Main exact results

### Integrability

On a connected CAL carrier:

`gamma exact  <=>  exists r_i > 0 with gamma_ij = log(r_j/r_i)`.

The rates are unique up to `r_i -> c r_i`.

### Nonintegrable memory

`gamma = D0 phi + eta`.

A connected tree has `eta = 0` identically. Cycles are required for irreducible CAL memory.

### Realized-change balance

`Delta rho + div_T J = S`.

This is a closure/bookkeeping law after a realized change. It is not an autonomous equation of motion.

### Support change

For a new internal edge `e=(u,v)` born from an integrable parent:

`kappa_e = gamma'_e - log(r_v/r_u)`.

For multiple births from one integrable ancestor:

`Rho_after = kappa^T K kappa`.

For one unit-weight new edge:

`Rho_birth = kappa_e^2 / (1 + R_eff_old(u,v))`.

`R_eff` is used only as a graph-theoretic coefficient. No electrical interpretation is claimed.

## Firewalls

This release does **not** identify:

- `Rho` with energy or entropy;
- `rho_i` with matter density;
- `J` with a spatial flow;
- CAL support with physical space;
- `R_eff` with physical electrical resistance;
- cycle holonomy with Lorentz curvature;
- source sign with a thermodynamic arrow;
- `kappa` with force;
- the structural theory with an autonomous dynamics.

No spacetime metric, Lorentz symmetry, Hamiltonian, energy law, or autonomous defect dynamics is imported into this branch.

## STOP result

`LQTA-PHYS-0K` shows that the frozen model admits multiple inequivalent update maps compatible with all current structural constraints. Therefore any unique CAL dynamics would require an additional physical selection principle.

The scientific decision is:

**STOP on added autonomous dynamics; GO on Article 3 synthesis.**

## Reproducibility

The complete frozen scientific packages are bound by SHA-256 in the release manifest. Human-readable scientific lineage and the manuscript blueprint are included in the repository; the exact binary freeze is archived under Zenodo DOI `10.5281/zenodo.21959348`.

See:

- `docs/SCIENTIFIC_INDEX.md`
- `docs/DEPENDENCY_GRAPH.md`
- `release/MANIFEST_v0_1.json`
- `release/RELEASE_NOTES_v0_1.md`
- `manuscript/LQTA_ARTICLE_3_SYNTHESIS_BLUEPRINT_v0_1.md`

## Literature posture

Standard mathematical structures used here—graph cochains, Hodge decomposition, synchronization/gain-graph consistency, cycle holonomy, effective resistance identities, and graph-topological birth/death bookkeeping—are treated as antecedent mathematics.

The object frozen here is the **LQTA-D temporal assembly and its endogenous chain of interpretation**, not a claim of ownership over those mathematical ingredients.
