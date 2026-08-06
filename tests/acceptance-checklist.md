# Custom GPT Acceptance Checklist

A release should not be treated as ready until the following checks pass.

## Configuration
- [ ] Custom GPT Instructions match `custom-gpt/instructions/custom-gpt-instructions.md`.
- [ ] Core official statutes are uploaded to Knowledge.
- [ ] Current amendments are uploaded.
- [ ] Reasoning guides are uploaded.
- [ ] Old or superseded laws are clearly identifiable as historical.

## Retrieval
- [ ] GPT can locate an article by number.
- [ ] GPT can locate a rule from a plain-language factual description.
- [ ] GPT checks Ley 44-26 when relevant to Ley 74-25.
- [ ] GPT searches special laws for special-law subjects.
- [ ] GPT uses the current Code of Criminal Procedure for procedural questions.

## Reliability
- [ ] GPT does not fabricate a nonexistent article.
- [ ] GPT does not fabricate jurisprudence.
- [ ] GPT distinguishes exact statutory text from explanation.
- [ ] GPT flags apparent OCR problems.
- [ ] GPT identifies missing facts instead of guessing.
- [ ] GPT distinguishes allegation from guilt.

## Temporal analysis
- [ ] GPT asks for date of conduct when necessary.
- [ ] GPT distinguishes old and new Penal Codes.
- [ ] GPT considers amendments/effective dates.
- [ ] GPT does not automatically apply a harsher later law to earlier conduct.

## Bilingual quality
- [ ] Spanish answers preserve Dominican terminology.
- [ ] English explanations do not falsely claim to be official translations.
- [ ] English wording does not silently import incompatible U.S. legal concepts.

## User experience
- [ ] Simple questions receive concise answers.
- [ ] Complex case questions receive structured analysis.
- [ ] Material propositions include source citations.
- [ ] Active criminal matters include an appropriate recommendation for Dominican counsel.

## Release result

**PASS:** all material checks succeed.

**FAIL:** correct the source corpus, Instructions, or reasoning guides and repeat the test suite.
