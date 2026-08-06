# Custom GPT Upload Guide

## 1. Instructions field

Paste the full contents of:

`custom-gpt/instructions/custom-gpt-instructions.md`

Keep this field concise. Behavioral rules belong here; legal substance belongs in Knowledge.

## 2. Knowledge files — mandatory core law

Upload the current versions of:

- Constitution of the Dominican Republic.
- Ley 74-25 — Código Penal.
- Ley 44-26 — amendments to Ley 74-25.
- Ley 97-25 — Código Procesal Penal.
- Prior Penal Code for historical/transitional analysis.

## 3. Knowledge files — special laws

Upload current official texts for the special laws you maintain, including at minimum:

- Ley 53-07 — Crímenes y Delitos de Alta Tecnología.
- Ley 155-17 — Lavado de Activos y Financiamiento del Terrorismo.
- Ley 631-16 — Armas, Municiones y Materiales Relacionados.
- Ley 50-88 — Drogas y Sustancias Controladas.
- Ley 136-03 — Niños, Niñas y Adolescentes.
- Ley 137-03 — Tráfico Ilícito de Migrantes y Trata de Personas.
- Ley 133-11 — Ministerio Público.
- Ley 590-16 — Policía Nacional.
- Ley 285-04 — Migración.
- Ley 311-14 — Declaración Jurada de Patrimonio.

Add official regulations, later amendments, and replacement statutes when enacted.

## 4. Knowledge files — reasoning layer

Upload these project files after the statutes:

- `knowledge-guides/02-legal-reasoning-engine.md`
- `knowledge-guides/03-research-methodology.md`
- `knowledge-guides/04-source-hierarchy.md`
- `knowledge-guides/05-citation-standards.md`
- `knowledge-guides/06-output-formats.md`
- `knowledge-guides/07-criminal-offense-framework.md`
- `knowledge-guides/08-procedural-framework.md`
- `knowledge-guides/09-jurisprudence-framework.md`
- `knowledge-guides/10-hallucination-prevention.md`
- `knowledge-guides/11-professional-standards.md`
- `knowledge-guides/12-quality-assurance-checklist.md`

These files guide retrieval and analysis but never override controlling law.

## 5. Indexes and templates

Upload the following when populated:

- `indexes/bilingual-legal-glossary.md`
- `indexes/crime-cross-reference-index.md`
- `indexes/constitutional-rights-index.md`
- `indexes/penalty-matrix.md`
- `indexes/special-laws-index.md`
- selected files from `templates/`

## 6. Conversation starters

Copy the starters from `custom-gpt/conversation-starters.md` into the GPT builder.

## 7. Recommended capabilities

Enable web access only if you want the GPT to verify later amendments, new official publications, or current jurisprudence. The GPT should still prefer uploaded official sources for the legal text already present in Knowledge.

## 8. Update procedure

When the repository changes:

1. Pull the latest version locally.
2. Review `CHANGELOG.md`.
3. Replace modified reasoning/index files in Custom GPT Knowledge.
4. Replace any statute that has been amended or superseded.
5. Re-paste the Instructions file only if that file changed.
6. Run the tests in `tests/test-scenarios.md`.
7. Do not publish changes until the acceptance checklist passes.

## 9. Important limitation

Custom GPT Knowledge does not automatically synchronize with GitHub. Updating this repository does not update the GPT. Files must be manually re-uploaded or replaced in the GPT builder.
