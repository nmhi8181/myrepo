# Research Objective 1 Summary

## Hybrid Model
- Architecture: `static_mlp + causal_tcn + uni_lstm + fusion`
- Macro F1 (mean +- std): `0.0461 +- 0.0096`
- Success target met (`>= 0.90`): `False`

## Ablation
- Static-only Macro F1 (mean +- std): `0.0368 +- 0.0086`

## Statistical Significance
- Paired t-test p-value: `0.014336`
- Significant improvement (`p < 0.05`): `True`
