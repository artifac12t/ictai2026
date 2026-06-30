# OntologyWeb ICTAI 2026 Evaluation Artifact

This repository contains the evaluation artifact for **OntologyWeb: A Human-in-the-Loop Tool for LLM-Assisted Triple and Ontology-Compatible Graph Curation**.

## What is included

- `data/requirement_pairs/`: five baseline/current requirement-version pairs used in the evaluation.
- `data/generated_graphs/`: generated triple-graph JSON files for each text.
- `data/generated_ontologies/`: generated ontology-compatible Turtle (`.ttl`) files for each text.
- `data/comparison_screenshots/`: screenshots of triple and ontology comparison views where available.
- `docs/screenshots/`: representative screenshots of the OntologyWeb prototype interface.
- `results/adjudicated/`: final adjudicated reference changes, raw triple audit labels, and curated correction structures.
- `results/summary/`: paper-ready summary tables, including reference-change detection, raw-triple audit counts, and error/gap taxonomy.
- `review/`: anonymized evaluator agreement summaries and adjudicated exceptions. Raw evaluator workbooks are not included in the public artifact.
- `docs/`: evaluation protocol, annotation schema, adjudication notes, and data dictionary.

## Final evaluation snapshot

- Requirement-version pairs: 5
- Requirement texts: 10
- Human-verified reference changes: 35
- Final raw-triple audit items after adjudication: 46
- Curated correction structures: 46
- Triple comparison: 12 detected, 19 partial, 4 missed
- Ontology comparison: 1 detected, 30 partial, 4 missed
- Evaluator confirmation review: 124/128 and 126/128 direct row-level agreement; all exceptions adjudicated.

## Tool code availability

This repository focuses on the evaluation data, generated graph files, adjudicated labels, summary tables, and documentation for the OntologyWeb ICTAI 2026 evaluation. The related OntologyWeb tool source code may be released separately after the code repository is cleaned and reviewed according to the applicable project, institutional, and policy requirements.

## Suggested use

Start with [`docs/screenshots/README.md`](docs/screenshots/README.md) for a visual overview of the system interface and comparison workflow.

1. Start with `docs/evaluation_protocol.md` and `docs/annotation_schema.md` to understand the labeling protocol.
2. Inspect `data/requirement_pairs/` together with the generated JSON and TTL files under `data/generated_graphs/` and `data/generated_ontologies/`.
3. Use `results/adjudicated/` for the final labels used in the paper.
4. Use `results/summary/` for the paper-level aggregate tables.
5. Use `review/` to inspect the anonymized evaluator agreement summary and adjudicated exceptions.

## Summary tables

The aggregate summary tables used in the paper are provided directly under `results/summary/`. They are derived from the adjudicated CSV files in `results/adjudicated/` and the anonymized evaluator-review files in `review/`.
