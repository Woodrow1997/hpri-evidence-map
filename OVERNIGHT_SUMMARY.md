# OVERNIGHT SUMMARY
**Date:** June 5, 2026  
**Review URL:** https://woodrow1997.github.io/hpri-evidence-map/framework.html

---

## What Happened Tonight

Three tasks completed: framework redesign, expanded taxonomy, and deploy.

---

## TASK 1: framework.html — Integrative Redesign

### What changed

**Old design:** Five stacked vertical layer blocks (L1 → L2 → L3 → Experience/Prevention → L4 → Outcomes). Layer 1 was a single card: "Public Attitudes & Political Will."

**New design:** A two-column integrative layout — cross-cutting horizontal sidebar (left) + main causal flow (center).

### Specific architectural changes

**Layer 1 split into two distinct cards (side-by-side):**
- **Layer 1A — Public Opinion & Narrative:** What citizens believe, stigma, framing effects, media, moral attributions
- **Layer 1B — Political & Economic Power:** Real estate lobbies, Cicero Institute, corrections interests, developer coalitions
- A floating "↔ Often in direct conflict" label bridges the two cards — the key insight that sympathetic public opinion + hostile power structures = criminalization

**Three cross-cutting forces added as a left sidebar (vertical bands that span the full diagram height):**
- ⏳ **History & Time** — cumulative disadvantage, 1978 federal disinvestment, life course compounding
- 📍 **Place & Geography** — spatial concentration, NIMBYism, transit access, residential segregation
- 🌡️ **Climate & Displacement** — wildfires, extreme heat, flooding, climate-induced housing loss

**Cross-cutting legend below the diagram** — three clickable cards explaining each force with key research questions tagged by evidence strength.

### Modal content updated for:
- `l1-opinion` — public opinion formation, framing research
- `l1-power` — Cicero Institute, real estate lobbies, criminalization infrastructure
- `l2` — now includes financialization of housing
- `crosscut-history` — Reagan cuts, cumulative disadvantage, Dannefer/Elder frameworks
- `crosscut-place` — Kain spatial mismatch, Fischel Homevoter, NIMBYism
- `crosscut-climate` — UCLA 2026 climate-homelessness study, JAMA heat mortality data

### Coverage bars updated:
- Added "History, place, climate" row (5% — Emerging research)
- Updated "Public opinion & power" to reflect split framing

### What stayed the same:
- USC cardinal (#990000) and gold (#FFCC00) color scheme
- River/flow metaphor and bold public-facing language
- All JS modal functionality, coverage bar animations
- All existing layer cards (L2, L3, Experience, Prevention, L4, Outcomes)

---

## TASK 2: Expanded Research Catalogue Taxonomy

### Summary

Added **15 new topic nodes** to the framework taxonomy. Each topic was:
1. Searched against the 579-entry HPRI catalogue using keyword matching
2. Supplemented with 3–5 landmark field papers sourced via web research

### Files created
- `data/topic_papers_expanded.json` — all 47 topics (32 original + 15 new), with HPRI matches flagged `{"source": "hpri"}` and field papers flagged `{"source": "field", "landmark": true}`
- `data/field_landmarks.json` — just the 46 new landmark papers found, organized by topic

### Per-topic breakdown

| Topic ID | Question summary | HPRI matches | Landmarks |
|----------|-----------------|-------------|-----------|
| geo-t1 | Spatial concentration & neighborhood geography | 11 | 3 |
| geo-t2 | NIMBYism & local land use politics | 1 | 4 |
| geo-t3 | Transit access & urban design | 33 | 3 |
| time-t1 | Cumulative disadvantage across life course | 14 | 3 |
| time-t2 | Federal housing disinvestment since 1970s | 6 | 4 |
| climate-t1 | Climate disasters & homelessness | 7 | 3 |
| climate-t2 | Extreme heat & homeless health | 1 | 3 |
| power-t1 | Real estate/political interests & policy | 5 | 3 |
| power-t2 | Think tanks & criminalization advocacy | 9 | 3 |
| global-t1 | International comparisons (Finland, Canada, UK) | 31 | 3 |
| econ-t1 | Financialization of housing | 6 | 3 |
| econ-t2 | Labor market restructuring & gig economy | 1 | 3 |
| cap-t1 | Capability/flourishing framework | 3 | 4 |
| race-t1 | Racial capitalism & homelessness disparities | **0** | 4 |
| race-t2 | Racially-targeted interventions | 1 | 3 |

**Total field landmark papers found: 46**

### Topics where HPRI catalogue had ZERO matches (real gaps)

**`race-t1` — How does racial capitalism explain racial disparities in homelessness?**

This is the most significant gap. Zero matches in the 579-entry catalogue for terms like "racial capitalism," "structural racism," "antiblack," or "racial disparity" in the context of theoretical explanation. Note: There ARE papers on racial disparities in the catalogue — but they don't use a racial capitalism framing. This represents a genuine theoretical gap in HPRI's current coverage, and is where the Willse, Vitale, and Olivet/Dones field landmark papers are most important.

Landmark papers added for this gap:
- Willse (2015) — *The Value of Homelessness* — racial capitalism framework
- Olivet et al. (2021) — *Who Are the Homeless?* — anti-Black racism centering
- Greer et al. (2025) — Black-White disparities geographic variation (Springer)
- Padgett et al. (2022) — *Race Matters* scoping review (HPRI paper, added as field landmark)

### Other thin topics (1 match)
- `geo-t2` (NIMBYism): 1 match — Menendian et al. (2024) on single-family zoning in CA
- `climate-t2` (extreme heat): 1 match — PATHS study mentions heat
- `econ-t2` (gig economy/wage inequality): 1 match — income inequality study

---

## TASK 3: GitHub Deployment

- **Commit:** `7d82d51` — "Integrative framework redesign + expanded catalogue taxonomy"
- **Branch:** `main`
- **Remote:** `https://github.com/Woodrow1997/hpri-evidence-map.git`
- **Push:** ✅ Successful

**GitHub Pages URL:** https://woodrow1997.github.io/hpri-evidence-map/framework.html  
*(Allow 1–2 minutes for GitHub Pages to rebuild)*

---

## Things to Review in the Morning

1. **The two L1 cards side-by-side** — does the visual tension ("↔ Often in direct conflict") land clearly? The key insight is that sympathetic public + hostile power = criminalization, and this needs to be legible at a glance.

2. **The cross-cutting sidebar height** — on large screens, the three sidebar bands (History, Place, Climate) should span the full diagram height. On mobile they collapse to horizontal strips. Worth checking on different screen sizes.

3. **race-t1 gap** — this is real and worth discussing. The HPRI catalogue has papers on racial disparities but not papers that theorize them through a racial capitalism lens. Do you want to add any HPRI work that addresses this, or commission a literature review on racial capitalism and homelessness?

4. **geo-t2 (NIMBYism)** — also very thin in the catalogue (1 paper). The Rothstein *Color of Law*, Fischel *Homevoter Hypothesis*, and Shertzer et al. zoning paper are all field landmarks, but none are in the HPRI catalogue. Worth curating this section.

5. **`field_landmarks.json`** — 46 total landmark papers organized by topic. These are all non-HPRI papers recommended for the evidence map as "field context." At some point it might be worth deciding whether to link these out to the main index or keep them as background context.

---

*Completed overnight by Mark, June 5 2026*
