VW After the Capacity Cuts

Capacity cuts bought time, not competitiveness: Volkswagen's next move on unit cost.

A business strategy case study on how Volkswagen should respond to Chinese electric-vehicle imports after the EU's October 2024 anti-subsidy duties. The project combines public trade data (Eurostat), company filings and press releases, and a transparent set of estimates to reach one recommendation, delivered as a 12-minute board-level presentation.

The question

VW has cut capacity and costs, yet its own Passenger Cars brand earned a 2.4% operating margin in H1 2026 against a 6.5% target. Chinese EV imports have recovered despite the duties. What closes the remaining gap?

The answer in one sentence

Announced savings are not closing VW's margin gap while Chinese imports return, so VW should cut entry-segment unit cost through shared platforms and external battery and software partners.

Key findings
Finding	Evidence
The margin gap is large	VW Passenger Cars 2.4% (3.8% before special items) vs a 6.5% target; Škoda earns 8.5%
Duties slowed imports, then imports recovered	Chinese EV imports fell 20% after the duties (35,648 to 28,518 cars a month), then reached 36% above the pre-duty level in 2026 (48,395 a month)
Even with duties, import prices land near VW's entry price	Average customs value per car fell 29% to about €15,600; with 27% duties, about €19,700 against the VW ID. Polo at €21,004 ex-VAT and the BYD Dolphin Surf at €19,739
Reported savings are large but not yet visible in the margin	About €18B a year reported saved in 2025 (press), yet the Group margin is 3.8%
A unit-cost program is estimated to save about €490 to €2,090 per entry car	Four levers: shared platform, external software partner, lower-cost battery, sourcing. Equivalent to 0.2 to 1.2 margin points on VW Passenger Cars, or 4% to 29% of the gap

The main limit of the recommendation is stated in the work itself: entry cars alone close at most about a third of the gap, so the approach has to extend to higher-volume models.

Repository contents
File	What it is
VW After the Capacity Cuts.pptx	The final presentation: a cover and 10 slides structured as WHY, WHAT, HOW and a decision slide, with speaker notes
Presentation script_ Capacity cuts bought time, not competitiveness.docx	Word-for-word script for every slide, timing plan, audience checkpoints and prepared answers for the Q&A
Unit-cost program_ reasoning behind the estimates.docx	How each per-car estimate was built: formulas, sourced inputs, labelled assumptions, limits and sources
Charter & WBS_ VW After the Capacity Cuts (1).docx	Project charter and work breakdown structure: objectives, deliverables, success criteria, data plan, risks and the work plan
vw_casestudy_clean_code.pdf	Export of the Python (Jupyter) notebook that cleans the trade data and produces every chart and number used in the talk
Data and method

Trade data. Eurostat Comext dataset DS-045409: monthly EU imports of battery-electric cars from China (CN8 codes 87038010 and 87038090), January 2019 to August 2026, by member state. The EU aggregate is dropped to avoid double counting, and implausible rows (very low value or weight per car) are flagged and excluded. Periods are compared as the 12 months before the duties, the period after, and 2026 to date; October 2024, the transition month, is excluded from averages.

Company and market sources. VW Group Annual Report 2025, VW press releases no. 68/2026 and 69/2026 (H1 2026 results), VW newsroom, VW and BYD websites for entry-model list prices, press reports for savings figures (electrive), and BloombergNEF and UBS findings for battery and cost benchmarks.

Estimates. VW does not publish savings by lever, so each per-car figure is a team estimate built from published inputs plus assumptions that are labelled and can be changed. Every input is recorded with its type (sourced, assumption) and source. Levers overlap, so the program total applies an overlap haircut rather than adding them.

Limitations

Stated openly, because they affect how the results should be read:

The per-car savings and the investment ceiling are estimates, not VW data. They depend on assumptions such as the platform share of R&D, the overlap between levers and the entry volume.
Customs value excludes duty, VAT, shipping and dealer margin, and covers all China-origin makers, not only BYD. The 27% duty used is BYD's rate; other makers pay more or less.
The €15B and €18B savings figures come from press reports, not VW releases. The VW brand's 6.5% target was set in 2023 and has not been checked for restatement.
Some benchmark figures were read from press summaries of the BNEF and UBS reports, not the original reports.
Authors

Ben An, Dan Mosu, Kai Clancy, Kate Bloom and Priyanka Govani.

Project completed for a business strategy course, October 2026. This is an academic exercise using public information; it is not affiliated with or endorsed by Volkswagen AG or any other company named.

<!-- Optional: once the notebook and data are added to the repository, paste a section like this. ## Reproducing the analysis 1. Place the Comext export in `data/raw/comext/`. 2. Run `vw_casestudy_clean.ipynb` top to bottom (Python 3, pandas, matplotlib). 3. Charts and `key_numbers.csv` are written to `data/exhibits/`; inputs are in `data/inputs/`. -->
