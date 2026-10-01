# Solarae audit (pass 4)

17 September 2026. Scope: the Solarae report as supplied in pass 4 (93 sheets), its build, and its research registers.

## 1. Inputs

Pass 3 inputs M1 to M9 are cleared, with these exceptions:

| # | Item | State | Clear-by action |
|---|---|---|---|
| M3 | Raw data | Cleared as a finding: no measured layer exists because no pilot has run (`DATA_POSITION.md`). | None; the report now says so on the contents page. |
| P1 | `process-lineage.mmd`, `full-concept-lineage.mmd` | Missing | Add both to `build/`; `npm run build:html` fails without them. |
| P2 | Rendered PDF | Omitted (size); `pdf-status.md` says no PDF is approved | Run the prepress pipeline after the HTML is approved. |
| P3 | `EDITORIAL_VISUAL_QA.md` (referenced by `pdf-status.md`) | Missing | Send it, or retire the reference. |

## 2. Overall reading

The report is careful and honest. The arithmetic is sound: every total, ratio and scenario on the economics sheets recomputes correctly (A$20.38 hurdle, A$214.5k first gate, both bills of materials, the EBITDA cases, the A$27.04 capital-return illustration). The withdrawal of the old A$380k, A$2.0m and A$16.20 figures is handled well. The exploration record (48 concepts, dossiers, dead ends) is the document's credibility, and **none of it was cut**.

The problems were presentation and labelling, not substance.

## 3. Ranked findings

| Rank | Finding | Severity | Pass 4 action |
|---|---|---|---|
| 1 | On screen, 89 to 90 of 93 sheets hid content at phone widths (up to 1,800px on the funding page); 4 dossier headings were cut off even at desktop | High | **Fixed** with screen-only CSS. 0 clipped at 320, 375, 1440px; print unchanged |
| 2 | 512 text elements failed WCAG AA contrast (grey labels at 2.9 to 4.4:1, mostly from opacity fades) | High | **Fixed.** Secondary grey darkened on light sheets (#7a7770 to #5f5d58), lightened on dark sheets (#8a8a88 to #9a9a98), fades removed from labels. Still near-monochrome; no new accent |
| 3 | Evidence vocabulary contradicted itself: sheet 15 headline said "3 levels: published, quoted, measured" beside a 4-class table; sheet 56 promised "quotation, measured result"; neither quotes nor measurements exist | High | **Fixed.** One scheme (below), stated on sheets 15, 56 and the contents page |
| 4 | Sheet 10 SAM and SOM rows showed unsourced gross values (A$41m, A$440k) and 15,000 panels in year one, contradicting sheet 40 ("SAM and SOM not established") and the A$30k first-gate feed budget | High | **Fixed.** Rows relabelled "not established" and "test batches" (class R); old values listed in the changelog |
| 5 | The A$485k fixed opex is a legacy allowance yet sets ~53% of the hurdle | High | **Flagged in place** (sheets 45, 47, 56); decision below |
| 6 | 28kg average mass disagrees with the report's own intake mix (~23kg) and is called the "midpoint" of 20 to 32kg (which is 26kg) | Medium | **Flagged in place** (sheets 47, 56); decision below |
| 7 | 19 charts had `role="img"` but no text alternative | Medium | **Fixed.** Each has a descriptive label |
| 8 | The brief requires the document to say it is a pre-feasibility and pilot-design study; cover and contents said only "pre-feasibility" | Medium | **Fixed** on cover and contents |
| 9 | "Single-file HTML" loads two sibling stylesheets (`_fonts.css`, `proposal-polish.css`) | Medium | **Not changed.** Decision below |
| 10 | Seven links point to `docs/*.md`, which will not exist on static hosting or in the PDF | Medium | **Not changed.** Decision below |
| 11 | `npm run build:html` fails from the pack as shipped (P1) | Medium | Reported |
| 12 | Sheet 02 said "48+ concepts"; the audit and every other page say exactly 48 | Low | **Fixed** |

## 4. The evidence scheme (reconciled)

The brief asks for three states at a glance; `DATA_POSITION.md` uses four labels; the report already used classes A to D. These are now one system:

| Mark | Class | Reads as | DATA_POSITION label |
|---|---|---|---|
| A (filled) | measured or contracted | evidenced; **none yet** | (none) |
| B (solid) | published | evidenced | Published |
| C (rounded) | third-party claim | evidenced as someone's claim | Claimed |
| D (dashed) | modelled | defined and scoped | Modelled |
| R (dotted) | required | open | Required |

Marks are letters in outlined boxes, so they survive greyscale print. They appear on headline figures from the contents page to the funding decision, on the assumption register, and on all 17 existing "Evidence status" lines in the appendices and dossiers.

## 5. Decisions needed from Blake

1. **A$485k fixed opex.** It sets A$10.78 of the A$20.38 hurdle. Each A$100k moves the hurdle A$2.22/panel; at the 30k/y stop line it becomes A$25.77. Replace with a roster and site quotes, or state a basis for keeping it.
2. **Average mass.** Choose 28kg with a stated reason, or recompute at the intake-mix figure (~23kg). This changes the 1.26kt/y feed, the 16.8t Brisbane payload and any weight-based freight allowance, not the per-panel hurdle arithmetic.
3. **SAM and SOM values.** If A$41m, ~1.4M panels, 31,000t, 15,000 panels and A$440k have a source and method, send it and they can return as class D with a basis line. Otherwise leave them out.
4. **Cover paragraph.** Marlowe's description ("about 1.2 million panels a year", "over 85% landfilled or crushed") comes from the lineage dossier and disagrees with the report (~2.0m retired now; 17% recycled; split not published). The report's figures are the sourced ones. Don't use the paragraph externally as written.
5. **Single file.** Either inline the two stylesheets at build time or restate the constraint as "one HTML file plus two stylesheets".
6. **Docs links.** Publish `docs/` beside the report, or cite the notes by name instead of linking.
7. **Appendix figures.** Pages 63 to 71 are correctly labelled as scenarios, but some figures are striking (47% silver cake, +A$15/panel freight dividend, A$45 second-life value). A peer reviewer will ask for the basis of each; attach sources where they exist.
