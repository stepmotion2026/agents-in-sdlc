# de-de

These rules apply to **both roles**: the `translator` agent uses them as generation directives (how to write the German text), and the `evaluator` agent uses them as review criteria (what to check and flag).

Good translation requires both accuracy of meaning and natural flow. Verify that the text passes the core tests for accuracy, fluency, consistency, and cultural appropriateness.

The four core pillars are:

- **Accuracy:** Preserve the source meaning exactly, without additions, distortions, or omissions.
- **Fluency:** Follow German grammar, spelling, and punctuation so the text reads as native German.
- **Terminology & Consistency:** Use specialized terms, names, and recurring phrases uniformly.
- **Cultural Appropriateness:** Adapt idioms and register for readers in Germany, Austria, and Switzerland.

## English to German (Germany) Localization Scenario

### Key Evaluation Pillars for German

- **Regional Standard:** Use standard German (`de-DE`) with new German orthography. Do not use Swiss spellings such as `ss` for `ß`.
- **Reader Address and Register:** Address developers with the informal **du** form and keep it uniform. Write imperatives in the second person singular (**Führe aus**, **Öffne**, **Prüfe**). Do not mix **du**, **Sie**, and impersonal forms within a document.
- **Grammar:** Check case, gender, number, and adjective endings, especially around untranslated product names and code terms. Write compound nouns correctly (**Kontextfenster**) and join compounds that contain English terms or product names with hyphens (**Copilot-CLI-Sitzung**).
- **Natural Syntax:** Restructure English noun stacks and long chains of modifiers. Place verbs naturally; avoid literal word order.
- **Punctuation:** Use German quotation marks („…“) for prose, but keep straight quotes inside code. Use a comma before dependent clauses.

### Common Translation Mistakes to Flag

- **English Calques:** Flag literal renderings such as *Das macht Sinn* for "That makes sense" (prefer **Das ist sinnvoll**) or *Applikation* where **Anwendung** or **App** is the established term.
- **Over-translation:** Do not translate product names, commands, or widely used developer terms such as **Pull Request**, **Commit**, **Branch**, **Prompt**, or **Agent** when they are the normal usage in German developer documentation.
- **Anglicized Verbs:** Avoid forced forms like *committen* or *pushen* in running prose unless they are the common usage; prefer a plain phrase such as **einen Commit erstellen** or **per Push hochladen**.
- **False Friends:** Check terms such as *actually* (**tatsächlich**, not *aktuell*), *eventually* (**schließlich**, not *eventuell*), and *library* (**Bibliothek**, not *Librarie*).
- **Possessive Overuse:** English repeats "your" more often than German. Omit possessives when the referent is clear.

### Practical Evaluation Framework

| Evaluation Metric | What to Look For (English to German Context) |
| :--- | :--- |
| **Accuracy (Genauigkeit)** | Are every fact, condition, number, name, and logical relationship preserved? |
| **Fluency (Sprachfluss)** | Would a reader in Germany understand each sentence immediately without noticing English syntax? |
| **Style Guide (Stil)** | Are case, compounds, punctuation, and capitalization correct? |

## Markdown Syntaxes

Keep Markdown delimiters attached to the text they format. Do not allow translated punctuation or articles to enter URLs, code spans, or link targets.

When a translated heading changes its generated slug, update every same-document link to the localized anchor. Preserve external URLs exactly.

## Localization for Technical Documents for Developers

German developer documentation should be precise and concise. Translate established concepts when the German term is conventional, and keep product names, API names, identifiers, commands, and widely recognized technology terms.

### Developer-Specific Evaluation Rules

#### Terminology and English Terms

Use consistent glossary terms:

| English | German |
| :--- | :--- |
| context window | Kontextfenster |
| instructions | Anweisungen |
| issue | Issue (Plural: Issues) |
| pull request | Pull Request |
| repository | Repository |
| session | Sitzung |
| plan mode | Plan-Modus |
| skill | Skill |
| custom agent | benutzerdefinierter Agent |
| workshop | Workshop |
| lesson | Lektion |

- Keep variables, function names, APIs, CLI commands (`npm install`), file names, slash commands (`/context`), and code exactly as in the source. Translate only human-language comments and explanatory prose inside code blocks.
- For critical or unfamiliar jargon, the first occurrence in a file may include the English source term in parentheses when it helps lookup. Apply this selectively.

#### Tone and Instructions

- Use concise professional prose with direct instructions such as **Führe den folgenden Befehl aus**.
- Avoid unnecessary courtesy formulas and padding such as **bitte**.
- Preserve distinctions among requirements (**muss**), recommendations (**sollte**), and possibilities (**kann**). Never weaken or strengthen normative language.

