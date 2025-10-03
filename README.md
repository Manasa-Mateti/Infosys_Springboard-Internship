# Infosys_Springboard-Internship

# Milestone1 — Text Summarization & Paraphrasing
This repository contains the Colab notebook and data for implementing and 
comparing pretrained models for summarization and paraphrasing.
## Structure
- `Milestone1.ipynb` — the main notebook (copy/paste the Colab cells).
- `data` — `input1.txt`, `input2.txt`, `ref1.txt`, `ref2.txt` (sample data 
provided).
- generated outputs and plots (saved after running notebook).
## How to run
1. Open `Milestone1.ipynb` in Google Colab.
11
2. Run the cells from top to bottom (select GPU runtime for speed).
3. Review `results.json` and `metrics.json` in `/content` and export them to 
your repo.
## Models used
- Summarization: `t5-base`, `facebook/bart-large-cnn`, `google/pegasus-xsum`.
- Paraphrasing: attempt to use `Vamsi/T5_Paraphrase_Paws`, `mrm8488/
pegasus_paraphrase`, `eugenesiow/bart-paraphrase` with fallbacks if 
unavailable.
## Evaluation
- ROUGE (1,2,L) for summaries.
- BERTScore (semantic similarity) for paraphrases.
## Observations 
- Summaries produced by Pegasus were often more concise; BART gave fluent 
sentences; T5 gave more literal outputs.
- Paraphrase models vary in creativity; compare semantic similarity and 
manual inspection.
