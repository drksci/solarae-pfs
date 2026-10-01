# Solarae research and source register

Pass 3, researched 17 September 2026 (all sources accessed that day).

Scope: **general methods and practice only.** No source below is about Solarae, and nothing here is a Solarae fact. The workflow files cite these IDs.

Quality key: **Primary** = standard-setter or original author. **Secondary** = reputable summary of a primary. **Tertiary** = convenience reference; verify before relying on it.

## Sources used

| ID | Source | Type | Quality | Used for | Used in |
|---|---|---|---|---|---|
| R1 | d/rksci, "How to Measure a Site Acquisition Pipeline", published research note, 19 Aug 2026. https://drksci.com/research-how-to-measure-a-site-acquisition-pipeline | Method note | Primary (Blake's own house method) | Measured/derived/assumed/unknown states; source, as-of and learned dates, licence and provenance fields; "does not claim" section; proceed/revise/stop ending; "Read as" line under diagrams | evidence-standard 1, 4, 6; figure-standard 2; plan 3; scaffold |
| R2 | IPCC, Guidance Note for Lead Authors of the AR5 on Consistent Treatment of Uncertainties (Mastrandrea et al. 2010). https://www.ipcc.ch/site/assets/uploads/2017/08/AR5_Uncertainty_Guidance_Note.pdf | Guidance | Primary | Calibrated confidence and likelihood framework | evidence-standard 3 |
| R3 | "Combining probability with qualitative degree-of-certainty metrics in assessment", *Climatic Change* (2018), via PMC. https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12078392/ | Peer-reviewed article | Secondary | Five confidence levels; "unlikely" = 0–33%, "very unlikely" = 0–10% | evidence-standard 3 |
| R4 | GreenFacts summary of IPCC AR5 WG1. https://www.greenfacts.org/en/climate-change-ar5-science-basis/l-3/1-likelihood.htm | Summary | Secondary | Confidence rests on type, amount, quality and consistency of evidence plus agreement | evidence-standard 3 |
| R5 | Wilke, *Fundamentals of Data Visualization*, ch. 22 "Titles, captions, and tables". https://clauswilke.com/dataviz/figure-titles-captions.html | Book (open access) | Primary | Title as first part of caption; titles state the point | figure-standard 2 |
| R6 | W3C WAI, Images Tutorial: Complex Images. https://w3c.github.io/wai-tutorial-images/tutorials/images/complex/ | Guidance (draft preview of the published tutorial) | Primary | Two-part text alternative; long description available to everyone | figure-standard 3 |
| R7 | Clemson University, Complex Images. https://www.clemson.edu/accessibility/digital/concepts/complex-images.html | University guidance | Secondary | Offer chart data in an accessible table | figure-standard 3 |
| R8 | W3C, Understanding SC 1.4.11 Non-text Contrast. https://www.w3.org/WAI/WCAG22/Understanding/non-text-contrast.html, with Deque's summary https://dequeuniversity.com/resources/wcag2.1/1.4.11-non-text-contrast | Standard | Primary | 3:1 for graphical objects such as chart lines and bars | figure-standard 3; plan 9 |
| R9 | DigitalA11Y, Understanding SC 1.4.11. https://www.digitala11y.com/understanding-sc-1-4-11-non-text-contrast/ | Summary | Secondary | 4.5:1 for text in or over graphics | figure-standard 3; plan 9 |
| R10 | SciFig, Okabe-Ito hex reference (Jul 2026). https://scifig.ai/blog/okabe-ito-color-palette-hex-codes | Reference | Tertiary | The eight hex codes | figure-standard 4 |
| R11 | Sci-draw, Okabe-Ito reference (Jun 2026). https://sci-draw.com/blog/colorblind-safe-palettes-okabe-ito-reference; and conceptviz citation of Okabe & Ito (2008) and Wong (2011) *Nature Methods* 8(6):441 | Reference | Tertiary, pointing to primary | Palette origin and CVD design; verify-in-simulator advice | figure-standard 4 |
| R12 | Conceptviz, scientific colour palettes (Jan 2026). https://conceptviz.app/blog/scientific-color-palette-for-research-papers-and-posters | Blog | Tertiary | Viridis for continuous data | figure-standard 4 |
| R13 | Wilke, *Fundamentals of Data Visualization* (O'Reilly 2019), as excerpted on Goodreads. https://www.goodreads.com/book/show/40014286-fundamentals-of-data-visualization | Book excerpt | Primary text, secondary host | Colour matching breaks down at 8–10 categories; table layout rules | figure-standard 4, 5 |
| R14 | Australian Government Style Manual, "The basics of plain language" (2023). https://www.stylemanual.gov.au/blog/basics-plain-language | Government guidance | Primary | Understanding users comes first | plan 1 |
| R15 | Australian Government Style Manual, writing guidance. https://www.stylemanual.gov.au/node | Government guidance | Primary | Headings state the point and lead with keywords; Australian English | plan 4 |
| R16 | As R14 | Government guidance | Primary | One idea per paragraph; subject–verb–object | plan 4 |
| R17 | Australian Government Style Manual / APSC Government Writing Handbook, "Keep it simple: plain language". https://www.stylemanual.gov.au/about-style-manual/government-writing-handbook/section-2-write-so-your-meaning-clear/keep-it-simple-plain-language | Government guidance | Primary | Short words; explain jargon; glossary for long technical documents | plan 4 |
| R18 | WCAG 2.2 SC 1.4.10 Reflow, via summary. https://medium.com/@michaelmoubani/wcag-2-2-accessibility-guide-34927b655913 | Summary | Tertiary | Reflow without sideways scrolling at 400% zoom. The 320 CSS px test width is the W3C-specified equivalent; **verify against the W3C Understanding page**, which wasn't opened this pass | plan 9; checklist |
| R19 | As R18 | Summary | Tertiary | Data tables are an allowed exception to reflow | plan 9 |

## Searches that found nothing usable

| Search | Result | What it means |
|---|---|---|
| "Solarae report drksci" | Unrelated results (malware reports, a scam-checker page for a similarly named site, fiction). Nothing about this project. | No public Solarae material to draw on. None of those results were used. |
| d/rksci research index, checked 17 Sep 2026 | Solarae isn't listed. | Solarae is either unpublished or published under another name. |

## Context research blocked

The "Why it matters now" section can't be researched until the report says what Solarae is. To clear it, see audit item M9.

## Pass 4 additions (17 September 2026)

No new external sources were used. Pass 4 relied on the project's own files and on tools:

| ID | Item | Type | Used for |
|---|---|---|---|
| T1 | `research/research-notes.md`, `research/research-lineage-dossier.md`, `research/docs/financial-model-rebuild-2026-09-11.md` (pass-4 pack) | Project registers | Confirming the A$485k legacy status and the 28kg basis; tracing the 1.2m and 85% figures to the dossier |
| T2 | axe-core 4 (Deque), run in headless Chromium | Accessibility test engine | WCAG 2 A/AA checks before and after |
| T3 | Playwright with Chromium | Rendering | Clipping measurements at 320, 375, 1440px and A4 print; local PDF render |
| T4 | The report's own `audit-html.mjs` | Project tooling | Structural audit |

The pass-3 note R18 (320px reflow basis) is unchanged: still to verify against the W3C Understanding page.
