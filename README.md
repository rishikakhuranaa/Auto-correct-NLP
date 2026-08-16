# SpellCorrect — Statistical NLP Autocorrect

A lightweight **NLP spelling-correction system** based on **word frequency and edit distance**, implementing Peter Norvig's classic spelling-corrector approach.

## How It Works

```text
Misspelled Word
      ↓
Generate 1–2 Edit Candidates
      ↓
Keep Known Words
      ↓
Rank by Word Frequency
      ↓
Best Correction
```

The vocabulary is built from the **NLTK Brown corpus**, containing about **24,900 unique words**. Word frequencies are used as the prior for ranking candidate corrections.

## Notebooks

- `01_eda.ipynb` — Explores word frequencies, Zipf's law, and word-length distribution.
- `02_build_corrector.ipynb` — Builds the spelling corrector using deletion, insertion, replacement, and transposition edits.
- `03_evaluation.ipynb` — Evaluates the corrector on 43 common misspellings.

## Results

- **42/43** test cases were evaluable.
- Achieved **88.1% correction accuracy** on the evaluable test set.
- Works for both **individual words and sentences**.

## Tech Stack

**Python · NLTK Brown Corpus · Pandas · NumPy · Matplotlib**

## Key NLP Concepts

**Edit Distance · Word Frequency · Zipf's Law · Spelling Correction · Statistical NLP · Evaluation**
