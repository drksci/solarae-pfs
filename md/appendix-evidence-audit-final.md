# Appendix evidence audit (sections 63–80)

**Compared with:** `docs/inspiration/CNC Silver Extraction Strategy.md` (line numbers below refer to that file).  The source is a design conversation and contains useful literature-backed comparators, but it repeatedly labels numbers as hypotheses, illustrative values, or things to assay.  A page should therefore distinguish *source-supported evidence* from a proposed test envelope and from a business assumption.

## Overall finding

The new dossier pages (72–77) are materially more disciplined than the application pages (63–71, 78–80): they use TEST/FAIL/PARTNER dispositions and state what must be measured. They preserve the central architecture—local release, intact glass where possible, selective silver liberation, concentration, and an external refiner. The previously missing source concepts are now explicit in compact concept ledgers on pages 72–76; the numeric and commercial caveats below remain active.

The most serious evidence problem is that pages 63–71 present invented-looking operational and commercial figures as if measured: cycle times, recovery percentages, prices, energy, lead levels, temperatures, flow rates, freight dividends, depot counts, capex and break-even prices. The source supports only a small subset of the recovery figures (97.6% Ag rougher recovery, ~32× upgrade, ~47 wt% Ag cleaner concentrate, ~86.5% retained Ag, 1.4% mass, 94.4% in <0.25 mm, and 61% liberation), and explicitly says to assay or reproduce them on representative feed (lines 79–89, 119–164, 186–202).

## Per-page corrections

### 63 — Intake & triage

- **Unsupported:** `<1.5 s`, ~4.2% quarantine, A$45/panel, “up to 15%” repowering feed, >80% Voc resale rule, ±0.2 mm profilometry, 5.0 mm bow threshold, and “three times intrinsic commodity value.” None appears in the source. The source says to reject unsuitable panel types automatically and record panel type, estimated yield, processing time and cartridge mass (lines 65–75, 99–105), but supplies no intake dataset or resale price.
- **Overconfident mechanism:** “flash IV sweep” and NIR lead-leaching detection are reasonable engineering additions, not source evidence. Mark as proposed instrumentation and add a validation requirement (false-positive/false-negative rate, electrical isolation, contaminated modules).
- **Missing reasoning:** retain the source’s frame/J-box removal and exposed-cell-sheet sequence (lines 16–40). Triage should explicitly determine whether the panel is suitable for whole-sheet delamination, surface skim, busbar/ribbon harvest, or rejection—not merely route to “resale vs delamination.”
- **Correction:** replace all hard figures with “illustrative test target” labels; add a small acceptance matrix: panel construction/age, front vs rear Ag location, intact second-life candidate, and hazardous/unknown feed.

### 64 — Mechanical baseline

- **Unsupported:** 42 kWh/t, 72% glass recovery, <A$15/t, >450 ppm Pb, the 16.5/68.0/1.2/14.3% mass balance, 0.08% Ag, and all commodity prices. The source only says whole-panel grinding creates a large silicon stream, warns against over-grinding, and cites 94.4% of Ag in <0.25 mm fines (lines 79, 156–164, 190–200).
- **Correction:** call this a *local baseline to measure*, not an Australian benchmark. Add feed basis, shredder screen size, dust losses, assay method, Pb partition and delivered buyer specifications. Do not imply “thousands of tonnes of road base” or hazardous classification without measured stream chemistry.
- **Missing comparator:** the source’s recommended cheap prototype is “vision → shallow abrasive removal → vacuum capture → particle classification” (lines 99–105), and its simpler one-axis feed + floating abrasive drum is important (lines 49–77). Put those beside the shredder baseline.

### 65 — Thermal shear bed

