# Annotation Schema

## Reference-change detection labels

- `detected`: the graph comparison surfaces the core version-level change and its main qualifying semantics.
- `partial`: the graph comparison surfaces a change-specific actor, action, artifact, or ontology vocabulary item, but misses important conditions, preconditions, scope, exception, or timing semantics.
- `missed`: the comparison does not surface the version-level change. Generic vocabulary or actions common to both versions are not sufficient.

## Raw triple audit labels

Correctness / faithfulness:

- `yes`: the generated structure is supported by the source text.
- `partial`: the generated structure is related to the text but has an under-specified or imperfect subject, predicate, object, or role.
- `missing`: the relevant critical structure is absent.

Completeness / coverage:

- `complete`: the structure covers the relevant source semantics.
- `partial`: the structure is locally faithful but misses conditions, timing, scope, exception, or other qualifiers.
- `missing`: the relevant semantics are absent.

Curation actions:

- `accept`: keep as-is.
- `keep_and_extend`: preserve a faithful structure but add missing qualifiers.
- `edit_and_extend`: revise an underspecified or imperfect structure and add missing semantics.
- `add_missing`: add a missing condition, event, relation, or constraint.
