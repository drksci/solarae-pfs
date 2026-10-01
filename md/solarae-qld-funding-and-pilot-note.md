# Solarae: Queensland funding and the state recovery pilot

Prepared by Claude for Em and Blake, 17 September 2026. Proposed additions to sheet 44 (Funding and incentives), plus evidence from Queensland's completed solar panel recovery pilot that bears directly on the cost model.

Evidence marks follow the report's scheme: **B** published, **C** third-party claim or estimate, **D** modelled.

## 1. Proposed rows for sheet 44

| Pathway | Best fit | Caveat |
|---|---|---|
| QLD manufacturing grant | Future plant equipment, through an established Queensland manufacturer or recycler partner; matched grants of A$100k to A$1.5m | Applicant needs 3+ consecutive years of Queensland manufacturing, 5 to 200 FTE with at least 5 in Queensland, majority manufacturing turnover, ownership of the equipment and at least 50% co-funding. Not a first-gate route. Round 2 closes 25 November 2026. |
| QLD recovery pilot (SEC) | Published collection, cost, grading and reuse data; installer, logistics and recycler contacts | Evidence and partner lead, not funding. The state-funded pilot has finished. |

Ready to paste into the sheet 44 table body (row labels are under the audit's 28-character limit):

```html
<tr><th scope="row">QLD manufacturing grant</th><td>future plant equipment via an established Queensland manufacturer or recycler partner; matched A$100k–A$1.5m.</td><td>needs 3+ years of Queensland manufacturing, 5–200 FTE and 50% co-funding; not a first-gate route. Round 2 closes 25 Nov 2026.</td></tr>
<tr><th scope="row">QLD recovery pilot (SEC)</th><td><span class="ev" data-ev="B">B</span>published collection, cost, grading and reuse data; installer and recycler contacts.</td><td>evidence and partner lead, not funding; the funded pilot has ended.</td></tr>
```

And for the source line under the table:

```html
 · <a href="https://www.business.qld.gov.au/industries/manufacturing-retail/manufacturing/grant-programs">Qld manufacturing grants↗</a> · <a href="https://www.qld.gov.au/__data/assets/pdf_file/0037/656587/queensland-household-solar-panel-recovery-pilot-final-report-2025.pdf">Qld recovery pilot report↗</a>
```

The manufacturing grant row carries no evidence mark because it is a program description, not a figure in the case.

## 2. The Queensland Household Solar Panel Recovery Pilot

**What it was.** The Queensland Government funded the Smart Energy Council (SEC) with A$2.5 million over two years to pilot the collection, reuse and recycling of household solar panels. Consultation and design ran from December 2023; collections ran from August 2024 to 30 April 2025 (regional council drops to June 2025). The final report was published in September 2025. Delivery partners were New Limit Waste Services (collection and logistics); Pan Pacific Recycling, ACE Recycling and Sircel (recycling); Second Life Solar and CSIRO PV Labs (reuse testing); and Rexel/Ideal and Solar Shift (retail sites). A parallel commercial and utility-scale pilot is being reported separately.

**What it measured** (all class B unless marked):

| Topic | Finding |
|---|---|
| Panels handled | 18,082 household panels tracked end to end, 99.85% silicon |
| Age | 62% were 7 to 10 years old; 9% under 6 years |
| Best collection models | Installer-led: Consolidation Point (6,920 panels, 403 bookings, 55 businesses) and Back to Base (6,040 panels, 349 bookings, 56 businesses) |
| Weak models | Retail drop not recommended as run; resident-led models popular but costly, with high cancellations and breakage |
| Cost per panel, metro | A$43 to A$58 (logistics average A$28) |
| Cost per panel, regional | A$60.50 to A$75.50 (logistics average A$45.50) |
| Cost per panel, remote | A$70.50 to A$90.50 (logistics average A$55.50) |
| Cost structure | Logistics and handling above 60% of system cost; recycling A$10 to A$20 per panel regardless of location; admin, liability and IT excluded |
| Installer incentive | A$10 per panel, halved to A$5 with no drop in participation |
| Handling | Pallets carry 45 to 55 panels; 100 to 125% more efficient than stillages at sites with trained staff |
| Reuse | 5,067 panels visually graded reusable were tested; 2,200 passed EL/IV screening and 1,869 passed wet-leakage safety. About 29 in every 100 professionally collected panels are confirmed reusable |
| Newer panels | Panels made after 2020 failed testing more often |
| Material recovery basis | 21 kg average panel mass assumed |
| Processing capacity | About 240,000 panels a year theoretical Queensland capacity after two recyclers came online during the pilot |
| After the pilot | Recyclers saw substantial falls in household panel volumes once free collection ended |
| Annual household volume | 600,000 to 800,000 panels a year in Queensland (**C**: SEC's modelled estimate, supported by interviews, not a count) |
| Recycling rate | Under 5% in Queensland (**C**: participant consensus) |
| Licensing | State and council licensing can add 6 to 12 months to scaling |

## 3. What this means for Solarae

These are the points Blake should reconcile. None changes the report until he decides.

1. **Collection cost is the biggest gap.** The model allows A$6.40 per panel for collection. The pilot's observed metro logistics averaged A$28 per panel, and regional A$45.50. At A$28, the cash hurdle would be about A$41.98 per panel instead of A$20.38 (**D**: A$28 + A$1.80 + A$1.40 + A$10.78). The model either needs a stated reason why its collection will cost a quarter of the pilot's (feed delivered by a customer, a stewardship scheme paying collection, dense aggregated lanes), or a higher allowance.
2. **The revenue benchmark is lower than the hurdle.** Pilot recyclers were paid A$10 to A$20 per panel for processing. Solarae's A$20.38 hurdle sits above that range before any capital return. The report's case therefore rests on product value or a higher service fee, which should be said plainly.
3. **Feed depends on someone paying.** Household volumes to recyclers fell after the funded collection stopped. That supports the report's "signed feed first" stance and suggests installers and stewardship funding, not households, are the realistic feed source.
4. **Installers are the channel.** The two installer-led models delivered 72% of tracked panels. A first-gate feed contract is most likely to come from installer consolidation points.
5. **Mass supports the ~23 kg reading.** The pilot used 21 kg per household panel. This strengthens the audit's flag on the 28 kg basis.
6. **Reuse is far lower than visual grading suggests.** Only about 29% of professionally collected panels were confirmed reusable, against roughly 80% on visual grading. Appendix sheet 63's "divert: resale (80%)" should be read against this.
7. **Competition and capacity.** Three recyclers served the pilot around Brisbane, with about 240,000 panels a year of theoretical capacity against SEC's 600,000+ estimate. That capacity gap supports the opportunity; the incumbents are also potential partners, buyers or competitors.
8. **Better citation.** Sheets 40 and 41 cite the pilot second-hand through the 2026 WMRR submission. Cite the primary report instead, as class B.

## 4. Suggested next steps

1. Reconcile the A$6.40 collection allowance against the pilot's cost tables before the next investor conversation.
2. Add the two rows to sheet 44 and cite the primary pilot report on sheets 40, 41 and 44.
3. Approach SEC and New Limit Waste Services for installer consolidation-point data and a possible first-gate feed batch.
4. Leave the manufacturing grant until the plant gate, or pursue it through a Queensland manufacturer or recycler partner. A Queensland Manufacturing Hub can confirm eligibility early at no cost.

## Sources

- Smart Energy Council, *Queensland Household Solar Panel Recovery Pilot: Final Report*, September 2025. https://www.qld.gov.au/__data/assets/pdf_file/0037/656587/queensland-household-solar-panel-recovery-pilot-final-report-2025.pdf
- Queensland Government, Smart Energy Council solar panel and home battery recovery pilots (updated 22 December 2025). https://www.qld.gov.au/environment/waste-reduction-recycling/funded-initiatives/smart-energy-council
- Queensland Government ministerial statement, Transforming Queensland Manufacturing Grant Program opening, 5 February 2026. https://statements.qld.gov.au/statements/104444
- RSM Australia, TQMGP eligibility summary, February 2026. https://www.rsm.global/australia/insights/government-grant/transforming-queensland-manufacturing-grants-program-tqmgp
- Australian Manufacturing, round 2 announcement (closing 25 November 2026). https://www.australianmanufacturing.com.au/almost-80m-manufacturing-grants-open-to-queensland-businesses/
- Business Queensland, Manufacturing grant programs. https://www.business.qld.gov.au/industries/manufacturing-retail/manufacturing/grant-programs

Eligibility details come from program summaries; check the official round 2 guidelines before relying on them.
