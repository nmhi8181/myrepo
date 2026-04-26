# Hybrid TCN-LSTM Run Results

Execution date: April 26, 2026

This folder stores the exported results for the hybrid TCN-LSTM style experiment run from the local Research Objective 1 pipeline.

## Model used

- Architecture: `static_mlp + causal_tcn + uni_lstm + fusion`
- Config file used: `ro1_datastudent.json`
- Runs: `10`
- Device: `CPU`

## Key results

- Hybrid macro-F1 mean: `0.0461`
- Hybrid macro-F1 std: `0.0096`
- Static-only macro-F1 mean: `0.0368`
- Static-only macro-F1 std: `0.0086`
- Paired t-test p-value: `0.014336`
- Significant improvement over static-only: `True`
- Success target met (`>= 0.90`): `False`

## Dataset summary

- Rows before filter: `12411`
- Rows after filter: `12409`
- Classes before filter: `21`
- Classes after filter: `19`
- Excluded classes: `INDUSTRIAL CONTROL AND AUTOMATION ENGINEERING`, `TEXTILE ENGINEERING`

## Files

- `summary.md`: compact Markdown summary
- `summary.json`: structured machine-readable results
- `per_run_metrics.csv`: run-by-run hybrid and static-only metrics
- `config_used.json`: configuration used for this run

## Note

The exact `run_all_hybrid_models_2026-04-12/hybrid_tcn_lstm` training script was not present in the local workspace. This run used the available local hybrid experiment implementation whose temporal branch is a causal TCN followed by a uni-directional LSTM.