- **Unsupported/contradictory:** 65–85°C, 78% peel-force drop, 85→<18 N/cm, >92% intact glass, 18–25 mm/s and 72/88°C operating limits are not in the source. The source instead describes local softening, a heated zipper peel, 180° geometry and load-cell control (lines 585–637), and notes published hot-knife systems at roughly 40–60 s/panel with ~300°C blades (lines 641–668). It does not establish a universal 65–85°C EVA window or “eliminating” off-gas.
- **Correction:** label 60–85°C as a *proposed low-temperature programme envelope* and explicitly test backsheet/EVA families. Keep a separate comparator row for published ~130°C PET peel and ~300°C commercial hot knife; do not present these as interchangeable process conditions.
- **Missing mechanism:** the source’s 20–40 mm local heat strip, 20–30 mm flap, torque-controlled take-up roller and constant-peel-force controller (lines 607–625) should appear in the figure/table. Also mention fluorinated backsheet decomposition risk (lines 695–715).

### 66 — AI vision robotics

- **Unsupported:** 1.2 s scan, <85 s complete cycle, A$65/h labour and +A$28/h viability ceiling; <25 N and all tool traverse rates/99.97% containment are engineering targets, not source results. The source proposes a camera, floating Z, adjustable skim depth, automatic rejection and weighing (lines 43–77), not a validated 6-axis cell.
- **Overreach:** “decouples cycle time” and “future-proofing” are claims. Warped, dirty, cracked, bifacial and shingled modules are precisely the unvalidated cases; the source recommends a cheap 1-axis feed + CNC-Z architecture before full CNC/robotics (lines 49–77).
- **Correction:** make 6-axis robotics a challenger after a fixed/one-axis benchmark. Add tests for scan latency, dust fouling, registration error, tool reaction force, glass damage, intervention rate, uptime and maintenance cost. Remove the labour-dollar claim unless sourced to a plant model.

### 67 — Photothermal & NIR

- **Unsupported:** 850–1,050 nm, >90% transmission, 0.14 kWh/panel, 4× advantage, four seconds/75°C, 12 kWh oven comparator and “eliminating fire risks/off-gassing.” The source supports selective IR heating from the glass side and an estimated **US$0.22/module** for a laser-assisted study (lines 1713–1736), but also says optimum temperature must be determined and warns against broad heating.
- **Microwave correction:** 2.45 GHz and selective cell heating are source-supported (lines 2328–2355), but the source reports 500 W for 5 minutes reaching roughly 200–300°C in a patent experiment—not a 75°C, 4-second production cycle. Keep microwave as a guarded challenger with arcing/shielding/uniformity trips (lines 2430–2449).
- **Missing mechanism:** scanning microwave shoe, internal cell heating, pneumatic blister/vacuum peel and one-axis bar (lines 2361–2476) should be shown. Distinguish laser ablation of Ag from NIR assistance for delamination.

### 68 — Fluid scour & sensing

- **Unsupported:** 27.5 mN/m, 580 nm/365 nm, 60 fps, <4.5 L/panel, 95% recirculation, 5 bar, Mohs 6.5 and 1,600× flash expansion. The source discusses hot cavitating water, lateral hydraulic peeling, IR + cavitation + vacuum and acoustic/optical detection, but supplies no such formulation or operating numbers (lines 1798–1889, 1978–2082).
- **Correction:** present tracer/surfactant and autogenous silicon scour as hypotheses requiring foam, residue, wastewater and flotation-compatibility tests. Do not call Rhodamine “zero residue” or a formulation “environmentally benign” without an EHS assessment.
- **Missing mechanism:** source preference is hot water/cavitation **under** the backing, at shallow angle, to shear polymer—not abrasive scour of exposed Ag (lines 1872–1894, 2029–2060). The page should include a stop rule when the backing is gone and acoustic/optical sensing backs off pressure (lines 2082–2094).

### 69 — Beneficiation & flotation

