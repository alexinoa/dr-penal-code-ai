# DR Penal Code AI

A bilingual (Spanish/English) legal-research knowledge base for Dominican criminal law. The project is designed to support a Custom GPT grounded in official statutes, amendments, procedural rules, and curated research guides.

## Purpose

The assistant should help users locate and explain Dominican criminal-law provisions, compare prior and current law, identify procedural rules, and produce source-grounded bilingual explanations. It is a legal-information and research tool, not a substitute for representation by a licensed attorney.

## Repository structure

- `custom-gpt/` — short instructions, conversation starters, and upload guidance.
- `knowledge/` — official legal texts and gazettes.
- `knowledge-guides/` — reasoning, research, citation, and quality-control guidance.
- `indexes/` — cross-reference and retrieval aids.
- `templates/` — standard answer and analysis formats.
- `tests/` — regression and acceptance tests for the Custom GPT.

## Core source hierarchy

1. Constitution of the Dominican Republic.
2. Current controlling criminal legislation and amendments.
3. Código Procesal Penal.
4. Special criminal laws.
5. Regulations and official implementing norms.
6. Binding or persuasive official jurisprudence, according to its legal force.
7. Prior/historical law for temporal analysis and comparison.
8. Secondary summaries and commentary only as explanatory material.

## Current core corpus

The intended knowledge base includes the Constitution, Ley 74-25, Ley 44-26, Ley 97-25, the prior Penal Code, and special statutes concerning cybercrime, money laundering, firearms, controlled substances, children and adolescents, trafficking, migration, public prosecution, police, and public-asset declarations.

## Custom GPT setup

Use `custom-gpt/instructions/custom-gpt-instructions.md` in the GPT **Instructions** field. Upload the official legal texts plus the selected files from `knowledge-guides/`, `indexes/`, and `templates/` to the GPT **Knowledge** section. See `custom-gpt/upload-guide.md`.

## Reliability rule

Official legal texts remain the source of truth. Curated indexes and guides are navigation and reasoning aids; they must never override the controlling statute, amendment, Constitution, or applicable official jurisprudence.
