# Custom GPT Upload Guide — 20 File Limit Strategy

The Custom GPT Knowledge limit is 20 files. The GitHub repository may contain many development files, but the production GPT should use a compact release set.

## 1. Instructions field

Paste the full contents of:

`custom-gpt/instructions/custom-gpt-instructions.md`

This does not consume a Knowledge file slot. Replace the prior Instructions text whenever this file changes.

## 2. Mandatory project-generated Knowledge files — 2 slots

Upload only:

1. `custom-gpt/DR-Criminal-Law-AI-Index.md`
2. `custom-gpt/master-reference-index.md`

`DR-Criminal-Law-AI-Index.md` is the consolidated legal reasoning, writing, conflict-resolution, hallucination-prevention, and response-quality engine. `master-reference-index.md` is the consolidated retrieval and cross-reference index.

Do NOT separately upload files from `knowledge-guides/`, `indexes/`, `templates/`, or `tests/`.

## 3. Core legal authorities — 5 slots

Upload current versions of:

1. Constitution of the Dominican Republic.
2. Ley 74-25 — Código Penal.
3. Ley 44-26 — amendments to Ley 74-25.
4. Ley 97-25 — Código Procesal Penal / Gaceta 11221.
5. Prior Penal Code for historical/transitional analysis.

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

With the 2 project-generated files and 5 core authorities, the recommended production set totals 17 Knowledge files.

## 5. Reserve the remaining 3 slots

Keep 3 slots free for high-value future additions such as:
- controlling regulations;
- later amendments;
- official jurisprudence compilations;
- another special criminal statute shown by testing to be necessary.

Do not fill these slots merely because they are available.

## 6. Files that should NOT be uploaded separately

Do not upload:
- `knowledge-guides/*`
- `indexes/*`
- `templates/*`
- `tests/*`
- `README.md`
- `CHANGELOG.md`
- `CONTRIBUTING.md`
- `custom-gpt/upload-guide.md`
- `custom-gpt/conversation-starters.md`

They are development and maintenance files.

## 7. Optional future legal consolidation

If the legal-source count later exceeds the available slots, consolidate only when legally safe. Prefer clear categories while preserving each law's complete title, article numbering, publication information, and full text. Never summarize or renumber controlling statutes merely to save slots.

Examples:
- `Special_Laws_Public_Authorities.md` — Ley 133-11 + Ley 590-16.
- `Special_Laws_Migration_Trafficking.md` — Ley 285-04 + Ley 137-03.

## 8. Conversation starters

Copy starters from:

`custom-gpt/conversation-starters.md`

These do not consume Knowledge slots.

## 9. Recommended capabilities

Enable web access if you want the GPT to verify later amendments, new official publications, or current jurisprudence. Uploaded official law remains the preferred source for legal text already present in Knowledge.

## 10. Update procedure

When the repository changes:

1. Run `git pull origin main` locally.
2. Review `CHANGELOG.md`.
3. If `custom-gpt-instructions.md` changed, replace the GPT Instructions field with its complete contents.
4. If `DR-Criminal-Law-AI-Index.md` changed, remove/replace that Knowledge file with the latest version.
5. If `master-reference-index.md` changed, remove/replace it with the latest version.
6. Replace any statute that has been amended or superseded.
7. Keep total Knowledge count at 20 or less.
8. Run the scenarios in `tests/test-scenarios.md` and review `tests/acceptance-checklist.md` before publishing.

## 11. Migration to current production layout

For the current reasoning upgrade:
- Replace the GPT Instructions field using the latest `custom-gpt/instructions/custom-gpt-instructions.md`.
- Remove any older `knowledge-guidelines.md` Knowledge upload if it is still present.
- Upload/replace `custom-gpt/DR-Criminal-Law-AI-Index.md`.
- Keep `master-reference-index.md` unless a later commit modifies it.
- No statute needs to be re-uploaded solely because of this reasoning-engine update.
- Your Knowledge file count should remain 17.

## 12. Important limitation

GitHub does not automatically synchronize with Custom GPT Knowledge. Repository changes must be manually uploaded or pasted into the GPT Builder.
