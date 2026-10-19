# Rule-based vs LLM parsers for flag football play entry (COMP 365 final project)

Question: can an LLM turn one plain-English sentence about a flag football play into a six-field stat record more accurately than a rule-based baseline?

## Files
- `final_eval_notebook_v2.ipynb` - full evaluation (dataset embedded). Run all in Google Colab (CPU is fine).
- `play_dataset_v1.csv` - 130 labeled sentences (20 dev, 80 test, 30 hard). `LABELING_GUIDE.md` - labeling conventions.
- `annotator2_ai_labels.csv` - second-pass labels for 20 random rows (made by Claude; 20/20 agreement; consistency check only).
- `results.json`, `results_table.csv`, `errors.csv`, `predictions.json`, `fig_main.png`, `fig_category.png` - outputs from the reported run (19 Oct 2026).

## Run it
1. Open the notebook in Colab, choose Run all.
2. Paste an Anthropic API key when asked (hidden input, never stored). The baseline needs no key.
3. Models: `claude-haiku-4-5-20251001`, `claude-sonnet-5-5`; default temperature; max_tokens 1024; two runs each.

## AI use and limits
The sentences, labels, and notebook code were produced with Claude (Anthropic). The same model family is also tested, so results are a feasibility check, not evidence of real-world accuracy. No human-subjects data were collected.
