# LQTA-D Article 3 — Literature Expansion Audit v0.1

Date: 2026-08-16
Scope: recent and conceptually adjacent literature for Article 3.
Goal: expand bibliography and sharpen neighboring-work discussion without changing scientific claims.

## Global verdict

`EXPAND_BIBLIOGRAPHY_AND_NEIGHBORING_WORK_DISCUSSION`

The current bibliography is too sparse for the maturity of the manuscript. The mathematical backbone is adequately anchored by Whitney, discrete exterior calculus, Hodge ranking, graph Hodge Laplacians, synchronization, and connection Laplacians, but the 2021–2026 literature now contains several much closer references.

No scientific claim needs to be reopened. The main change is to situate LQTA-D more precisely among three literatures:

1. cycle consistency / synchronization / holonomy;
2. graph-Hodge and changing-support Laplacian methods;
3. relational clock and finite-history formalisms.

## Tier A — references that should be added

### A1. Torres-Hugas, Duch, Gómez, Arenas (2026)

**Cycle holonomy captures higher-order compatibility constraints in remote synchronization**, arXiv:2604.19682v2 (2026).

Why it is close:
- edge data carry a gauge structure;
- accumulation around cycles gives gauge-invariant holonomy;
- global compatibility is equivalent to vanishing cycle holonomies;
- nonzero holonomy is interpreted as a local-to-global obstruction/frustration.

Why it is not the same theory:
- it is a dynamical phase/synchronization model with a U(1)-valued connection and twisted Laplacian;
- LQTA-D uses a real additive CAL 1-cochain on a finite relational carrier and interprets exactness as existence of a complete local-rate representation;
- LQTA-D additionally includes provenance-conditioned accounting, changing-support defect laws, and an explicit endogenous-dynamics no-go.

Recommended use: mandatory citation in the Introduction or Discussion immediately after the synchronization references. This is currently the closest mathematical neighbor to the cycle-holonomy/integrability sector.

### A2. Churilov (2026)

**Finite Quantum Histories: Holonomy Spectra, Minimal Clocks, and Exact Clock-Change Covariance**, arXiv:2608.05748 (2026).

Why it is close:
- finite histories and clocks;
- connection-Laplacian formulation on a cycle;
- monodromy/holonomy is the complete gauge invariant of the cyclic unitary history;
- exact relational history is controlled by the holonomy/monodromy sector;
- explicit discussion of finite clocks and clock changes.

Why it is not the same theory:
- quantum, unitary, finite-dimensional history states on a cyclic clock register;
- gauge invariant is non-Abelian/unitary monodromy rather than an additive real CAL cochain;
- restricted to cyclic history architecture rather than arbitrary relational support with births/deaths;
- does not contain LQTA-D's local-rate reconstruction theorem, provenance current, ancestor-anchored CAL birth defect algebra, or structural STOP theorem in the same form.

Recommended use: mandatory citation as the nearest conceptual finite-clock/holonomy neighbor. Because it appeared in August 2026, it should be discussed explicitly rather than buried in a bibliography list.

### A3. Mémoli, Wan, Wang (2022)

**Persistent Laplacians: Properties, Algorithms and Implications**, SIAM Journal on Mathematics of Data Science 4(2) (2022), DOI 10.1137/21M1435471.

Why it is close:
- treats Laplacian structure across inclusions of complexes;
- links persistent Laplacians to persistent Betti numbers;
- in the graph case gives a connection to effective resistance;
- relevant mathematical neighbor for changing relational support and the single-edge effective-resistance coefficient.

Why it is not the same theory:
- persistence is a topological/data-analysis construction, not a temporal CAL ontology;
- LQTA-D explicitly refuses to identify pre/post cochain spaces without endogenous structure and derives only restricted cross-support source statements.

Recommended use: mandatory citation in the changing-support/effective-resistance discussion.

### A4. Li, Shi, Lerman (2024)

**Efficient Detection of Long Consistent Cycles and its Application to Distributed Synchronization**, Proc. IEEE/CVF CVPR 2024, pp. 5260–5269.

