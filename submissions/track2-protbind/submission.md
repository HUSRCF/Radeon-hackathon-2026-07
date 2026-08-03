# ProtBind — Track 2 Submission

**Application:** ProtBind

**Track:** Track 2 — Development & Local Deployment of Private AI Agents

**Participant / team:** Huang Siming / ProtBind Team

**Complete source repository:** https://github.com/HUSRCF/hackathon/tree/submission/protbind-amd-devmaster

**Source commit:** `e9f727597765c3ad29406d87aa5ce5ab78196871`

**Demo video:** Pending publication before the final submission deadline

**Project Specification:** [ProtBind_Project_Specification.pdf](ProtBind_Project_Specification.pdf)

**Pitch Deck:** [ProtBind_Pitch_Deck.pptx](ProtBind_Pitch_Deck.pptx)

## Summary

ProtBind is a local-private protein–ligand research agent for staged drug-discovery workflows on
AMD Radeon GPUs and ROCm. Its local LLM runs through HipFire, while typed scientific tools cover
protein and ligand intake, pharmacophore screening, docking preparation, evidence-gated
validation, optional sequence–SMILES concordance annotation, and append-only wet-lab assay
analysis. Sensitive data access and database mutations require explicit, auditable approval.

The submission was validated on an AMD Radeon Pro W7900 (`gfx1100`). A three-repeat local agent
benchmark achieved 100% required-tool success and artifact-citation rates, with 16.552 s p50
end-to-end latency, 9.605 s p50 first-model time-to-first-token, 33.139 p50 end-to-end model
tokens/s, and 7.271 GB observed peak VRAM. The accompanying TriPharm HIP pharmacophore prefilter
has exact complete-score parity with its CPU reference on the frozen three-target evaluation. We
do not claim an end-to-end screening speedup because the current CPU exact finalizer dominates
application latency.

## Deliverables

| Official Track 2 requirement | Location |
| --- | --- |
| Project Specification Document | Attached PDF above |
| Complete source code | Pinned source repository and commit above |
| Environment, dependencies, and startup instructions | Source repository `README.md` and `submission/REPRODUCIBILITY.md` |
| Real Radeon GPU demo video | Link will be inserted above before the deadline |
| PPT or poster | Attached pitch deck above |

The source repository also includes an English claim matrix, demo script, reproducibility guide,
machine-readable benchmark receipts, 454 passing tests, and explicit scientific and licensing
boundaries for optional third-party components.