### Quick Quality Checklist for Developer Docs

| What to Flag (Bad) | What to Approve (Good) | Why it Matters |
| :--- | :--- | :--- |
| **„Lauf `npm install`“** | **„Führe `npm install` aus“** | Avoids an English calque while preserving the command. |
| Switching between **du** and **Sie** | One consistent treatment | Keeps the documentation voice stable. |
| Translating `/context` | Keeping `/context` unchanged | Preserves the command exactly. |

## Evaluator Scoring Rubric

This is the **definitive pass/fail gate** for the `evaluator` role. Criteria are split into two tiers:

- **Tier A — Hard-fail criteria:** any material defect makes the document unusable, so these **must score 5 to pass**.
- **Tier B — Graded criteria:** scored on the 1–5 scale below; these **pass at 4 or 5**.

A document **PASSES only when every applicable Tier A criterion scores 5 and every applicable Tier B criterion scores 4 or 5.** Otherwise it FAILS and is returned to the translator with specific notes that cite the offending source and target snippets.

Tier B scale:

- **5 — Excellent:** Fully meets the criterion; no issues.
- **4 — Good (pass):** At most 1–2 trivial, non-blocking nits per ~1,000 words.
- **3 — Borderline (fail):** Several noticeable issues, or any issue that changes how a sentence reads.
- **2 — Poor (fail):** Frequent or significant violations.
- **1 — Unacceptable (fail):** The criterion is largely unmet.

### Determining Content Type

- **Technical documentation** is content for developers or operators, or any document containing code, commands, or API identifiers. Criteria 7–8 apply.
- **Non-technical content** is UI, marketing, narrative, or conversational copy without code. Criteria 7–8 do not apply.

### Tier A — Hard-Fail Criteria (Must Score 5)

| # | Criterion | Passes (5) when… | Fails (<5) when… |
| :-- | :--- | :--- | :--- |
| 1 | **Accuracy (Genauigkeit)** | Meaning matches the source exactly; all facts, numbers, names, conditions, and modality are preserved. | Any mistranslation, negation flip, fabricated or dropped fact, altered number or name, or changed requirement level occurs. |
| 2 | **Markdown & Structural Integrity** | Frontmatter keys, Markdown, tables, external URLs, and heading order are preserved; localized anchors resolve; image paths point to real assets. | Any link or asset path is broken, a frontmatter key is translated, an English anchor remains after its heading changes, or Markdown or table structure is damaged. |

### Tier B — Graded Criteria (Must Score at Least 4)

| # | Criterion | Scores 5 when… | Pass floor — Score 4 | Fail ceiling — Score 3 | Scores 1 when… |
| :-- | :--- | :--- | :--- | :--- | :--- |
| 3 | **Fluency (Sprachfluss)** | Reads as native German; grammar, case, compounds, and punctuation are correct; no calques. | At most 2 minor slips that do not impede reading. | Any awkward calque requiring rereading, or 3+ language errors. | English-shaped or ungrammatical prose is pervasive. |
| 4 | **Register & Reader Address** | Professional register with a uniform **du** treatment. | One isolated treatment slip. | Two or more treatment shifts, or an audience-inappropriate tone. | Register and reader address are inconsistent throughout. |
| 5 | **Terminology & Consistency** | Terms follow the glossary and German conventions; each concept is rendered consistently. | One minor inconsistency remains understandable. | Two or more inconsistent renderings, a false friend, or one misleading term. | Terminology is unreliable throughout. |
| 6 | **Naturalness** | Idioms, possessives, and syntax are natural German without source-language interference. | One or two harmless stylistic nits. | Several calques or ambiguous possessives. | The text consistently sounds translated. |
| 7 | **Code & Command Integrity** *(technical only — Tier A severity: any violation caps this at ≤2)* | Variables, identifiers, APIs, file names, slash commands, and commands are unchanged; only human-language comments are translated. | — (no trivial tolerance) | A single identifier, file name, or command is altered. | Code and commands are altered throughout. |
| 8 | **Developer Terminology Convention** *(technical only)* | Established German and retained English terms match actual developer usage; over-translation is avoided. | One borderline but recognizable choice. | A forced translation or nonstandard term would confuse a developer. | Technical concepts are consistently rendered unnaturally. |

> Criterion 7 has Tier A severity in practice: any altered command or identifier fails the document.

**Overall result:** PASS only if Criteria 1–2 equal 5 and every applicable Criterion 3–8 is at least 4, with no Criterion 7 violation. Otherwise FAIL and iterate, up to the 3-iteration escalation cap. Score each defect under the most specific criterion and do not double-penalize it.
