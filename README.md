# DR Penal Code AI

A bilingual (Spanish/English) legal-research knowledge base for Dominican criminal law. The project supports a Custom GPT grounded in official statutes, amendments, procedural rules, and curated research guidance.

## Purpose

The assistant helps users locate and explain Dominican criminal-law provisions, compare prior and current law, identify procedural rules, and produce source-grounded bilingual explanations. It is a legal-information and research tool, not a substitute for representation by a licensed attorney.

## Repository structure

- `custom-gpt/` — production instructions, conversation starters, upload guidance, and consolidated Knowledge files.
- `knowledge/` — official legal texts and gazettes maintained in the repository.
- `knowledge-guides/` — detailed reasoning, research, citation, and quality-control source material maintained for development.
- `indexes/` — detailed cross-reference and retrieval aids maintained for development.
- `templates/` — standard answer and analysis formats.
- `tests/` — regression and acceptance tests for the Custom GPT.

## Core source hierarchy

1. Constitution of the Dominican Republic.
2. Current controlling criminal legislation and amendments.
3. Código Procesal Penal.
4. Special criminal laws.
5. Regulations and official implementing norms.
6. Verified official jurisprudence according to its legal force.
7. Prior/historical law for temporal analysis and comparison.
8. Secondary summaries and commentary only as explanatory material.

## Custom GPT production setup

The Custom GPT Knowledge section has a 20-file practical limit, so the production configuration intentionally uses consolidated project guidance instead of uploading every development file separately.

### Instructions field

Paste the contents of:

`custom-gpt/instructions/custom-gpt-instructions.md`

### Knowledge section

Upload the official legal corpus plus these two consolidated project files:

- `custom-gpt/knowledge-guidelines.md`
- `custom-gpt/master-reference-index.md`

Do **not** separately upload the files in `knowledge-guides/`, `indexes/`, `templates/`, or `tests/` unless a future release explicitly instructs otherwise. They remain in GitHub as maintainable source material for the consolidated production files.

See `custom-gpt/upload-guide.md` for the current file-slot plan and update procedure.

## Current recommended Knowledge allocation

The recommended base configuration uses 17 of 20 slots:

1. Constitution of the Dominican Republic.
2. Ley 74-25 — Código Penal.
3. Ley 44-26 — amendments to Ley 74-25.
4. Ley 97-25 — Código Procesal Penal.
5. Prior Penal Code.
6. Ley 53-07 — Crímenes y Delitos de Alta Tecnología.
7. Ley 155-17 — Lavado de Activos y Financiamiento del Terrorismo.
8. Ley 631-16 — Armas, Municiones y Materiales Relacionados.
9. Ley 50-88 — Drogas y Sustancias Controladas.
10. Ley 136-03 — Niños, Niñas y Adolescentes.
11. Ley 137-03 — Tráfico Ilícito de Migrantes y Trata de Personas.
12. Ley 133-11 — Ministerio Público.
13. Ley 590-16 — Policía Nacional.
14. Ley 285-04 — Migración.
15. Ley 311-14 — Declaración Jurada de Patrimonio.
16. `custom-gpt/knowledge-guidelines.md`.
17. `custom-gpt/master-reference-index.md`.

This leaves three Knowledge slots available for high-value future additions such as important regulations, verified jurisprudence compilations, or another controlling special statute.

## Reliability rule

Official legal texts remain the source of truth. Consolidated guides and indexes are navigation and reasoning aids; they never override the controlling Constitution, statute, amendment, procedural rule, regulation, or verified jurisprudence.

## Updating locally

From the project directory:

```bash
cd /Users/alexinoa/DMZ/drpenalcode
git pull origin main
```

Then review `CHANGELOG.md` and `custom-gpt/upload-guide.md` before replacing files in the Custom GPT.
