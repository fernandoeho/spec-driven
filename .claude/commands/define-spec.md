# Define Spec

## Purpose
Transform a requirement into a structured spec that can drive implementation
and test generation.

## Input
The user provides:
- A requirement (user story, feature description, or bug report)
- Optionally: the relevant section of `docs/product.md` for context

## Instructions
You are a senior engineer writing a spec for a junior developer.
Be explicit. Leave no ambiguity.

## Output

Produce a file `specs/<feature-name>.md` with this structure:

### Overview
One paragraph. What this feature does and why it exists.

### Acceptance Criteria
Written as Given/When/Then or bullet assertions.
- [ ] ...
- [ ] ...

### Data Model (if applicable)
Fields, types, constraints.

### API Contract (if applicable)
Method, path, request shape, response shape, error cases.

### Edge Cases & Error Handling
Enumerate explicitly.

### Out of Scope
What this spec deliberately does NOT cover.

### Open Questions
Unresolved decisions that need an answer before implementation starts.