- **Supported, with scope caveat:** ~32×, 47 wt% Ag, ~86.5% Ag recovery, 1.4% mass, and 61% liberation are consistent with source lines 79–89 and 119–164. The source says these are results from particular delaminated/ground PV-cell experiments, not guaranteed Solarae circuit performance.
- **Unsupported:** 0.1% feed grade, 0.6 mm ribbon aperture, >90% Pb capture, P80=103 µm, 7 wt% solids, reagent suite/doses, <10% moisture, and direct Nyrstar sale. Source says around 100 µm grinding, ordinary froth flotation and possible direct smelting subject to impurity specifications (lines 119–154, 204–224); it does not supply this flowsheet or buyer acceptance.
- **Correction:** label all Newcastle values “external comparator; reproduce on representative feed.” Add dry mass balance, Ag/Si/Pb/Cu/Sn assays, moisture, reagent consumption, tailings and payable/penalty terms. Preserve the source’s warning that selective skim feed is an engineering hypothesis to assay (lines 168–188).
- **Missing route:** source also ranks electrostatic and rejects gravity/magnetic as primary Ag separation (lines 190–202); add these as screened alternatives, not silently omit them.

### 70 — Regional logistics / CDS

- **Unsupported:** 22 kg/16 kg panel composition, A$14–18.50 freight, 600 km, +A$15/panel, <A$1.50 cake freight, 300+ depots, 500-panel trigger, 24 h campaign, A$450k capex, US$32/oz and US$18.50/oz break-even. None is in the source. Source says the prototype could be roughly $2–5k-ish and fit near two washing machines, but explicitly as an estimate (lines 99–107, 220–224).
- **Correction:** downgrade the mobile-CDS model to a scenario. Require route-specific payload, mobilisation, utilities, labour, permits, glass/Al buyer, concentrate settlement, downtime and reverse logistics. “Road base” is not an automatic product destination.
- **Missing source reasoning:** start with contracted repeatable batches and only add mobility after route density and product outlets are measured; retain the source’s “stop at concentrate / external refiner” architecture (lines 204–224).

### 71 — Export & domestic recovery

- **Generally sound framing:** unlike the other application pages, this page correctly excludes export revenue and says classification, permits, destination diligence and legal advice are required.
- **Unsupported:** A$3,500/container is still an unlabelled numeric anchor; make it explicitly illustrative and remove unless a quote is attached. “Local products may reduce transport” is a scenario, not evidence.
- **Missing source relevance:** source strongly prefers a mechanical front end and commercial refiner rather than in-house chemical refining (lines 91–103, 204–224). Add a domestic toll-refiner acceptance/assay gate before any export comparison.

### 72 — Dossier: cutting & physical entry

- **Good:** C01–C08 correctly separate proposed mechanisms from proof and identify bow, hidden interfaces, glass damage and tool wear as the central problem. This aligns with the source’s floating-Z, shallow skim and rejection logic (lines 43–77).
- **Missing source concepts:** add explicit rows for (1) laser debond + tacky roller (source lines 240–280), (2) interface undercut (283–340), (3) electrochemical scanning bar (344–383), (4) peelable film collector (387–415), (5) busbar-first harvest (451–470), and (6) ribbon stripping as a low-cost bulk harvest (474–495). C01 “CNC skimmer” is not enough to preserve these distinct options.
- **Correction:** C08 finger trench should state it is a selective-silicon-loss hypothesis and cite the source’s preference for laser over long mechanical finger paths (lines 419–447). Add a “front vs rear face” warning: older Al-BSF rear surfaces are predominantly Al (source lines 1041–1045).

### 73 — Dossier: heat & electromagnetic release

- **Good:** TEST framing, a 90°C proposed envelope, and the warning that heat is an assist—not release—are appropriately cautious.
- **Missing/under-specified:** include the source’s continuous heated zipper peel, sharp ~180° peel, local strip heater, load-cell force control and heated wire/roller variants (lines 585–725). Include induction blister + vacuum roller/air injection, self-heated panel, hot/cold line, vacuum-form backing and ultrasonic roller (lines 2108–2122).
- **Correction:** C17 “200°C release” must clearly be an external comparator, not a process option. C16 pyrolysis needs explicit HF/fluorinated-organic and off-gas treatment rationale (lines 695–715, 1784). C11 microwave should cite the source’s 500 W/5 min, 200–300°C patent comparator and distinguish it from a proposed local scanner (lines 2334–2355).

