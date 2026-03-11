# Reviewer Map

## Claim Scope

- Canonical-lane claim: inside the `manifold_constrained` transfer lattice, if the theorem chain in this repository holds and the guard certificate passes, the repository-level super-lane closure claim is satisfied.
- Standard target claim: admissible `L`-group morphisms in the declared transfer lattice produce the predicted automorphic endpoint packets with matching local/global observables.
- External-strengthening rule: any statement beyond the admissible class must retain the explicit remainder carried by the defect/coherence ledgers; see `notes/GEOMETRIC_GALOIS_BRIDGE.md`.

## Super-Lane Families

The manuscript treats the following as routed sub-lane families inside one coordinating super-repo:

1. cyclic base change,
2. automorphic induction,
3. endoscopic/stable transfer,
4. tensor and Rankin-Selberg transfer,
5. symmetric/exterior power transfer.

## Theorem Dependency Chain

1. `EG1`: coercive transfer response and active floor.
2. `EG2`: local matching capture across the transfer lattice.
3. `EG3`: compactness and no-collapse spacing for packet towers.
4. `EG4`: rigidity and endpoint transfer.
5. Identification bridge: strict coherence on the determining class.
6. Scalar closure: `GLF_G1, GLF_G2, GLF_G3, GLF_G4, GLF_G5, GLF_G6, GLF_GM` all `PASS`.

Primary files:

- `paper/GENERAL_LANGLANDS_FUNCTORIALITY_PREPRINT.md`
- `notes/EG1_public.md`
- `notes/EG2_public.md`
- `notes/EG3_public.md`
- `notes/EG4_public.md`
- `notes/IDENTIFICATION_BRIDGE.md`
- `notes/GEOMETRIC_GALOIS_BRIDGE.md`

## Closure Gates

| Gate | Constant | Description |
|------|----------|-------------|
| `GLF_G1` | `kappa_transfer` | projected transfer response has a strict positive floor |
| `GLF_G2` | `sigma_matching` | local matching defect stays above capture floor across admissible transfer losses |
| `GLF_G3` | `kappa_compact` | normalized near-failure packet towers are precompact |
| `GLF_G4` | `rho_rigidity` | bad nonfunctorial countermodels are excluded |
| `GLF_G5` | `packet_transfer` | rigid limits transfer to predicted target packets |
| `GLF_G6` | `eps_coh` | strict coherence on the determining class |
| `GLF_GM` | derived | final strict margin |

## Falsification Conditions

- `repro/certificate_runtime.json` has any non-`PASS` gate.
- `lane.active_lane != "manifold_constrained"`.
- `all_pass != true`.
- Any manifest hash mismatch under `repro/repro_manifest.json`.
- A verified counterexample to any routed sub-lane transfer theorem used by the super-repo.
