# Changelog

## 0.3.0 — Legal Reasoning and Quality Upgrade

Strengthened the production Custom GPT without increasing the 17-file Knowledge footprint.

Changed:
- Expanded `custom-gpt/knowledge-guidelines.md` into the consolidated legal reasoning, constitutional/procedural review, conflict-resolution, legal-writing, hallucination-prevention, and response-quality engine.
- Added an explicit exhaustive-source-review workflow so the GPT does not stop at the first relevant article when another authority may modify, supplement, limit, or displace it.
- Added a formal conflict-resolution method for overlapping or inconsistent authorities.
- Added a professional legal-writing standard and structured response-quality standard.
- Strengthened `custom-gpt/instructions/custom-gpt-instructions.md` with exhaustive source review, conflict handling, and clearer separation of substantive criminal law, procedure, constitutional protections, and special legislation.
- Updated `custom-gpt/upload-guide.md` with the v0.3.0 migration procedure.
- Kept the production Knowledge allocation at 17 files; no additional Knowledge slot is required.

### v0.3.0 Custom GPT migration

Replace:
- GPT Instructions field with the latest `custom-gpt/instructions/custom-gpt-instructions.md`.
- Existing `knowledge-guidelines.md` Knowledge file with the latest `custom-gpt/knowledge-guidelines.md`.

Keep:
- `custom-gpt/master-reference-index.md` unless a later commit modifies it.
- Existing official statutes unless they have separately been amended or superseded.

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
