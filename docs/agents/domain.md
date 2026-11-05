# Domain Docs

This repository uses a single-context layout.

## Before exploring

Read `GLOSSARY.md` at the repository root and relevant decisions in `docs/adr/`.

If these files do not exist, proceed silently. Do not suggest creating them
upfront. The domain-modeling skill creates them as terms and decisions
are resolved.

## File structure

- `GLOSSARY.md`: repository-wide domain vocabulary.
- `docs/adr/`: repository-wide architecture decision records.

## Use the glossary's vocabulary

Use glossary terms in issue titles, proposals, hypotheses, and test names.
Avoid synonyms the glossary explicitly rejects.

If a needed concept is missing, reconsider whether the project uses it.
Record genuine vocabulary gaps for domain modeling.

## Flag ADR conflicts

Explicitly identify proposals that contradict an existing ADR and explain
why the decision should be revisited.