Why it is close:
- cycle consistency is treated as decisive for global synchronization;
- long cycles are used as explicit consistency constraints;
- provides a modern reference beyond the classical synchronization papers already cited.

Why it is not the same theory:
- computational group synchronization/vision setting;
- no temporal interpretation of an additive CAL field;
- no provenance or support-change physics.

Recommended use: cite with Singer/Bandeira when discussing cycle consistency and synchronization.

### A5. Chataignier, Hoehn, Lock, Mele (2026; preprint 2024)

**Relational Dynamics with Periodic Clocks**, New Journal of Physics 28, 034504 (2026), DOI 10.1088/1367-2630/ae46d0.

Why it is close:
- explicit relational dynamics relative to clocks;
- distinguishes clock-relative descriptions and gauge-invariant relational observables;
- treats periodic clocks and the limitations of clock descriptions.

Why it is not the same theory:
- Hamiltonian-constraint / classical-and-quantum relational-observable framework;
- periodic clock dynamics rather than finite graph CAL integrability;
- no graph holonomy memory sector of the LQTA-D type.

Recommended use: mandatory conceptual citation in Introduction/Discussion when positioning local-clock completeness versus broader relational-time approaches.

## Tier B — strong supporting references

### B1. Hoehn, Smith, Lock (2021)

**The Trinity of Relational Quantum Dynamics**, Physical Review D 104, 066001 (2021), DOI 10.1103/PhysRevD.104.066001.

Use: relational clocks, clock-neutral/gauge-invariant descriptions, change of temporal reference frames.

Role: conceptual context, not mathematical antecedent for the CAL cochain theorem.

### B2. Giacomini (2021)

**Spacetime Quantum Reference Frames and superpositions of proper times**, Quantum 5, 508 (2021), DOI 10.22331/q-2021-07-22-508.

Use: operational/relational role of physical clocks and proper-time reference frames.

Role: conceptual clock literature; cite sparingly because LQTA-D is not quantum and does not assume spacetime.

### B3. Hoppe and Schaub (2024)

**Representing Edge Flows on Graphs via Sparse Cell Complexes**, Proceedings of Machine Learning Research 231 (2024), pp. 1:1–1:22.

Use: modern graph-Hodge decomposition of edge flows into gradient/curl/harmonic components.

Role: mathematical context for edge-cochain decompositions. LQTA-D should still use `exact/cycle` language rather than importing higher-cell curl semantics that are absent from the graph-only sector.

### B4. Grigor'yan, Lin, Yau, Zhang (2025)

**Eigenvalues of the Hodge Laplacian on digraphs**, Communications in Analysis and Geometry 33(4), 981–1023 (2025), DOI 10.4310/CAG.250815152654.

Use: recent rigorous Hodge-Laplacian work on directed graphs.

Role: useful recent mathematical citation if the journal referee asks for post-2020 Hodge literature; less directly relevant than A1/A3/A4.

### B5. Lin, Wan, Zhang (2024)

**Connection Laplacian on discrete tori with converging property**, arXiv:2403.06105 (2024).

Use: modern connection-Laplacian spectral literature; holonomy/twist structure on discrete tori.

Role: optional; relevant mainly to the connection-Laplacian neighborhood, not necessary for the core LQTA-D argument.

## Nearest-neighbor ranking

### Closest mathematically

1. Torres-Hugas et al. (2026): cycle holonomy + gauge + global compatibility obstruction.
2. Li, Shi, Lerman (2024): cycle consistency + global synchronization.
3. Mémoli, Wan, Wang (2022): changing support + Laplacian/effective-resistance relation.
4. Hoppe and Schaub (2024): modern Hodge edge-flow decomposition.

### Closest conceptually in temporal physics

1. Churilov (2026): finite histories + clocks + holonomy/monodromy + exact-history sector.
2. Chataignier et al. (2026): relational dynamics relative to clocks.
3. Hoehn, Smith, Lock (2021): gauge-invariant relational dynamics and temporal reference frames.
4. Giacomini (2021): operational spacetime quantum reference frames/proper times.

