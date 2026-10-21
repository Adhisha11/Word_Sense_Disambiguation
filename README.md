### Natural Language Processing & Topic Modeling Report

This project implements two core Natural Language Processing (NLP) modules: **Word Sense Disambiguation (WSD)** and **Topic Modeling via Latent Dirichlet Allocation (LDA)**.

---

## Part 1: Word Sense Disambiguation (WSD)
We leveraged the WordNet corpus to build a structured sense inventory and performed disambiguation on target polysemous words using the classical **Lesk algorithm**.

### 1. Sense Inventory
A total of **75 senses** were discovered and cataloged for the target words `bank`, `bat`, and `light`. The structured database is saved as `sense_inventory.csv`.

### 2. Disambiguation Results
Using context overlap, the Lesk algorithm classified target words in sample contexts with their most semantically appropriate sense:
- **"I deposited money in the bank"** → `depository_financial_institution.n.01`
- **"The fisherman sat on the bank of the river"** → `bank.n.01` (sloping land beside a body of water)
- **"The bat flew out of the cave at night"** → `bat.n.01` (nocturnal mammal)

The full mapping report is saved as `wsd_results.csv`.

---

## Part 2: Latent Dirichlet Allocation (LDA) Topic Modeling
An LDA model ($k=3$) was built and trained to identify major themes across an unstructured document corpus covering multiple domains.

### 1. Discovered Topics & Keywords
- **Topic 1 (Technology & Computing):** `tech`, `new`, `cloud`, `billion`, `investing`, `quantum`, `processor`
- **Topic 2 (Space & Aerospace Science):** `launched`, `space`, `resolution`, `telescope`, `image`, `high`, `nasa`
- **Topic 3 (Finance & Economy):** `stock`, `long`, `report`, `bank`, `bond`, `term`, `financial`

### 2. Topic Distributions & Document Assignments
Our trained model assigned documents with high probability confidence bounds ($>92\\%$):
- **Docs 1, 2, 7:** Strongly mapped to **Topic 1 (Tech)**
- **Docs 3, 8, 9:** Strongly mapped to **Topic 2 (Space)**
- **Docs 5, 6:** Strongly mapped to **Topic 3 (Finance)**

### 3. Deliverables
- `topic_word_lists.csv` — Key terms associated with each topic.
- `topic_interpretation_report.csv` — Full document probability vector mappings.
- `README.md` — This comprehensive technical execution summary report.
