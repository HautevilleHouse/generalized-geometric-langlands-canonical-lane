# Reviewer Map

    ## Claim Scope

    - Canonical-lane claim: inside the `manifold_constrained` routed lattice, if the theorem chain in this repository holds and the guard certificate passes, the repository-level super-lane closure claim is satisfied.
    - Standard target claim: Across the declared admissible correspondence lattice, derived Hecke eigensheaves, spectral-side categories, and stack-level transfer objects persist with the expected compatibility, singular-support control, and local-global endpoint identification.

    ## Super-Lane Families

    1. derived Hecke transport and geometric Satake extensions
2. singular-support and spectral-category coherence
3. ramified and stack-level eigensheaf generation
4. categorical duality and kernel transfer
5. local-global stitching across the declared derived packets

    ## Theorem Dependency Chain

    1. `EG1`: coercive projected response and active floor.
    2. `EG2`: routed-family capture across the declared lattice.
    3. `EG3`: compactness and no-collapse spacing for normalized towers.
    4. `EG4`: rigidity and endpoint transfer.
    5. Identification bridge: strict coherence on the determining class.
    6. Scalar closure: `GGL_G1`, `GGL_G2`, `GGL_G3`, `GGL_G4`, `GGL_G5`, `GGL_G6`, `GGL_GM` all `PASS`.

    ## Falsification Conditions

    - `repro/certificate_runtime.json` has any non-`PASS` gate.
    - `lane.active_lane != "manifold_constrained"`.
    - `all_pass != true`.
    - Any manifest hash mismatch under `repro/repro_manifest.json`.
    - A verified counterexample to any routed family theorem used by the super-repo.
