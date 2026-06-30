# Evaluation Protocol

The evaluation uses five requirement-version pairs. Each pair contains a baseline requirement and a revised requirement for the same scenario. The tool generated two types of artifacts for each text: a triple graph in JSON and an ontology-compatible graph in Turtle.

The evaluation addressed three questions:

1. How faithful and complete are raw LLM-generated triples before human curation?
2. What types of semantic gaps does human curation address?
3. To what extent does OntologyWeb's graph comparison surface human-identified requirement changes?

A primary evaluator created proposed reference changes, raw triple audit labels, and curated correction structures. Two additional evaluators then reviewed 128 row-level judgments in structured workbooks. Direct agreement was 124/128 and 126/128, respectively. Exceptions were accepted or resolved through adjudication and incorporated into the final labels.

Because the second-stage workbooks were confirmation reviews of proposed labels rather than blind independent coding from scratch, the paper reports row-level agreement and adjudicated exceptions rather than Cohen's kappa.
