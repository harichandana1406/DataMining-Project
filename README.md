### What I posted (Checkpoint 1)

* `notebooks/Checkpoint1_EDA.ipynb` (dataset selection + EDA + initial insights)
* `requirements.txt` (or `environment.yml`) for reproducibility

---

## Initial README (copy/paste template)

### Project Title

**Directed Graph Mining on Reddit Hyperlink Networks (SNAP)**

### What this project is about

This project analyzes the **soc-RedditHyperlinks** dataset from SNAP, a **directed, signed, temporal** network where edges represent hyperlinks between subreddits extracted from posts (Jan 2014–Apr 2017). The goal is to apply course graph mining methods (centrality, SCC/WCC structure, community analysis) and explore a beyond-course technique such as **signed/temporal link prediction**.

### Dataset

* SNAP: soc-RedditHyperlinks (title/body files)
* Source: SNAP Datasets: Stanford Large Network Dataset Collection
  (include citation in notebook)

### Methods (planned)

* Course: degree distributions, SCC/WCC, reciprocity, PageRank/HITS, snapshot-based community structure
* Beyond-course: signed link prediction and/or temporal modeling (change-point detection, dynamic embeddings)

### Current status

* Checkpoint 1 completed: candidate dataset comparison, dataset selection, EDA (label distribution, temporal gaps, sparsity/edge weights, top sources/targets), and initial research questions.

### How to run

```bash
pip install -r requirements.txt
jupyter notebook notebooks/Checkpoint1_EDA.ipynb
```

### Repo structure (suggested)

```
.
├── notebooks/
│   └── Checkpoint1_EDA.ipynb
├── src/
│   ├── load_data.py
│   └── eda.py
├── data/               # ignored (raw files not committed)
├── requirements.txt
└── README.md
```

### Notes on ethics

This project reports aggregate statistics and avoids targeting individuals or small communities. The signed labels can be noisy and are interpreted cautiously.
