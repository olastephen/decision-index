# Submissions

| Model | Edition | Decision Index | Complete results | Engine / commit | Hardware | Declared limits |
|---|---|---:|---|---|---|---|
| PurpleMIST-Mini-1.0 ([`olaverse/PurpleMIST-Mini-1.0`](https://huggingface.co/olaverse/PurpleMIST-Mini-1.0) @ `8072361`) | 0.3 | 13.10 | [`runs/purplemist-mini-1.0`](https://huggingface.co/datasets/olaverse/decision-index-results/tree/6afbf05964ab969178eb14e27cc820e071c240f2/runs/purplemist-mini-1.0) | `http` engine against `serve.py --no-truncate --max-len 32768` from the model repo, fp32; kit `fbdc87c` | 1 x RTX PRO 6000 Blackwell Server Edition 96 GB | 32,768 tokens per pass; questions that do not fit beside the state are split across passes; nothing truncated, every request answered |