### 74 — Dossier: fluids, acoustics & phase change

- **Good:** the retained architecture (mechanical lift opens; water wets/cools/carries/observes) is faithful and the controls (foam, residue, wastewater, flotation compatibility) are valuable.
- **Missing:** source explicitly ranks hot cavitating water, dry ice, ice slurry, heat+cavitation, lateral hydraulic peeling, and an IR → hot cavitation → vacuum → collector sequence (lines 1798–1810, 1898–1936, 1940–1974, 1978–2094). Add each as a separate concept or cross-reference; C25 water jet currently collapses too much distinct mechanism.
- **Correction:** C20 “steam zipper” and C21 carbonated wedge should be framed as speculative variants of pneumatic/hydraulic crack propagation; source’s preferred mechanism is low-pressure warm air/water after a tiny opening (lines 1586–1711), not a generic phase-change claim. Include the source’s warning that ordinary dry ice may not remove mature cross-linked EVA quickly (lines 1926–1936).

### 75 — Dossier: force, fixtures & geometry

- **Good:** this is the most faithful page conceptually: supported work-bed, shortened crack front, load/displacement/acoustic measurement and stable-crack success criteria reflect source lines 585–637 and 1586–1644.
- **Missing:** add explicit 180° peel, constant-force feedback, the retained-frame option, and the source’s pneumatic zipper geometry. C29 “one-glass release” should link to the source’s intact front glass + cell/EVA sheet architecture (lines 499–553), not read as an unqualified “sacrifice.”
- **Correction:** “vacuum zipper” must state the required edge initiation and pad-grip failure modes. C34 blister inflation should cite the source’s need for a small puncture, regulated low pressure and pressure-versus-detached-area measurement (lines 1683–1711, 1774–1786).

### 76 — Dossier: recovery, concentration & refining

- **Good:** commercial proof, assay, moisture, penalties and external specialist disposition accurately preserve the source’s “stop at concentrate” logic (lines 204–224).
- **Missing/important:** C39 metal getter needs the full Ag→molten Pb→Ag–Pb→Pb electrorefining/Ag-rich slime or Parkes Zn phase sequence and the explicit lead hazards (lines 737–885). The source’s preferred low-cost variant is a recovered Sn–Pb wetted wheel, not an unspecified getter (lines 897–1039). C44 should mention toll refining, not only “industrial temperature.”
- **Correction:** retain 32×/47 wt%/86.5%/1.4% only as external comparator values, with feed-size and assay context (lines 119–164). C38 should require buyer acceptance and penalties before “saleable” is claimed. C40 bipolar cell can remain FAIL, but explain source did not propose it; otherwise mark as out-of-source extension.

### 77 — Dossier: systems, logistics & deployment

- **Good:** fixed/mobile/partner cases are correctly conditional; no mobile economics are asserted as results.
- **Missing:** source’s actual low-cost architecture is a one-axis feed plus floating abrasive drum/cyclone and a compact “couple of washing machines” selective-CNC + miniature flotation concept (lines 49–77, 220–224). Add it as the reference deployment before a container plant.
- **Correction:** C48 “not inherently unlawful” is a legal conclusion beyond the source’s technical conversation. Keep it as a diligence question: classification, permits, destination, treatment, freight and legal advice. Require named local buyers and route density before C46/C47 advance.

### 78 — Blades & peeling tools

