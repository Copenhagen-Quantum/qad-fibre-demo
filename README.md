# Quantum Anomaly Detection — Fibre Demo

Live operator-dashboard demo for **Quantum Anomaly Detection (QAD)** applied to photonic fibre cable monitoring, by [Copenhagen Quantum](https://github.com/Copenhagen-Quantum).

Open the live demo: **[https://copenhagen-quantum.github.io/qad-fibre-demo/](https://copenhagen-quantum.github.io/qad-fibre-demo/)**

## What is this?

QAD is a hybrid quantum-classical pipeline for detecting rare events in high-volume sensor streams. This demo shows the operator-facing dashboard against five public fibre-monitoring datasets covering:

- **Fibre intrusion** (security — dig, knock, water, shake, walk events)
- **OTDR fibre events** (industry-standard reflectometry traces)
- **OTDR fibre health** (maintenance reflection events)
- **DAS event detection** (distributed acoustic sensing — vehicle, fence, construction)
- **DAS acoustic anomaly** (acoustic signal classification)

## Headline numbers (PR-AUC)

| Dataset                        | QAD PR-AUC | Isolation Forest |
|--------------------------------|-----------:|-----------------:|
| OTDR fibre events              | 0.91       | 0.80             |
| Phi-OTDR fibre intrusion       | 0.61       | 0.53             |
| OTDR fibre health              | 0.94       | 0.82             |
| DAS event detection            | 1.00       | 0.87             |
| DAS acoustic anomaly           | 0.82       | 0.72             |

## Methodology (high-level)

A three-phase hybrid quantum-classical pipeline:

1. **Phase 1 — Quantum Kernel Prescreen.** Quantum kernel scoring against a learned reference set.
2. **Phase 2 — Quantum Autoencoder.** Reconstruction-error scoring.
3. **Phase 3 — QAOA Selector.** Group-level selection using a quantum optimisation routine.

A fourth optional validation track compares the locked Phase-1 circuits against a real IBM Heron QPU, an ideal Aer simulator, and a noise-modelled Aer emulator.

Aligned with NIST / NIS2 / CER quantum-safe monitoring guidance.

## Contact

Tim Madsen — `timb.madsen@math.ku.dk`

## Note

This is a static snapshot dashboard for demonstration purposes. Streamed events are synthetic, drawn from distributions fitted on published source datasets.
