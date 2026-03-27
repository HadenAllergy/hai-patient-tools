# HAI Patient Handout Pipeline — MANIFEST
## Last updated: March 27, 2026

### How to use this file
Update a row each time a handout moves through a pipeline stage. Statuses: `pre-protocol` → `validated` → `polished` → `deployed`. Keep in your GitHub repo or laptop. Do NOT upload to Claude sessions — the handoff references it, Claude doesn't need it.

---

## Currently on GitHub (hai-patient-tools/content/handouts/)

| Filename | Domain | Validated? | Grade | Polished? | Status | Notes |
|----------|--------|-----------|-------|-----------|--------|-------|
| allergic_shiners.html | Derm | No | — | No | pre-protocol | |
| anaphylaxis_2025_update.html | Urticaria/Anaph | Mar 26 | B | No | validated | 3 MOD — corrections + voice needed |
| autoimmune_urticaria.html | Urticaria | Mar 26 | B | No | validated | 3 MOD — corrections + voice needed |
| bp_medication_reactions.html | Drug Allergy | No | — | No | pre-protocol | |
| cholinergic_urticaria.html | Urticaria | Mar 26 | B | No | validated | 4 MOD — corrections + voice needed |
| cold_urticaria.html | Urticaria | Mar 26 | B | No | validated | 3 MOD — corrections + voice needed |
| covid19_urticaria.html | Urticaria | Mar 27 | B | No | validated | 2 MOD — corrections + voice needed |
| dermatitis_vs_urticaria.html | Derm/Urticaria | No | — | No | pre-protocol | |
| dermatographic_urticaria.html | Urticaria | Mar 27 | B+ | In-session | validated | Corrections applied in validation (lane break) — re-validate |
| hae_hereditary_angioedema.html | Angioedema | No | — | No | pre-protocol | |
| hives_and_hormones.html | Urticaria | Mar 27 | B | No | validated | 3 MOD — corrections + voice needed |
| hives_and_stress.html | Urticaria | No | — | No | pre-protocol | |
| hives_in_kids.html | Urticaria | No | — | No | pre-protocol | |
| idiosyncratic_medication_reactions.html | Drug Allergy | No | — | No | pre-protocol | |
| large_local_insect_reactions.html | Venom/Insect | No | — | No | pre-protocol | |
| mcas_vs_csu.html | Mast Cell | Mar 26 | A- | No | validated | 2 MOD — minor revisions + voice |
| nsaids_and_angioedema.html | Drug Allergy | No | — | No | pre-protocol | |
| physical_urticarias_umbrella.html | Urticaria | Mar 27 | B+ | In-session | validated | Corrections applied in validation (lane break) — re-validate |
| pregnancy_hives_mast_cell.html | Urticaria | No | — | No | pre-protocol | |
| shingles_skin.html | Derm | No | — | No | pre-protocol | |
| sjs_ten_dress.html | Drug Allergy | No | — | No | pre-protocol | |
| solar_urticaria.html | Urticaria | No | — | No | pre-protocol | |
| understanding_nsaids_acetaminophen.html | Drug Allergy | No | — | No | pre-protocol | |
| understanding_your_rash.html | Derm | No | — | No | pre-protocol | |
| urticaria_angioedema_foundational.html | Urticaria | Mar 26 | B+ | No | validated | 4 MOD — corrections + voice needed. START HERE. |
| urticaria_pigmentosa.html | Mast Cell | No | — | No | pre-protocol | |
| vertigo_dizziness.html | ENT | No | — | No | pre-protocol | |

**Summary:** 11 validated (9 need voice rewrite, 2 need re-validation) | 16 pre-protocol

---

## Coverage Gap Handouts (not yet written)

| Topic | Domain | Priority | Status | Notes |
|-------|--------|----------|--------|-------|
| Alpha-Gal Syndrome | Food Allergy | HIGH #1 | not started | Endemic in Texas. Critical gap. |
| AERD / Samter's Triad | Asthma/ENT | HIGH | not started | Nasal polyps + asthma overlap |
| Biologic Medications Overview | Multi | HIGH | not started | Omalizumab, dupilumab, mepo, benra, teze |
| Drug Allergy Evaluation / Penicillin Delabeling | Drug Allergy | HIGH | not started | High referring-physician value |
| Hereditary Alpha-Tryptasemia (HαT) | Mast Cell | HIGH | not started | Flagged in MCAS validation |
| Sublingual Immunotherapy (SLIT) | Immunotherapy | HIGH | not started | No handout exists |
| Occupational Asthma | Asthma | MEDIUM | not started | |
| Drug Desensitization | Drug Allergy | MEDIUM | not started | |
| EoE / Eosinophilic GI Umbrella | GI | MEDIUM | not started | Individual EoE files exist on laptop |
| CRS with/without Nasal Polyps | ENT | MEDIUM | not started | |
| OIT for Food Allergy | Food Allergy | MEDIUM | not started | |
| FPIAP | Food Allergy/Peds | MEDIUM | not started | FPIES exists, FPIAP does not |
| Latex Allergy | Contact/Occup | MEDIUM | not started | |
| When to See an Immunologist | Immunodeficiency | MEDIUM | not started | Referring physician screening tool |
| IgG Subclass Deficiency | Immunodeficiency | MEDIUM | not started | |

---

## Domain Decision Trees (build when 5+ validated handouts exist per domain)

| Domain | Handouts Available | Tree Built? | Notes |
|--------|-------------------|-------------|-------|
| Urticaria / Angioedema / Mast Cell | 11 validated | Yes (prior session) | Routing landing page exists |
| Drug Allergy / Reactions | 5 on GitHub (pre-protocol) | No | Build after Phase 2 validation |
| Food Allergy / Intolerance | ~15 on laptop (raw) | No | Build after Phase 3-4 |
| Asthma / Pulmonary | ~15 on laptop (raw) | No | Build after Phase 3-4 |
| Contact Dermatitis | ~15 on laptop (raw) | No | Build after Phase 3-4 |
| Immunodeficiency | ~6 on laptop (raw) | No | Build after Phase 3-4 |
| Venom / Insect | ~5 on laptop + 1 GitHub | No | Build after Phase 2-3 |
| ENT | ~10 on laptop + 1 GitHub | No | Lower priority |
| Derm (non-urticaria) | ~12 on laptop + 2 GitHub | No | Lower priority |

---

## Pipeline Phase Tracker

| Phase | Description | Status | Sessions Est. |
|-------|-------------|--------|---------------|
| 1 | Voice rewrite validated batch (9 handouts) | READY | ~10 |
| 1b | Re-validate Phys/Derm corrections | READY | ~1 |
| 2 | Validate remaining GitHub handouts (~15) | READY | ~8 |
| 3 | Builder polish raw laptop drafts (~120-140) | BLOCKED on dedup | ~80-95 |
| 4 | Validate polished drafts | After Phase 3 | ~60-70 |
| 5 | Write + validate new gap handouts | Anytime | ~20-30 |
| 6 | Corrections + re-validation | Ongoing | ~40-50 |

---

*HAI Pipeline MANIFEST v1.0 — March 27, 2026*
