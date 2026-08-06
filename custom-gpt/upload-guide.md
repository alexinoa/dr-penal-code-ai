# Custom GPT Upload Guide — 20 File Limit Strategy

The Custom GPT Knowledge limit is 20 files. Do not upload every project guide, index, template, and test file separately. The GitHub repository may contain many files for maintenance, but the Custom GPT should receive a compact release set.

## 1. Instructions field

Paste the full contents of:

`custom-gpt/instructions/custom-gpt-instructions.md`

This does not consume a Knowledge file slot.

## 2. Mandatory reasoning files — 2 slots total

Upload only these two project-generated Knowledge files:

1. `custom-gpt/knowledge-guidelines.md`
2. `custom-gpt/master-reference-index.md`

Do NOT separately upload the files in `knowledge-guides/`, `indexes/`, `templates/`, or `tests/`. They remain in GitHub for maintenance, development, and future generation of the consolidated files.

## 3. Core legal authorities — 5 slots

Upload current versions of:

1. Constitution of the Dominican Republic.
2. Ley 74-25 — Código Penal.
3. Ley 44-26 — amendments to Ley 74-25.
4. Ley 97-25 — Código Procesal Penal.
5. Prior Penal Code for historical/transitional analysis.

Running total: 7 files.

## 4. Priority special laws — 10 slots

Upload:

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

With the 2 project-generated files and 5 core authorities, this produces a total of 17 Knowledge files.

## 5. Reserve the remaining 3 slots

Keep 3 slots free for the most valuable current additions, such as:

- a controlling regulation directly relevant to frequent consultations;
- an official consolidated amendment;
- a high-value official jurisprudence compilation;
- another special criminal statute that proves necessary in testing.

Do not fill the last three slots merely because space exists. Reserve them for real coverage gaps.

## 6. Files that should NOT be uploaded separately

Do not upload these separately to the GPT Knowledge section:

- `knowledge-guides/*`
- `indexes/*`
- `templates/*`
- `tests/*`
- `README.md`
- `CHANGELOG.md`
- `CONTRIBUTING.md`
- `custom-gpt/upload-guide.md`
- `custom-gpt/conversation-starters.md`

They are development and maintenance files. Their useful behavioral content is consolidated into the two required project-generated Knowledge files.

## 7. Optional future legal consolidation

If the legal-source count later exceeds 18 statutory files, consolidate only when legally safe. Prefer grouping documents by a clear category while preserving each law's complete title and article numbering, for example:

- `Special_Laws_Public_Authorities.md` containing Ley 133-11 + Ley 590-16.
- `Special_Laws_Migration_Trafficking.md` containing Ley 285-04 + Ley 137-03.

Do not merge unrelated controlling laws merely to save slots. Never edit, summarize, renumber, or intermix statutory text. Each law inside a merged file must have a prominent delimiter, full title, law number, publication information, and complete text.

## 8. Conversation starters

Copy starters from:

`custom-gpt/conversation-starters.md`

Conversation starters do not consume Knowledge slots.

## 9. Recommended capabilities

Enable web access if you want the GPT to verify later amendments, new official publications, or current jurisprudence. Uploaded official law remains the preferred source for text already present in Knowledge.

## 10. Update procedure

When the repository changes:

1. `git pull origin main` locally.
2. Review `CHANGELOG.md`.
3. If `custom-gpt-instructions.md` changed, re-paste it into Instructions.
4. Replace `knowledge-guidelines.md` and/or `master-reference-index.md` if modified.
5. Replace any statute that was amended or superseded.
6. Keep the total Knowledge count at 20 or less.
7. Run `tests/test-scenarios.md` locally as your validation checklist.

## 11. Important limitation

GitHub does not automatically synchronize with Custom GPT Knowledge. Repository updates must be manually uploaded/replaced in the GPT Builder.
