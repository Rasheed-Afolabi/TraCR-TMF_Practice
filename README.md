# TraCR-TMF practice

Practice work reproducing the threat-modeling framework in Salek et al., *A Large Language
Model-Supported Threat Modeling Framework for Transportation Cyber-Physical Systems*
([arXiv:2506.00831](https://arxiv.org/abs/2506.00831)).

Their code and data: https://github.com/TraCR-National-UTC/TraCR-TMF

## What is here

| Notebook | What it does |
|---|---|
| `01_RAG_Library.ipynb` | Builds the searchable library of MITRE ATT&CK technique descriptions |
| `02_ICL.ipynb` | In-context learning — zero shot, one shot, few shot |
| `03_RAG.ipynb` | Retrieval-augmented generation over that library |
| `Fine_Tuning.ipynb` | Their fine-tuned ModernBERT, run on their published checkpoints |

## What I did

I worked through all three approaches on the authors' own data, following their released code,
to see what each one produces and where the numbers land.

- The fine-tuned model came out at micro-F1 **0.7222**, matching the number in their notebook.
- Retrieval-augmented generation came out at **0.225**, against their reported **0.25**.
- In-context learning I have only run on a small subset so far, so it is not comparable to
  their 0.48 yet.

Rasheed Afolabi · TRP 525
