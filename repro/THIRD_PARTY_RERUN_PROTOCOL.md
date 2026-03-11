# Third-Party Rerun Protocol

1. Clone the repository.
2. Run `bash repro/run_repro.sh`.
3. Confirm that `repro/certificate_runtime.json` reports `GLF_G1` through `GLF_G6` and `GLF_GM` as `PASS`.
4. Confirm that `scripts/release_gate.py --mode fully_extracted` returns `ok = true`.
5. Confirm that all tracked hashes in `repro/repro_manifest.json` match.
6. Read `paper/GENERAL_LANGLANDS_FUNCTORIALITY_PREPRINT.md` with the super-repo interpretation in mind: the declared object is a transfer lattice over admissible `L`-group morphism families.
