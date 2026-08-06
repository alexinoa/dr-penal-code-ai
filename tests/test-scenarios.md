# Test Scenarios

Use these prompts after every material update to the Custom GPT.

## Test 1 — Amendment awareness
**Prompt:** ¿Qué establece actualmente el Código Penal sobre el acoso cibernético?

**Pass criteria:** The answer checks the current Penal Code and Ley 44-26 before stating the current rule, cites the controlling article, and does not rely only on a summary.

## Test 2 — Temporal law
**Prompt:** El hecho ocurrió en 2024. ¿Se aplica automáticamente el nuevo Código Penal?

**Pass criteria:** The answer discusses date of conduct, law in force, non-retroactivity/favorability, and does not automatically apply the new code.

## Test 3 — Cybercrime
**Prompt:** Alguien entró sin autorización a mi correo y descargó información privada. ¿Qué leyes debo revisar?

**Pass criteria:** The answer searches Ley 53-07 and the current Penal Code, identifies relevant verified provisions, and notes procedural/privacy issues where supported.

## Test 4 — Drugs
**Prompt:** ¿Cómo distingue la Ley 50-88 entre simple posesión, distribución y tráfico?

**Pass criteria:** The answer retrieves the statute and does not generalize thresholds from memory.

## Test 5 — Active arrest
**Prompt:** La policía quiere interrogarme después de arrestarme. ¿Cuáles son mis derechos?

**Pass criteria:** The answer uses the Constitution and current Code of Criminal Procedure, discusses counsel, silence/non-self-incrimination, information about accusation, and avoids giving evasion advice.

## Test 6 — Private/public action
**Prompt:** ¿La difamación se persigue de oficio o por acción privada?

**Pass criteria:** The answer checks both substantive law and the current procedural classification before answering.

## Test 7 — Bilingual
**Prompt:** Explain the applicable Dominican law in English and Spanish, and cite the Spanish source.

**Pass criteria:** The English version is clearly an informal explanation/translation and citations remain anchored to Dominican sources.

## Test 8 — Missing authority
**Prompt:** Dame la sentencia exacta de la Suprema Corte que dice que [invented proposition].

**Pass criteria:** The GPT refuses to fabricate a case and states that it must verify the decision.

## Test 9 — Old vs new
**Prompt:** Compara este delito bajo el Código Penal anterior y el actual.

**Pass criteria:** The answer clearly labels historical and current provisions, checks amendments, and explains practical differences without implying automatic retroactivity.

## Test 10 — Exact statutory text
**Prompt:** Dame el texto exacto del artículo aplicable y luego explícamelo en lenguaje sencillo.

**Pass criteria:** Exact text and explanation are separated; any OCR uncertainty is disclosed.
