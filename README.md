# DOC-1-016 - PET Hydrolases

## Summary (from `DOC-1-016-PET-hydrolases/PROJECT_SUMMARY.md`)


## Status
R2 locked negative/refinement followed by R3 locked structural/register success. The result is a computationally prioritized shortlist, not proof of PET hydrolysis.

## Useful cumulative result
R2 preserved a 20-candidate shortlist after five of seven gates passed; PF12740 family coherence and strict catalytic-triad rules failed, showing that broad motif/domain screening was insufficient. R3 then tested an orthogonal structural hypothesis with ESMFold models, Foldseek-like positive-panel similarity, catalytic-register mapping and triad geometry:
- 20/20 structures completed;
- 20/20 passed the fold leg;
- 19/20 passed fold plus register plus geometry;
- MGYP001374132912 remained a valuable fold-intact/register-destroyed negative.

Adversarial negatives also cross-hit positive structures, so fold similarity alone is explicitly non-specific.

## What is new
The project turns a failed sequence/domain screen into a register-aware structural adjudication. It separates three levels that are often conflated: same fold, plausible catalytic register and plausible triad geometry.

## Why it matters
Polyesterase discovery pipelines can produce large false-positive lists from motif or fold similarity alone. A 19-candidate register/geometry-vetted panel is a stronger, auditable basis for later biochemical testing, while the retained negative demonstrates why the additional leg matters.

## Working tool/application
A PET-hydrolase candidate adjudicator can combine:
- sequence/domain provenance;
- structure prediction confidence;
- positive/adversarial fold matches;
- catalytic-register conservation;
- triad-distance/geometry calibration;
- explicit abstention and failure cards.

It supports experimental prioritization only. It does not claim PET hydrolysis, thermostability, expression, product yield or safety.

## Top-lab reviewer questions
1. Do the 19 candidates hydrolyze PET or model substrates under blinded matched assays?
2. Which register/geometry features predict activity after controlling for fold family?
3. Can a prospective independent metagenome replicate the 19/20 structural pass rate without threshold changes?
4. Do adversarial polyester-adjacent enzymes reveal a more specific substrate-access tunnel or surface signature?

## Next direction
A true next round requires independent replication and substrate-specific discrimination, not another structural rescore of the same 20. Freeze an external candidate panel, adversarial polyesterases and tunnel/electrostatics metrics before outcomes.


## Contents

- `DOC-1-016-PET-hydrolases/` - migrated unchanged from `science-program/projects/DOC-1-016-PET-hydrolases` (32 files)

## Provenance

Split out of the `science-program` repository (source commit `028a7141ed5f951a7b6e6517d4e72768d414a560`) on 2026-09-23. Every file is byte-identical to the source; `MIGRATION_MANIFEST.tsv` lists sha256, original path and new path for each of the 32 files.

Part of Udita Phookan's computational science program: every experiment locks its question, validation design, success gate and failure policy before outcome analysis, and negative results are preserved. Program-wide ledgers and standards live in the `science-program-ledger` repository.
