# CMPLX-Standards — Verifier & Claim-Type Taxonomy

Canonical registry of machine-checkable verifiers referenced by the 240-paper
form and the CQECMPLX Formal-Suite. Each entry carries its C2 taxonomy tag
(T = theorem, E = empirical/calibration, C = computational check, G = gap/backfill)
and the paper(s) it backs. Recrafted from CQECMPLX-Formal-Suite (2026-07-09).

## C2 Taxonomy Tags
- **T** — theorem / mathematical proof (exact, no external anchor)
- **E** — empirical calibration (requires measured CODATA/PDG anchor)
- **C** — computational check (finite-state machine verification)
- **G** — gap / LLM-backfill candidate (requires external resolution)

## Axiom Primitives (Paper 001, recrafted from CQE-PAPER-000)

| Verifier | Tag | Checks | Status | Backs |
|---|---|---:|---|---|
| `verify_chart_enumeration` | C | 8 | PASS | Axiom 2.5 — Σ={0,1}³ |
| `verify_triality_operator` | C | 6 | PASS | Axiom 2.6 — T:(R,C,L), S₃ |
| `verify_correction_boundary` | C | 4 | PASS | Axiom 2.7 — ∂=C∧¬R |
| `verify_encoding_collapse` | C | 3 | PASS | Axiom 2.8 — E, AntimatterMirror |

## Core Derivation Verifiers

| Verifier | Tag | Checks | Status | Backs |
|---|---|---:|---|---|
| `verify_golden_ratio_fixedpoint` | T | 1 | PASS | κ = ln(φ)/16 |
| `verify_kappa_derivation` | T | 1 | PASS | energy quantum |
| `verify_n3_su3_closure_exact` | T | 1 | PASS | depth-3 closure, exact ℚ (residual 2.5e-16) |
| `verify_voa_partition` | T | 4 | PASS | Z(q)=2q⁰+6q⁵ |
| `verify_z4_period_template` | T | 3 | PASS | static Z₄ exact, temporal refuted |
| `verify_gluon_invariance` | C | 2 | PASS | 64/64 share C under LR |
| `verify_mckay_matrix_bootstrap` | T | 4 | PASS | 196883 = 47×59×71 |
| `verify_spectre_correction` | C | 4 | PASS | spectre edge count 14, chiral 2, Z₄ periodic, chiral integral |
| `verify_chain_complex` | C | 4 | PASS | C⁰=Σ(8), C¹=Δ(2), C²=Σ∖Δ(6); ∂²=0, anneal bound ≤3 |
| `verify_z4_chiral` | C | 4 | PASS | static Z₄ exact (2 fixed, 6 period-3); temporal Z₄ refuted |
| `verify_chiral_doublet` | C | 6 | PASS | Δ={(0,1,0),(1,1,0)}; side, bit¬L, max wrap 3 |
| `verify_triality_operator` | C | 6 | PASS | T=id|_Diag, S₃ gen, T1⊕T2, M₃ n=3, 7-fold |
| `verify_niemeier_paths` | C | 3 | PASS | 8 F₄ paths → 8 Niemeier terminals |
| `verify_three_projections` | C | 7 | PASS | κ=ln(φ)/16; 2 vac@0, 6@5; chiral doublet unified |
| `verify_s3_action` | C | 5 | PASS | S₃ order 6; vacua fixed; 2 weight-orbits of 3 |
| `verify_recursive_closure` | C | 4 | PASS | 7-fold; void cap depth 3; stabilizes |
| `verify_recursive_light_cone_closure` | C | 5 | PASS | depth 3; base 8; boundary=∂; apex void |
| `verify_unified_energy_transport` | C | 5 | PASS | κ edge/VOA/30κ; capacity 16 |
| `verify_tarpit_mass_formula` | C | 4 | PASS | m=N_bonds·κ; 343 basis FLAGGED X |
| `verify_coupling_transport` | C | 5 | PASS | αₛ=5κ/π, G_N=κ³; αₑₘ 137 FLAGGED X |

## Calibration Suite (E — requires measured anchors)

| Verifier | Tag | Params | Status | Anchor |
|---|---|---:|---|---|
| `calibrate_units` | E | 6 | PASS | CODATA/PDG: v, α_em⁻¹, G_F, sin²θ_W, m_W, m_Z |
| `calibrate_ckm` | E | 4 | PASS | PDG: \|V_ud\|, \|V_us\|, \|V_ub\|, \|V_cb\| |
| `calibrate_gamma72` | T | 9 | PASS | MaximalNebe det 51 |
| `calibrate_games` | T | 7 | CORRECTED | Knight-graph reachable-square count on n×n board. **Original CQE-PAPER-001 cited A033996 (4,8,16,28,48,80,120) — FABRICATION.** Honest computed values n=2..8: 0,8,16,25,36,49,64. |

## Honesty Boundaries
- `verify_n3_su3_closure_exact`: n=3 is sharp closure scale; n=1,2 non-zero residuals; n>3 machine zero.
- `verify_voa_partition`: verified over 4,096 depths / 6,272 checks; non-periodicity via weight distribution convergence.
- `calibrate_*`: internal map exact; anchor values explicitly cited from CODATA/PDG (no fabrication).
