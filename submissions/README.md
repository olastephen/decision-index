# Submissions

| Model | Edition | Decision Index | Complete results | Engine / commit | Hardware | Declared limits |
|---|---|---:|---|---|---|---|
| PurpleMIST-Mini-2.0 ([`olaverse/PurpleMIST-Mini-2.0`](https://huggingface.co/olaverse/PurpleMIST-Mini-2.0) @ `7e32e4c`) | 0.3 | 46.52 | [`runs/purplemist-mini-2.0`](https://huggingface.co/datasets/olaverse/decision-index-results/tree/6afbf05964ab969178eb14e27cc820e071c240f2/runs/purplemist-mini-2.0) | `http` engine against `serve.py --max-len 262144` from the model repo, bf16; kit `25c6ec7` (2d7791c reverted for the suite rebuild, #274) | 1 x RTX PRO 6000 Blackwell Server Edition 96 GB | 262,144 tokens per pass; questions that do not fit beside the state are split across passes; nothing truncated, every request answered |

| Board | Model | Hub repo | Results | Engine and options | Kit commit | Hardware | Resolution | Declared limits |
|---|---|---|---|---|---|---|---|---|
| **vision** | PurpleMIST-Mini-2.0 | [olaverse/PurpleMIST-Mini-2.0](https://huggingface.co/olaverse/PurpleMIST-Mini-2.0/tree/7e32e4cdfef21599b11636210b0e4929b521d46d) (public) | [runs/purplemist-mini-2.0-vision/](https://huggingface.co/datasets/olaverse/decision-index-results/tree/6afbf05964ab969178eb14e27cc820e071c240f2/runs/purplemist-mini-2.0-vision) | `decide`, `protocol=decisions`, against `serve.py --max-len 262144 --image-max-tokens 1600`; bf16 | 25c6ec7 | 1 x NVIDIA RTX PRO 6000 Blackwell Server Edition, bf16, one request at a time on the server | native up to 1.6 MP per image | none; 1 to 4 images per request, all answered |
