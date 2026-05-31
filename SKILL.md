---
name: my-dream-skills
description: >
  Use when the user asks to write, plan, revise, upgrade, review, or finalize a
  doctoral dissertation, CSSCI paper, SSCI paper, AMI journal paper, humanities
  or social science manuscript, literature review, thesis chapter, research
  proposal, or academic outline according to CSSCI, SSCI, AMI, or
  discipline-specific academic writing standards. This skill upgrades the user's
  installed academic writing skills by enforcing progressive argument logic,
  journal-aware structure, humanities/social-science disciplinary voice,
  academic register, separate body/full-text word counts, recent DOI-based
  literature selection, and citation/reference formatting in GB/T 7714-2025,
  MLA, or APA style.
metadata:
  display_name: "MY dream skills"
---

# MY Dream Skills

This skill is an optimization layer for academic writing, not a copy of the
other installed skills. Use those skills for their original strengths, then
apply this skill's stricter standards for structure, argument, citation quality,
reference formatting, literature freshness, and final manuscript readiness.

## Core Purpose

Every substantial output must improve the user's existing academic workflow in
four ways:

- Argument upgrade: build a progressive chain from problem consciousness to
  research gap, research question, theoretical frame, evidence, analysis,
  contribution, limitation, and future research.
- Style upgrade: use formal academic prose, reduce colloquial phrasing, avoid
  decorative verbosity, and adapt the language to the target discipline.
- Citation upgrade: use one declared citation mode: GB/T 7714-2025, MLA, or
  APA. Keep in-text citations and reference-list entries consistent.
- Source upgrade: prefer literature published within 5 years of the writing
  date and require DOI-bearing sources unless the user explicitly allows
  exceptions for classics, laws, archives, historical texts, datasets, policy
  documents, or primary materials.

## Relationship to Existing Skills

Do not duplicate other skills. Use them as engines and apply this skill as the
quality specification above them.

- `academic-research-suite`: use for research-question narrowing, literature
  review, outline design, drafting, revision, peer-review simulation, citation
  checks, and academic-paper workflows.
- `paper-spine`: use for full paper or dissertation workflows requiring target
  research, motivation confirmation, section blueprints, writing rationale
  matrices, LaTeX/DOCX finalization, translation, humanizing, and audit.
- `paper-spine-research`: use when the target journal, field, examples, SOTA,
  or recent literature landscape must be learned before writing.
- `paper-spine-citation`: use to build a citation support bank. Upgrade its
  output with the recency, DOI, and citation-format rules in this skill.
- `paper-spine-build` and `paper-spine-rewrite`: use for building or rewriting
  manuscripts; this skill defines the target structure, disciplinary tone, and
  citation constraints.
- `paper-spine-humanize`: use only after the logic and citations are stable to
  reduce mechanical or AI-like phrasing while preserving academic precision.
- `paper-spine-audit`: use before calling a major manuscript complete.
- `zotero-review-matrix`: use when Zotero collections, notes, annotations,
  highlights, or reading matrices are part of the evidence base. Upgrade its
  references to the requested citation style when possible.

## Intake Rules

Ask only for missing information that materially changes the output. For most
tasks, ask no more than 3 questions at once.

Required when available:

- Target type: CSSCI, SSCI, AMI, doctoral dissertation, thesis chapter, journal
  article, proposal, literature review, or other.
- Language: Chinese, English, or bilingual.
- Discipline and subfield.
- Manuscript genre and stage: outline, abstract, introduction, literature
  review, method, analysis, discussion, conclusion, revision, full draft, or
  final formatting.
- Citation mode: GB/T 7714-2025, MLA, APA, or target journal style.
- Word budget:
  - Body-only count.
  - Full-text count including title, abstract, keywords, notes, tables,
    captions, appendices, and references.
- Evidence base: Zotero collection, PDFs, notes, dataset, cases, interviews,
  archives, policy documents, theoretical texts, existing draft, tables, or
  figures.

If the citation mode is missing, use these defaults:

- CSSCI and AMI Chinese manuscripts: GB/T 7714-2025.
- SSCI English manuscripts: APA, unless the field clearly prefers MLA.
- Literature, cultural studies, art history, and language studies in English:
  ask whether MLA or APA is preferred when the target journal is unknown.

## Literature Selection Standard

Default rule: references should generally be from the latest 5 years relative
to the writing date and should have DOI numbers.

Apply the rule as follows:

- Build a recent-literature pool first. Prefer peer-reviewed journal articles
  with DOI.
- Record DOI for every scholarly article whenever available.
- If a source has no DOI, do not use it as a default core citation unless it is
  a justified exception.
- Mark exceptions explicitly: `经典理论`, `原始文献`, `法律政策`, `档案材料`,
  `数据集`, `行业报告`, `历史文本`, `目标期刊要求`, or `用户指定`.
- Keep classic and foundational works only when they are necessary for theory,
  method, or genealogy; pair them with recent DOI-bearing scholarship where
  possible.
- When exact recent literature, DOI status, journal requirements, or citation
  rules are uncertain, verify from current sources before presenting them as
  final.

For each citation-support bank or reference list, include these fields when
possible:

| Field | Requirement |
|---|---|
| Citation key | Short stable key, e.g. `Wang2024Platform` |
| Authors | Preserve original order |
| Year | Publication year |
| Title | Article/chapter/book title |
| Source | Journal, book, conference, or repository |
| DOI | Required for ordinary journal articles unless justified |
| Age check | `近五年` or exception label |
| Use in paper | Which claim, paragraph, or section it supports |
| Citation style entry | GB/T 7714-2025, MLA, or APA formatted entry |

## Citation Modes

Use one mode consistently unless the user asks for comparison.

### GB/T 7714-2025 Mode

