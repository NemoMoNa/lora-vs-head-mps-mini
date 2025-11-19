# LoRA vs Head-Only (MPS/Colab) — Mini Project

A minimal, self-contained ablation comparing **LoRA** and **head-only** fine-tuning on Mac (MPS) and Colab.  
Data: small HF subset. Training: short steps. Eval: **chrF** (robust vs BLEU).  
Artifacts saved to `results/compare.tsv` and `results/notes.txt`.

## Quickstart
```bash
# (Optionally) create venv
python -m venv .venv && source .venv/bin/activate
pip install -U torch transformers datasets peft evaluate safetensors
jupyter lab  # or open the .ipynb in Colab
