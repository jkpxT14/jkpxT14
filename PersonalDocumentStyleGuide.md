# Personal Document Style Guide

This guide defines the shared design, typography, language, and maintenance conventions for Jungwoo Kim's personal academic documents. The current document family consists of the Curriculum Vitae and Acknowledgements. The documents should feel visibly related without being forced into identical information density or wording.

## 1. Core Principle

- Treat the Curriculum Vitae and Acknowledgements as members of one restrained academic document family.
- Preserve a clean, single-column, serif-based design with ample white space and minimal decoration.
- Keep structural text black. Use institutional colors semantically, not decoratively.
- Preserve intentional document-specific differences when they serve the document's purpose.
- Do not alter existing content merely because another wording or layout seems preferable. Change established content only when the user requests it or when it conflicts with this guide.

## 2. Page and Typography

Shared baseline:

- Paper: A4.
- Margins: top 1.88 cm, bottom 1.82 cm, left 2.12 cm, right 2.12 cm.
- Primary typeface: Linux Libertine.
- Base class size: 10 pt.
- Line spread: 1.01.
- Paragraph indentation: none.
- Text alignment: ragged right.
- Section title: 12.7 pt / 14.7 pt, normal weight.
- Section rule: 0.28 pt, black.
- Space before a section: 1.14 em.
- Space below the section rule: 0.30 em.
- Footer: centered page number `x / y`, 8.0 pt / 9.3 pt, gray.
- Footer skip: 0.78 cm.

Page-break safeguards such as `Needspace` may differ by document because they are layout-safety logic rather than visual style.

## 3. Color

The Curriculum Vitae and Acknowledgements use the same `InstitutionColors.tex` definitions.

Institutional color is reserved for institution-related text. Dates, section rules, punctuation, hyphens, parentheses, descriptive prose, and other structural elements remain black unless explicitly defined otherwise.

Examples:

- `POSTECH` uses POSTECH Red.
- `KAIST` uses KAIST Blue.
- `SNU` uses SNU Blue.
- `Korea University` uses Korea University Crimson.
- `Yonsei University` uses Yonsei Blue.
- `University of Cambridge` uses Cambridge Dark Blue.
- `MIT` uses MIT Red.

In compound expressions such as `KAIST-POSTECH`, color only the institution tokens; keep the hyphen black.

## 4. Punctuation and Separators

### 4.1 Comma `,`

Use commas for linguistic lists: items that belong to the same grammatical field or ordinary sequence.

Examples:

- `Jungwoo Kim, Coauthor Name`
- `C, C++, Python, Java`
- `Korean (native), English (fluent), Japanese (currently studying)`
- `Undergraduate Student, Department of Mathematics, POSTECH`
- `jkpxt14@postech.ac.kr, https://github.com/jkpxT14`
- `Pohang, Republic of Korea`

Do not replace ordinary list commas with middle dots for decoration.

### 4.2 Middle Dot `·`

Use the middle dot only as a visual separator between short, parallel metadata fields or independent keywords.

Examples:

- `Calculus · Analysis · Linear Algebra`
- `Seoul · Pohang, Republic of Korea`
- `Journal Name · Vol. 42 · pp. 123–145`

Do not use the middle dot between authors, programming languages, natural-language lists, or contact items.

### 4.3 Bullet `·`

A middle dot at the beginning of a line may function as a subordinate-list bullet in Acknowledgements.

Example:

- `· Academic Advisor`

This bullet use is distinct from the middle dot as an inline metadata separator.

### 4.4 Hyphen `-`

Use a hyphen when it belongs to an official or established compound name.

Example:

- `KAIST-POSTECH Science War`

Keep the hyphen black even when the adjacent institution names are colored.

### 4.5 En Dash `–`

Use an en dash for ranges.

Examples:

- `2025–Present`
- `June 2026–September 2026`
- `pp. 123–145`

In LaTeX source, use `--`.

### 4.6 Em Dash `—`

Use an em dash to separate hierarchical or explanatory information, not for simple lists.

Example:

- `2026 KAIST-POSTECH Science War — Science Quiz Representative Team`

In LaTeX source, use `---`.

### 4.7 Ampersand `&`

Use `&` in section titles and compact parallel headings.

Examples:

- `Research & Academic Interests`
- `Books & Expository Works`
- `Friends & Peers`

Use `and` in ordinary prose unless an official name requires otherwise.

