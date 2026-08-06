# Changelog

## 0.2.0 — Consolidated Custom GPT Knowledge Pack

Updated the project for the Custom GPT 20-file Knowledge limit.

Changed:
- Added `custom-gpt/knowledge-guidelines.md` as the consolidated legal reasoning and reliability layer.
- Added `custom-gpt/master-reference-index.md` as the consolidated retrieval, special-law, bilingual terminology, and cross-reference layer.
- Updated `custom-gpt/upload-guide.md` so the production GPT uses only the two consolidated project files in Knowledge.
- Updated `README.md` with the current 17-of-20 recommended Knowledge allocation.
- Kept detailed files in `knowledge-guides/`, `indexes/`, `templates/`, and `tests/` as development/source material rather than separate production uploads.
- Reserved three Knowledge slots for future high-value official sources.

### Current production files

Instructions field:
- `custom-gpt/instructions/custom-gpt-instructions.md`

Project-generated Knowledge files:
- `custom-gpt/knowledge-guidelines.md`
- `custom-gpt/master-reference-index.md`

Administrative setup guide:
- `custom-gpt/upload-guide.md`

## 0.1.0 — Foundation

Initial Custom GPT reasoning layer.

Added:
- bilingual Custom GPT instructions;
- upload/update guide;
- conversation starters;
- legal reasoning engine;
- research methodology;
- source hierarchy;
- citation standards;
- output formats;
- criminal-offense framework;
- procedural framework;
- jurisprudence framework;
- hallucination-prevention rules;
- professional standards;
- QA checklist;
- bilingual legal glossary;
- crime cross-reference index;
- constitutional-rights retrieval index;
- initial penalty matrix;
- legal analysis templates;
- regression tests and acceptance checklist.

### Next planned work

- Import and normalize official legal texts into the `knowledge/` folders.
- Expand the penalty matrix from verified current statutes.
- Add article-level crime cross-references.
- Add verified constitutional article mappings.
- Add jurisprudence records from official Tribunal Constitucional and Suprema Corte de Justicia sources.