- **Good:** the narrow technical requirement and TEST disposition are consistent with the source’s hot knife, zipper peel and compliant entry ideas (lines 503–505, 585–668).
- **Missing:** source distinguishes backsheet removal from front-glass/EVA removal and recommends scoring + flap + pinch rollers + local IR/PTFE heat + powered take-up + load-cell control (lines 607–625). Add this sequence and the 180° peel rather than leaving “hot knife” as a generic label.
- **Correction:** patent literature is evidence of a mechanism, not proof of this feed. Keep the page’s no-universal-claim language and add per-vintage residue/fume/glass-damage acceptance tests.

### 79 — Electrical processes

- **Good:** stopping high-voltage/buried-electrode front-end routes and partnering for specialist refining is directionally faithful to source lines 91–103 and 204–224.
- **Overconfident/incorrect scope:** “ARENA’s Swinburne programme >90% boron/phosphorus removal and >90% silver recovery in silicon” is not the central source result and is not enough to establish Ag refining, payable terms or this flow sheet. The source’s relevant specialist route is concentrate to a refiner; electrical/electrochemical scanning is a *front-end Ag liberation* concept (lines 344–383), not only downstream refining.
- **Correction:** separate “electrochemical scanning bar” (TEST front-end, source lines 344–383) from “specialist Si/Ag refining” (PARTNER). Do not imply the ARENA numbers validate the proposed regional product without source report scope and assay.

### 80 — AI disruptor robotics

- **Good:** 3D/NIR vision, adaptive tooling and scan fouling/slippage risks are reasonable engineering hypotheses; TEST labels are preferable to the page-66 claims.
- **Unsupported:** “<90 s,” ±0.5 mm, zero glass shattering, zero retooling and the named Fanuc/KUKA equivalence are not source results. Remove from the diagram or label as acceptance targets. “Cavitation jet” should be the source’s guarded heat+cavitation/vacuum architecture, not an assumed abrasive metallisation-scour tool.
- **Missing decision logic:** source recommends simple one-axis feed / floating head before a heavy XY/6-axis system (lines 49–77), and says a full robotic cell should be justified by throughput and panel variance. Add a fixed/one-axis comparator and a gate based on cycle time, uptime, intervention rate, dust/water handling, product assay and maintenance cost.

## Source concepts not represented anywhere clearly

1. One-axis feed + CNC-Z/floating abrasive drum, cyclone and automatic weighing/rejection (lines 49–77).
2. Laser Ag debond + tacky roller/continuous adhesive pickup film (lines 240–280, 387–415).
3. Local interface undercut and electrochemical scanning bar (lines 283–383).
4. Busbar-first harvest and controlled ribbon stripping, including the warning that fingers are brittle fired paste (lines 451–495).
5. The source ranking that favours laser/interface routes and busbar/ribbon stripping over whole-cell grinding (lines 540–555).
6. The complete liquid-metal architecture: Ag–Pb collector, Parkes alternative, hazards, and recovered Sn–Pb wetted wheel (lines 737–885, 897–1039).
7. Induction blister + air propagation/vacuum drum, self-heated panel and hot/cold travelling line (lines 2108–2122).
8. Microwave applicator inside the frame with choke/shield, one-axis feed, pneumatic blister and vacuum peel (lines 2328–2516).

These are now restored as explicit TEST/PARTNER/FAIL rows or cross-referenced in the dossier ledgers. The audit conclusion remains: **the dossier preserves the strategic thesis and the major concept branches, but application-page numeric claims still require evidence-label discipline before they can be presented as decision-grade.**

### Source-pass update · 11 September 2026

Pages 72–76 now carry compact ledgers for laser/roller, undercut, electrochemical scanning, peel film, busbar/ribbon harvest, heated zipper and 180° peel, induction/ultrasonic/microwave variants, cavitation/dry-ice/ice-slurry/hydraulic branches, force-feedback/retained-frame/blister geometry, and Ag–Pb/Parkes/Sn–Pb/electrostatic recovery concepts. Each is marked as TEST, FAIL or PARTNER with a plain next proof. Page 77 still carries the fixed/mobile/partner deployment comparison; its low-cost one-axis concept remains an explicit validation dependency rather than a claimed plant design.
