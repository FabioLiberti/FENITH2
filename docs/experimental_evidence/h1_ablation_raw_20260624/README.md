# H1 Ablation — Raw Evidence Archive (SCAFFOLD Adam vs SGD)

**Archiviato il 24/06/2026** dalla VM `thesisvm` (NVIDIA A30 PST Alto Lazio) **prima della sua dismissione**, per preservare la provabilità raw del finding H1 usato nella tesi (Cap 7 §7.7.2, Cap 9, Cap 13, App A/B).

File: `h1_raw_archive_20260624.tar.gz` (4.6 MB, gzip verificato integro). Esclusi solo pesi modello e chart `.png` (non probatori per l'accuracy); inclusi tutti i JSON di metrica + script + codice optimizer.

## Dati canonici verificati (combaciano con tesi §7.7.2)

SCAFFOLD · MNIST · 10 client · 50 round · **full participation 1.0** · lr=0.005 · clipnorm=1.0 · seed {42,123,2026} · 18/05/2026.

| Seed | Adam `final_federated_accuracy` | SGD `final_federated_accuracy` |
|---|---|---|
| 42 | 0.097400 (9.74%) | 0.964900 (96.49%) |
| 123 | 0.113500 (11.35%) | 0.950800 (95.08%) |
| 2026 | 0.103200 (10.32%) | 0.934800 (93.48%) |

Adam mean **10.47%** · SGD mean **95.02%** · **Δ = 84.55 pp**. Pairing pulito *same-session*: `client_data_distribution.json` byte-identico per-seed (MD5: s42 `fbfe5c8f65`, s123 `bb41350616`, s2026 `f2a5a50a64`) → cambia solo l'optimizer.

## Portata (anti-over-claim)
Finding **SCAFFOLD-specifico** (gradient-correction control variate, Karimireddy 2020 Option II) e **LR-dipendente** (collasso solo per LR≥5e-3; con LR≤1e-3 converge, picco 95.21% a LR=5e-4). **NON** si estende a FedSpeed canonical (SGD 92.63/Adam 92.64) né FedDyn (SGD 98.99/Adam 99.20): vedi `FULL_MATRIX_state.json` e `SCAFFOLD_CRITICAL_state.json` nell'archivio.

## Contenuto archivio
- 6 dir esperimento (3 SGD `ABLATION_SGD_scaffold_mnist_s*` + 3 Adam `FULLPART_mnist_scaffold_s*`), ciascuna con `experiment_summary.json`, `all_rounds_metrics.json`, `client_data_distribution.json`, `client_participation.json`, `centralized_metrics.json`, `client_training_times.json`, `experiment_completed`.
- State JSON: `ABLATION_sgd_scaffold_state.json`, `MINI_full_participation_state.json.bak.3scaffoldAdam` (Adam), `ABLATION_fedspeed_canonical_H1_state.json`, `FULL_MATRIX_state.json`, `SCAFFOLD_CRITICAL_state.json`.
- Script: `FASE3_ablation_sgd_scaffold.py`, `FULL_MATRIX_8algos_ablation.py`, `SCAFFOLD_CRITICAL_ablation.py` (+`_PHASE2`), `FASE3_ablation_fedspeed.py`.
- Codice optimizer: `flopbg/models/model_definition.py` (env `FLOPBG_OPTIMIZER`, branch SGD) + backup `.bak.preSGDOpt`.

## Provenienza originale (VM dismessa)
Base: `/home/libe/flopbg/application/_Reports_/` e `/home/libe/FL-EHDS-FLICS2026/piano_sperimentale_tesi/{results,scripts}`.

## Come verificare
```
tar -xzOf h1_raw_archive_20260624.tar.gz \
  flopbg/application/_Reports_/ABLATION_SGD_scaffold_mnist_s42_20260518_172413/experiment_summary.json \
  | python3 -c "import json,sys;print(json.load(sys.stdin)['final_federated_accuracy'])"   # -> 0.9649
```

Evidenza testuale complementare (già nel repo tesi): `foundations/tesi_fl_2025/revision_notes/{fedspeed_analysis_19052026,full_matrix_22052026,scaffold_critical_24052026}/README.md`.
