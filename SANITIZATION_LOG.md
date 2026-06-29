# Sanitization log — QAD fibre demo v0.3.0 (2026-06-29)

**Source file:** `H:/QAD-HTML/dashboards/qad_live_dashboard_fibre_v2.4_2026-06-29.html` (101,051 bytes, ~1789 lines)
**Source samples:** `H:/QAD-HTML/dashboards/qad_real_samples.js` (2,083,479 bytes; 9 source datasets)
**Output index.html:** `index.html` (83,076 bytes)
**Output samples.js:** `qad_real_samples.js` (1,512,788 bytes — 5 fibre datasets only, finance datasets stripped)
**Tagged copy:** `qad_fibre_demo_v0.3.0_2026-06-29.html` (same as index.html, version-tagged filename per `feedback_versioned_artifacts_in_github.md`)

**Total redactions logged:** 51

## Per-rule redactions (in order applied)

| # | Rule | Source line | Removed | Replaced with |
|---|------|------------:|---------|---------------|
| 1 | A: title | ~200 | `TDC NET` | `Fibre Demo (generic)` |
| 2 | B: top live bar (BOHB version + trial count) | ~0 | `v2.4 live · 9298 trials` | `Demo snapshot · 2026-06-29` |
| 3 | C: TDC NET logo + header text + cluster URL | ~0 | `tdc_net_logo.png / TDC NET pilot / qad.<client>.eu-de.cloud.ibm.com` | `CoQu only / generic demo` |
| 4 | D: trial count in PR-AUC KPI | ~0 | `95% CI · Master locked · n_complete=1206` | `95% CI · production model locked` |
| 5 | E: BOHB live SQLite version | ~493 | `v2.4 (fibre) · BOHB live SQLite` | `Fibre model (locked)` |
| 6 | F: BOHB-tuned weights heading | ~0 | `BOHB-tuned weights` | `calibrated ensemble weights` |
| 7 | G1: drift panel header | ~0 | `vs locked Master config` | `vs locked production config` |
| 8 | G2: drift explanation (BOHB / micro-BOHB) | ~0 | `current optimal BOHB axes / rolling 7-day micro-BOHB / locked Master config` | `rolling 7-day estimate / tuned hyperparameter / locked production config` |
| 9 | H1: BOHB configuration header | ~0 | `Locked Master BOHB configuration` | `Locked production configuration` |
| 10 | H2: 31-axis BOHB footnote | ~0 | `31-axis BOHB on the NumPy surrogate` | `hyperparameter search on a classical reference` |
| 11 | I: Phase 4 git tag + __version__ | ~0 | `BOHB_v2.4_2026-06-29 · qad __version__ = "0.2.4"` | `Demo snapshot · 2026-06-29` |
| 12 | J: Phase 4 description (TDC NET deck / v2.4-locked) | ~0 | `TDC NET deck / v2.4-locked / HPC pipeline / 10 min QPU time` | `fibre pilot / locked Phase-1 / generic` |
| 13 | K1: Level A description (v2.4 best_params, SQLite) | ~0 | `Locked v2.4 best_params (live SQLite snapshot)` | `Locked best parameters run on a classical NumPy reference` |
| 14 | K2: cluster job tracker sub | ~0 | `cluster job tracker` | `simulator agreement check` |
| 15 | L: Phase 4 footer status (qiskit-ibm-runtime, Aer chain SLURM dispatch references) | ~0 | `Auth probe PASS (qiskit-ibm-runtime, channel ibm_quantum_platform, plan open) · Aer chains at v2.4 best_params re-dis...` | `IBM Quantum auth probe PASS, three backends reachable` |
| 16 | M: footer-cite (cluster paths, qad_master_*, v2.1/Fri 2026-06-20) | ~0 | `qad_master_followup_relevance_2026_06_07 / qad_master_stage_b / v2.1 / Fri 2026-06-20` | `fibre pilot configuration / generic` |
| 17 | N: REAL_DATA comment (cluster path /faststorage/.../qad_canon/data/external/*) | ~0 | `/faststorage/project/DeiC-KU-L64/qad_canon/data/external/*` | `published source CSVs` |
| 18 | O: MASTER configs comment (cluster path qad_master_stage_b) | ~0 | `qad_master_stage_b/*.json on 2026-05-24` | `locked per-dataset hyperparameters` |
| 19 | P: MASTER bestParams block (strip BOHB axes / cluster URL / live trial counts) for fibre_otdr_event | ~0 | `cluster URL + v2.4 BOHB live + 31 internal axis names` | `demo dashboard / Fibre model (locked) / 8 publishable axes` |
| 20 | P: MASTER bestParams block (strip BOHB axes / cluster URL / live trial counts) for fibre_intrusion | ~0 | `cluster URL + v2.4 BOHB live + 31 internal axis names` | `demo dashboard / Fibre model (locked) / 8 publishable axes` |
| 21 | P: MASTER bestParams block (strip BOHB axes / cluster URL / live trial counts) for fibre_health | ~0 | `cluster URL + v2.4 BOHB live + 31 internal axis names` | `demo dashboard / Fibre model (locked) / 8 publishable axes` |
| 22 | P: MASTER bestParams block (strip BOHB axes / cluster URL / live trial counts) for fibre_das_event | ~0 | `cluster URL + v2.4 BOHB live + 31 internal axis names` | `demo dashboard / Fibre model (locked) / 8 publishable axes` |
| 23 | P: MASTER bestParams block (strip BOHB axes / cluster URL / live trial counts) for fibre_das_audible | ~0 | `cluster URL + v2.4 BOHB live + 31 internal axis names` | `demo dashboard / Fibre model (locked) / 8 publishable axes` |
| 24 | Q: Phase 1 SVG label sub (ZZ/PQK/KTA kernel modes) | ~0 | `ZZ / PQK / KTA` | `quantum kernel scoring` |
| 25 | R: QPU_VAL_STATUS (SLURM 45927221/45927222, Aer chain re-dispatched, Phase-2 autoencoder fix) | ~0 | `SLURM 45927221 / SLURM 45927222 / Aer chain re-dispatched / post Phase-2 autoencoder fix` | `simulator agreement check` |
| 26 | S: QPU_VAL_STATUS comment (script path scripts/run_pipeline_at_optima_ibm_open_plan.sh) | ~0 | `scripts/run_pipeline_at_optima_ibm_open_plan.sh / backend_agreement_<dataset>.md` | `backend-agreement report (generic)` |
| 27 | T: KTA kernel internal label in finance describe | ~0 | `Phase 1 (KTA kernel)` | `Phase 1 (quantum kernel)` |
| 28 | U: kernel_mode in describeFibre | ~0 | `MASTER[key].bestParams.kernel_mode.toUpperCase() kernel` | `quantum kernel` |
| 29 | V: PQK kernel in describeFibre + "Kaggle-real-baseline" reference | ~0 | `Phase 1 (PQK kernel): trace shape outside Kaggle-real-baseline envelope` | `Phase 1 (quantum kernel): trace shape outside the normal baseline envelope` |
| 30 | W1: FIBRE_SEV "Tomasov DAS event" comment | ~0 | `Tomasov DAS event` | `DAS event detection classes` |
| 31 | W2: FIBRE_SEV "Dejdar DAS audible" comment | ~0 | `Dejdar DAS audible` | `DAS acoustic anomaly classes` |
| 32 | W3: FIBRE_SEV "Kaggle OTDR" comment | ~0 | `Kaggle OTDR` | `OTDR fibre health classes` |
| 33 | W4: FIBRE_SEV "BJTU phi-OTDR" comment | ~0 | `BJTU phi-OTDR fibre-intrusion` | `Phi-OTDR fibre intrusion classes` |
| 34 | X: BJTU-style comment | ~0 | `BJTU-style` | `numeric-prefix` |
| 35 | Y: PaySim 0.13% comment | ~0 | `e.g. PaySim 0.13%` | `(generic, removed)` |
| 36 | Z: BOHB w1,w2,w3 comment | ~0 | `REAL BOHB w1, w2, w3` | `locked ensemble weights w1, w2, w3` |
| 37 | AA: TDC NET requirement 2026-06-16 comment | ~0 | `TDC NET requirement 2026-06-16` | `(removed)` |
| 38 | BB: Master-config code comment (BOHB v2.4 tag + 22-axis enumeration) | ~0 | `BOHB v2.4 tag, BOHB_v2.4_2026-06-29 tag, internal axis names list` | `high-level configuration choices` |
| 39 | CC: MASTER_DISPLAY_KEYS (22 BOHB internal axes: kernel_mode, n_reuploads, phi_scale, entanglement, reference_set, warm_start, pc_selection_strategy, pc_relevance_method, kta_*, p_layers, mixer, phase3_init_mode, n_pool, n_restarts, selected_bonus) | ~0 | `22-axis BOHB enumeration with internal names` | `8 publishable axes with generic display names` |
| 40 | DD: KTA_ONLY / PQK_ONLY gating + cluster best_params comment | ~0 | `KTA_ONLY / PQK_ONLY axis-set Sets, kernel_mode gating, cluster best_params comment` | `simple value lookup` |
| 41 | EE: master tune meta (n_complete trials in tune_wall_h hours) | ~0 | `n_complete trials completed in tune_wall_h hours` | `(empty)` |
| 42 | FF: drift seed comment (33-axis layout) | ~0 | `33-axis layout` | `(removed)` |
| 43 | FF2: micro-BOHB perturb comment | ~0 | `rolling micro-BOHB estimate` | `rolling re-tune estimate` |
| 44 | GG: pipeline-arch line (kernel_mode, n_reuploads, phi_scale, entanglement, p_layers) | ~0 | `Master arch: KERNEL · n qubits · n_reuploads=N · φ=X · ENT · p_layers=P` | `Architecture: hybrid quantum-classical · n qubits` |
| 45 | HH: kpi-pr-sub Master locked n_complete | ~0 | `Master locked · n=N_COMPLETE` | `production model locked` |
| 46 | II: inspection provenance (pool.meta.source / pool.meta.file leak) | ~0 | `pool.meta.source + pool.meta.file (e.g. OTDR_data_part1)` | `published source dataset (generic)` |
| 47 | JJ: gov-cal calibration version (v2.0.3) | ~0 | `v2.0.3 — 2d ago` | `isotonic — 2d ago` |
| 48 | KK: Level F sign-off (TDC NET deck verbatim) | ~0 | `Goes into the TDC NET deck verbatim` | `(removed)` |
| 49 | LL: describeFinance function (mobile_money_fraud, aml_transaction_graph, bitcoin_aml_extended, vehicle_insurance_fraud, credit_card_fraud branches) | ~0 | `full describeFinance code branch` | `(removed entirely)` |
| 50 | MM: describe() router (finance branch) | ~0 | `family === finance ? describeFinance : describeFibre` | `always describeFibre` |
| 51 | NN: _postProcess function (mobile_money_fraud, aml_transaction_graph, bitcoin_aml_extended, credit_card_fraud branches) | ~0 | `finance dataset derived-field consistency code` | `fibre-only stub` |

## Data-file changes (qad_real_samples.js)

- Stripped 5 non-fibre dataset entries entirely:
  - `mobile_money_fraud` (PaySim — finance)
  - `credit_card_fraud` (ULB credit card — finance)
  - `aml_transaction_graph` (AML — finance)
  - `bitcoin_aml_extended` (Elliptic — finance/crypto)
  - `vehicle_insurance_fraud` (vehicle insurance — finance)
- Kept only the 5 fibre datasets:
  - `fibre_otdr_event`
  - `fibre_intrusion`
  - `fibre_health`
  - `fibre_das_event`
  - `fibre_das_audible`
- Within each remaining dataset, the `meta.source` and `meta.file` fields were replaced with `"published source dataset"` to remove specific filenames (e.g. `OTDR_data_part1`, `Tomasov...`) that leak dataset attribution.

## Verified PR-AUC numbers (cross-checked against source HTML)

| Dataset | QAD PR-AUC (kept) | Isolation Forest CI | Source line in v2.4 |
|---------|------------------:|---------------------|----------------------|
| fibre_otdr_event | 0.9095 | 0.7561 – 0.8366 | ~497 |
| fibre_intrusion | 0.6088 | 0.5005 – 0.5659 | ~507 |
| fibre_health | 0.9385 | 0.7808 – 0.8627 | ~517 |
| fibre_das_event | 1.0000 | 0.8330 – 0.9000 | ~527 |
| fibre_das_audible | 0.8230 | 0.6826 – 0.7587 | ~537 |

All five PR-AUC headline numbers carried forward verbatim from the source v2.4 dashboard `metrics:{qad_ap:...}` blocks — no fabrication.

## Anti-rules followed

- No `timbmadsen-eng/*` repos touched (Copenhagen-Quantum org only).
- No `git push --force` used.
- No synthetic data files added (CoQu IP stays internal).
- No fabricated numbers — every metric in the sanitized output appears verbatim in the source.
- No `__version__`, no BOHB version tags, no SLURM job IDs, no cluster paths, no Optuna/TPE/Hyperband mentions, no internal axis names, no academic citations.