## 5. Institution Naming

### 5.1 Curriculum Vitae

Use full official institutional names when the institution itself is a primary academic datum.

Examples:

- `Pohang University of Science and Technology (POSTECH)`
- `Seoul National University (SNU)`

Use established abbreviations naturally in event names, program names, and compact secondary references.

Examples:

- `POSTECH Student Mentoring Program (SMP)`
- `2026 KAIST-POSTECH Science War`
- `Mathematics Representative for POSTECH`

### 5.2 Acknowledgements

Prefer compact institutional names or well-established abbreviations because affiliations are secondary to people and relationships.

Examples:

- `POSTECH`
- `KAIST`
- `SNU`
- `MIT`
- `Korea University`
- `Yonsei University`
- `University of Cambridge`

The Acknowledgements owner affiliation should remain compact, e.g. `Undergraduate Student, Department of Mathematics, POSTECH`, rather than reproducing the longer CV affiliation.

## 6. Header Conventions

### Curriculum Vitae

The CV header is formal and institution-focused. It may include the full institutional name, location, email, GitHub, and phone number.

Contact items are black and separated with commas.

### Acknowledgements

The Acknowledgements owner header is intentionally more compact. Keep the owner name and affiliation aligned with the CV's typographic family, but use the short affiliation and only the contact items that are useful for this document.

Owner contact text is black and uses commas between contact items.

Contact information attached to other people in Acknowledgements remains visually subordinate: smaller and gray, while still using commas between contact items.

## 7. Sections and Spacing

Both documents use the same visible section language:

- 12.7 pt / 14.7 pt section titles.
- Normal-weight section titles.
- 0.28 pt black hairline.
- 1.14 em before the section.
- 0.30 em below the hairline.

Internal entry spacing may differ when the document's content structure requires it. For example, Acknowledgements uses dedicated spacing between people, while the CV uses entry-specific tabular structures.

## 8. Scholarly Works in the CV

Scholarly works use a title-first hierarchy rather than a reference-list style.

General hierarchy:

1. Title and year.
2. Authors.
3. Venue, status, bibliographic metadata, or concise description.

Authors form a linguistic list and therefore use commas. Do not add `By` before author names and do not append a period solely because the author line stands alone.

Example publication:

```text
Paper Title                                                   20XX
Jungwoo Kim, Coauthor Name
Journal Name · Vol. 42 · pp. 123–145
```

Example written work:

```text
Mathematics for Science Quiz                       September 2026
Jungwoo Kim
A comprehensive mathematics handbook ...
```

Book and expository-work titles may remain italic. Publication titles may use the CV's primary-entry emphasis. The common design language is the title-first hierarchy, not identical typography for every work type.

## 9. Event and Role Hierarchy

Preserve official year-specific event naming. For the 2026 Science War, the official order is `KAIST-POSTECH`.

When a category or role is subordinate to an event, use an em dash when a single-line hierarchy is appropriate.

Example in Acknowledgements:

- `2026 KAIST-POSTECH Science War — Science Quiz Representative Team`

The CV may express the same structure across multiple lines when its entry hierarchy calls for it.

## 10. Dates and Ranges

- Use month and year when the month is meaningful: `September 2026`.
- Use semester notation for semester-based university activities: `2026 Spring`, `2026 Fall`.
- Use en dashes for ranges: `2025–Present`.
- In LaTeX source, encode en dashes with `--` and em dashes with `---`.
- Preserve the most precise existing date style unless a document-wide inconsistency requires correction.

## 11. Document-Specific Differences

The documents should be consistent, not identical.

- The CV is formal, institution-focused, and designed for academic evaluation.
- Acknowledgements is people-focused and intentionally lighter in information density.
- The CV may use full institution names where academically important.
- Acknowledgements may prefer established abbreviations and shorter affiliations.
- Acknowledgements may use small gray contact metadata for other people.
- Acknowledgements has its own centered document title and one-line message beneath the owner identity block.

These differences are intentional and should not be normalized away merely for visual symmetry.

## 12. Maintenance Rule

When updating either document:

1. Start from the latest user-maintained source.
2. Preserve existing user edits outside the requested scope.
3. Apply this guide only where a genuine cross-document inconsistency exists or where the user explicitly requests normalization.
4. Keep `InstitutionColors.tex` synchronized between the two document folders.
5. Recompile and visually inspect the PDFs after any style or spacing change.
