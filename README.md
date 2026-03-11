# General Langlands Functoriality via Transfer-Packet Persistence
## Canonical Lane (defined term): the manifold-constrained local-to-global transfer super-architecture (`GLF1-GLF8`)

Canonical Lane super-repo for a flagship umbrella problem in automorphic forms, Galois representations, and the Langlands program:
proving persistence of admissible transfer packets across L-group morphisms through a multi-lane transfer super-architecture.

## Main Manuscript

- [paper/GENERAL_LANGLANDS_FUNCTORIALITY_PREPRINT.md](paper/GENERAL_LANGLANDS_FUNCTORIALITY_PREPRINT.md)
- [paper/CANONICAL_ROUTING_INDEX.md](paper/CANONICAL_ROUTING_INDEX.md)

## Super-Repo Role

This repository is not a single primitive transfer case. It is the coordinating functoriality lane for an admissible transfer lattice whose native sub-lane families are:

1. cyclic base change,
2. automorphic induction,
3. endoscopic and stable transfer,
4. tensor/Rankin-Selberg transfer,
5. symmetric and exterior power transfer.

The runtime surface certifies closure of the declared super-lane, not just one isolated transfer example.

## Structure

- `paper/`
  - `GENERAL_LANGLANDS_FUNCTORIALITY_PREPRINT.md`
  - `CANONICAL_ROUTING_INDEX.md`
  - `EXTRACTION_SPEC.md`

- `notes/`
  - `EG1_public.md`
  - `EG2_public.md`
  - `EG3_public.md`
  - `EG4_public.md`
  - `IDENTIFICATION_BRIDGE.md`

- `repro/`
  - `REPRO_PACK.md`
  - `THIRD_PARTY_RERUN_PROTOCOL.md`
  - `run_repro.sh`
  - `repro_manifest.json`
  - `certificate_baseline.json`

- `scripts/`
  - `glf_closure_guard.py`
  - `extract_constants.py`
  - `promote_constants.py`
  - `update_manifest.py`
  - `release_gate.py`
  - `README.md`

- `artifacts/`
  - `constants_extraction_inputs.json`
  - `constants_extracted.json`
  - `constants_registry.json`
  - `stitch_constants.json`
  - `promotion_report.json`

## Local Reproducibility Command

```bash
bash repro/run_repro.sh
```

This writes `repro/certificate_runtime.json`.

## How To Read This Professionally

1. Super-lane theorem chain first: read `paper/GENERAL_LANGLANDS_FUNCTORIALITY_PREPRINT.md`.
2. Transfer-lattice routing second: audit `paper/CANONICAL_ROUTING_INDEX.md` and the note layer.
3. Constants provenance third: audit `paper/EXTRACTION_SPEC.md`, `artifacts/constants_extraction_inputs.json`, `artifacts/constants_extracted.json`, and `artifacts/promotion_report.json`.
4. Pipeline fourth: run `bash repro/run_repro.sh` to audit hashes, provenance, and gates; it is reproducibility infrastructure, not theorem generation.

Release modes:

- `normalized`: `status=normalized_placeholder` allowed when explicitly labeled.
- `fully_extracted`: requires `status=derived_numeric` for all required constants and stitch keys.

Current GLF runner policy:

- `repro/run_repro.sh` extracts, promotes, runs `scripts/glf_closure_guard.py`, updates `repro/repro_manifest.json`, and enforces `fully_extracted` release-gate mode.

## Routing Rule (inclusion discipline)

Every claim-bearing item must be routed through all three layers:

1. main preprint section/appendix,
2. mirror note under `notes/`,
3. artifact key consumed by `scripts/glf_closure_guard.py`.

Routing map: [paper/CANONICAL_ROUTING_INDEX.md](paper/CANONICAL_ROUTING_INDEX.md)

## Citation

- Metadata: [CITATION.cff](CITATION.cff)
- Manuscript target: [paper/GENERAL_LANGLANDS_FUNCTORIALITY_PREPRINT.md](paper/GENERAL_LANGLANDS_FUNCTORIALITY_PREPRINT.md)

## Authorship

- Program author: **HautevilleHouse**
- Canonical attribution source: [`CITATION.cff`](CITATION.cff)
