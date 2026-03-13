# Generalized Geometric Langlands via Derived-Correspondence Persistence
    ## Canonical Lane (defined term): the manifold-constrained local-to-global super-architecture (`GGL1-GGL8`)

    Canonical Lane super-repo for a flagship umbrella problem in representation theory, algebraic geometry, and categorical sheaf theory:
    proving persistence of admissible derived Hecke correspondences and spectral-side objects through a multi-lane geometric-Langlands super-architecture.

    ## Main Manuscript

    - [paper/GENERALIZED_GEOMETRIC_LANGLANDS_PREPRINT.md](paper/GENERALIZED_GEOMETRIC_LANGLANDS_PREPRINT.md)
    - [paper/CANONICAL_ROUTING_INDEX.md](paper/CANONICAL_ROUTING_INDEX.md)

    ## Super-Repo Role

    This repository is not a single primitive endpoint case. It coordinates an admissible routed lattice whose native families are:

    1. derived Hecke transport and geometric Satake extensions
2. singular-support and spectral-category coherence
3. ramified and stack-level eigensheaf generation
4. categorical duality and kernel transfer
5. local-global stitching across the declared derived packets

    The runtime surface certifies closure of the declared super-lane, not just one local example.

    ## Structure

    - `paper/`
      - `GENERALIZED_GEOMETRIC_LANGLANDS_PREPRINT.md`
      - `CANONICAL_ROUTING_INDEX.md`
      - `EXTRACTION_SPEC.md`

    - `notes/`
      - `EG1_public.md`
      - `EG2_public.md`
      - `EG3_public.md`
      - `EG4_public.md`
      - `IDENTIFICATION_BRIDGE.md`
      - `GEOMETRIC_GALOIS_BRIDGE.md`

    - `repro/`
      - `REPRO_PACK.md`
      - `THIRD_PARTY_RERUN_PROTOCOL.md`
      - `run_repro.sh`
      - `repro_manifest.json`
      - `certificate_baseline.json`

    - `scripts/`
      - `ggl_closure_guard.py`
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

    1. Super-lane theorem chain first: read `paper/GENERALIZED_GEOMETRIC_LANGLANDS_PREPRINT.md`.
    2. Routed-family mapping second: audit `paper/CANONICAL_ROUTING_INDEX.md` and the note layer.
    3. Constants provenance third: audit `paper/EXTRACTION_SPEC.md`, `artifacts/constants_extraction_inputs.json`, `artifacts/constants_extracted.json`, and `artifacts/promotion_report.json`.
    4. Pipeline fourth: run `bash repro/run_repro.sh` to audit hashes, provenance, and gates; it is reproducibility infrastructure, not theorem generation.

    Release modes:

    - `normalized`: `status=normalized_placeholder` allowed when explicitly labeled.
    - `fully_extracted`: requires `status=derived_numeric` for all required constants and stitch keys.

    Current GGL runner policy:

    - `repro/run_repro.sh` extracts, promotes, runs `scripts/ggl_closure_guard.py`, updates `repro/repro_manifest.json`, and enforces `fully_extracted` release-gate mode.

    ## Routing Rule (inclusion discipline)

    Every claim-bearing item must be routed through all three layers:

    1. main preprint section/appendix,
    2. mirror note under `notes/`,
    3. artifact key consumed by `scripts/ggl_closure_guard.py`.

    Routing map: [paper/CANONICAL_ROUTING_INDEX.md](paper/CANONICAL_ROUTING_INDEX.md)