Use for CSSCI, AMI, Chinese dissertations, and Chinese social science papers
unless the user specifies another style.

Operational rules:

- Use numeric citation markers in the manuscript when the target requires
  numbered references, e.g. `[1]`, `[2]`.
- Format the reference list in the requested GB/T 7714-2025 style. If exact
  target-journal details differ, follow the journal guide and state the
  adjustment.
- Include DOI at the end of entries when available or required by the target.
- Keep Chinese and English references in a consistent sequence required by the
  target journal or school. If no rule is supplied, use citation order for
  numbered references.
- Do not silently convert GB/T to APA-like author-date prose.

Article template:

```text
[序号] 作者. 题名[J]. 刊名, 年, 卷(期): 起止页码. DOI: DOI号.
```

Book template:

```text
[序号] 作者. 书名[M]. 出版地: 出版者, 年.
```

Chapter template:

```text
[序号] 作者. 析出文献题名[M]//编者. 书名. 出版地: 出版者, 年: 起止页码.
```

### APA Mode

Use for SSCI manuscripts in psychology, education, communication, management,
sociology, public administration, political science, and related fields unless
the journal states otherwise.

Operational rules:

- Use author-date in-text citations, e.g. `(Author, 2024)` or
  `Author (2024)`.
- Use hanging-indent reference-list logic when producing formatted documents.
- Include DOI as a URL when available: `https://doi.org/...`.
- For multiple works by the same author/year, use `2024a`, `2024b`.

Article template:

```text
Author, A. A., & Author, B. B. (Year). Article title. Journal Title, volume(issue), page range. https://doi.org/DOI
```

Book template:

```text
Author, A. A. (Year). Book title. Publisher.
```

### MLA Mode

Use for literature, language, cultural studies, art history, media studies, and
humanities fields when MLA is requested or field-appropriate.

Operational rules:

- Use author-page in-text citations when page numbers are available, e.g.
  `(Author 23)`.
- If page numbers are unavailable, use author-only in-text citation or the
  target journal's preferred locator.
- Include DOI when available.
- Use a Works Cited list, not an APA-style References heading, unless the user
  asks otherwise.

Article template:

```text
Author Last Name, First Name. "Article Title." Journal Title, vol. volume, no. issue, Year, pp. page range. DOI.
```

Book template:

```text
Author Last Name, First Name. Book Title. Publisher, Year.
```

## Journal-Type Defaults

### CSSCI

- Chinese academic register; emphasize problem consciousness, theoretical
  dialogue, local context, social/cultural/policy relevance, and contribution
  to Chinese-language scholarship.
- Default citation mode: GB/T 7714-2025.
- Count by Chinese word/character convention. Report body count and full count
  separately.

### SSCI

- English academic register; emphasize explicit gap, research question,
  theoretical contribution, method transparency, findings, discussion, and
  limitations.
- Default citation mode: APA unless the field or journal prefers MLA.
- Count by English words. Report body count and full count separately.

### AMI

- Chinese humanities/social-science register; emphasize theoretical depth,
  academic innovation, disciplinary positioning, and a stable argument chain.
- Default citation mode: GB/T 7714-2025.
- Count by Chinese word/character convention. Report body count and full count
  separately.

## Disciplinary Voice

Adapt the structure and evidence logic:

- Literature, philosophy, art, history: conceptual genealogy, textual or
  historical evidence, interpretive depth, careful periodization, and restrained
  theoretical claims.
- Law and public administration: normative issue, institutional context, legal
  or policy framework, doctrinal/empirical support, and governance implications.
- Sociology, anthropology, communication, education: theory-driven empirical
  question, method transparency, field/context sensitivity, and mechanism
  analysis.
- Management, economics, information systems: construct clarity, model or
  mechanism logic, method and robustness when empirical, and practical plus
  theoretical contribution.
- Political science and international relations: concept definition, causal or
  interpretive logic, institutional/historical context, and evidence discipline.

When the discipline is unknown, ask or state the assumed disciplinary frame.

## Output Protocol

For paper writing or revision, produce:

1. Target profile: journal type, language, discipline, genre, citation mode,
   recency/DOI rule, and word-count basis.
2. Core argument: one controlling thesis and 3-5 subclaims.
3. Structure: section-level outline with each section's argumentative function.
4. Evidence and citation plan: sources, data, cases, texts, or citations for
   each claim; mark missing evidence as `待补充`.
5. Draft or revised text, if requested.
6. Reference list in the selected mode: GB/T 7714-2025, MLA, or APA.
7. Word-count report:
   - Body text count.
   - Full text count including references and auxiliary content.
   - Counting basis: English words or Chinese word/character convention.
8. Quality check: logic progression, academic register, disciplinary fit,
   citation-format consistency, DOI coverage, recency coverage, and unsupported
   claims.

For outlines only, omit the full draft but keep the target profile, core
argument, evidence plan, citation mode, and word-count plan.

## Reference Audit Gate

Before finalizing a literature review, article, dissertation chapter, or full
paper, produce or internally verify:

- Citation mode is declared and used consistently.
- At least 80% of ordinary scholarly journal references are from the latest
  5 years unless the user or field requires otherwise.
- Ordinary journal references include DOI where available; missing DOI entries
  are labeled and justified.
- Every in-text citation has a matching reference-list entry.
- Every reference-list entry is cited or marked as background/further reading.
- No fabricated DOI, page range, issue number, author, title, or journal name.
- Claims based on non-scholarly sources are labeled by source type.

## GitHub Skill Packaging

When preparing this skill for GitHub, include only necessary skill files:

```text
my-dream-skills/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    └── citation_modes.md
```

The GitHub version should preserve the same frontmatter `name:
my-dream-skills`. Do not include generated papers, user drafts, private notes,
Zotero exports, or local-only configuration in the public skill repository.
