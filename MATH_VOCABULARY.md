# CMPLX-Standards — Mathematics, Algebra & Calculus Vocabulary

Algebra / calculus referenced by the 240-paper form and CQECMPLX Formal-Suite
that was not previously enumerated in Standards. Recrafted 2026-07-09 from
CQE-PAPER-000..103. These are the formal objects every claim resolves against.

## Primitive Algebra (Σ = {0,1}³)
- **Chart states**: CHART_STATES = 8 triples (L,C,R). TRUE_VACUA={(0,0,0),(1,1,1)}.
- **Chiral doublet**: Δ = {(0,1,0),(1,1,0)} = supp(∂).
- **Lie conjugates**: L=R states {(0,0,0),(0,1,0),(1,0,1),(1,1,1)}.
- **Correction operator**: ∂(L,C,R)=C∧¬R (ANF: C·(1−R)). Nilpotent on {0,1}.
- **Triality**: T(L,C,R)=(R,C,L); fixes diagonal, generates S₃ off-diagonal.

## Energy & Coupling Calculus
- **Golden ratio fixed point**: φ=(1+√5)/2, unique fixed point of depth-3 recursion.
- **Energy quantum**: κ = ln(φ)/16.
- **Mass**: m = N_bonds · κ.
- **Couplings**: α_s = 5κ/π; α_em = κ² sin²θ_W; G_N = κ³.
- **Depth bound**: 3 (exact rational M₃²=M₃, T5 idempotency; residual 2.5e-16).

## Monster / Bijection Decomposition (196883 = 47×59×71)
Total resolution capacity of the Hilbert Light-Cone, split by the three bijections:
- **B₁ (Knights, 47)**: discrete path space. Forward resolution — (3,5) conjugation on genus-2 theta. HilbertLightCone⁺(E). *(NOTE: prior text cited "OEIS A033996" here — FABRICATION; see Calibration Constants.)*
- **B₂ (Jacobian, 59)**: continuous moduli (genus-2). Antipodal pairing — (5,7) adjugation. LightCone⁺(E) → LightCone⁻(E).
- **B₃ (Braiding, 71)**: topological (KZ equations). Closure — KZ monodromy on moduli. LightCone⁻(E) → E.

AntimatterMirror(E) = C\E is the exact counter-expression; I(E)+I(C\E)=I(C).

## VOA & Spectre
- **VOA partition**: Z(q) = 2q⁰ + 6q⁵ (2 vacua weight 0, 6 excited weight 5).
- **Spectre**: ∂ geometric realization; 14 edges, 2 chiralities, 7-fold substitution, depth bound 3, aperiodic (temporal Z₄ refuted).

## Boundary Chain Complex (CQE-PAPER-002 recraft)
- **Complex**: C⁰=Σ (8 states, 0-chains), C¹=Δ (2 chiral states, 1-chains), C²=Σ∖Δ (6 states, 2-chains).
- **Boundary map**: ∂: C⁰→C¹, ∂(s)=C(s)·¬R(s)∈{0,1}, surjective onto Δ, ∂²=0.
- **Anneal bound**: d(σ,vacuum) ≤ 3 for all σ∈Σ (S₃-transposition graph on 8 states has diameter 3). *(NOTE: CQE-PAPER-002 §3.3 per-state anneal table is internally inconsistent and FLAGGED X; honest BFS gives all non-vacua at d=3. See Paper 002 §2.14.)*

## Calibration Constants (exact, no external data)
- Monster scalar: 196883 = 47×59×71 (`verify_mckay_matrix_bootstrap`, 4/4).
- Gamma72 max det: 51 (MaximalNebe) (`calibrate_gamma72`, 9/9).
- OEIS A033996 (Knight CA): **CORRECTED** — the CQE-PAPER-001 claim "n=2..8 → 4,8,16,28,48,80,120 matches A033996" is a FABRICATION (X). Verified count of distinct knight-graph positions on an n×n board is n=2..8 → 0,8,16,25,36,49,64 (OEIS is NOT A033996; the correct sequence for distinct knight-reachable squares differs). `calibrate_games` must report the honest computed values, not the cited A033996 table.
- T5 n=3 residual: 2.5e-16 exact ℚ (`verify_n3_su3_closure_exact`, 1/1).