## Main originality boundary after the search

The recent literature removes any basis for presenting the following ingredients as unusual by themselves:

- local-to-global consistency controlled by cycles;
- gauge-invariant cycle holonomy as an obstruction;
- Hodge/connection-Laplacian decompositions of edge data;
- relational clock descriptions without a single external clock;
- effective-resistance coefficients in graph-Laplacian identities.

What remains distinctive in the current LQTA-D article is the particular constrained assembly:

- real additive CAL temporal-scale comparison as the primitive edge datum;
- exact iff complete representation by derived positive local rates;
- non-exact CAL remainder interpreted narrowly as collective temporal memory;
- provenance-selected current for realized changes without promoting it to a generator;
- explicit firewall between fixed-carrier and changing-carrier vector differences;
- bridge versus cycle birth and ancestor-anchored defect algebra;
- restricted positive birth law from an integrable ancestor;
- explicit counterexample preventing extension to a general nonintegrable parent;
- final no-go showing that the frozen structure does not select a unique autonomous CAL dynamics.

No searched source was found that combines this whole package. This is not a novelty proof; it is a literature-positioning result.

## Recommended manuscript changes

### Introduction

Add one short paragraph after the existing synchronization paragraph:

> Recent work sharpens two neighboring directions. In synchronization theory, cycle holonomy has been shown to encode gauge-invariant local-to-global compatibility obstructions, while modern cycle-consistency methods continue to use closed-loop constraints to determine global synchronizability. Separately, relational-clock formalisms study dynamics relative to internal clocks and temporal reference frames, including periodic clocks and finite quantum histories. The present construction differs in treating a real additive CAL comparison cochain on a finite relational carrier and asking first whether the relational state admits any complete positive local-rate representation.

Citations: Torres-Hugas et al.; Li-Shi-Lerman; Hoehn-Smith-Lock; Chataignier et al.; Churilov.

### Changing support

Add Mémoli-Wan-Wang near the first discussion of changing support/effective resistance, with wording that persistent Laplacians provide a mathematical neighboring treatment of Laplacians across nested complexes and connect to effective resistance, but are not being used here as a physical cross-carrier identification.

### Discussion / neighboring mathematics

Expand the existing paragraph into three sentences:

1. graph-Hodge / edge-flow decomposition references;
2. synchronization / cycle-holonomy references;
3. relational-clock / finite-history references.

Then state explicitly that these literatures overlap with different pieces of LQTA-D but do not supply the whole model-specific assembly.

## Recommended bibliography additions for the next manuscript patch

Minimum set (7 additions):

1. P. A. Hoehn, A. R. H. Smith, and M. P. E. Lock, Phys. Rev. D 104, 066001 (2021).
2. F. Giacomini, Quantum 5, 508 (2021).
3. F. Mémoli, Z. Wan, and Y. Wang, SIAM J. Math. Data Sci. 4(2) (2022), DOI 10.1137/21M1435471.
4. S. Li, Y. Shi, and G. Lerman, Proc. CVPR 2024, 5260–5269 (2024).
5. L. Chataignier, P. A. Hoehn, M. P. E. Lock, and F. M. Mele, New J. Phys. 28, 034504 (2026).
6. L. Torres-Hugas, J. Duch, S. Gómez, and A. Arenas, arXiv:2604.19682v2 (2026).
7. M. V. Churilov, arXiv:2608.05748 (2026).

Extended set: add Hoppe-Schaub (2024) and Grigor'yan-Lin-Yau-Zhang (2025).

## Recommendation

`GO_BIBLIOGRAPHY_EXPANSION_BEFORE_REFEREE_PASS`

The most important change is to cite and discuss the two 2026 papers explicitly. They materially improve the intellectual positioning of Article 3 and reduce the risk that a referee perceives the manuscript as unaware of very recent cycle-holonomy or finite-clock literature.