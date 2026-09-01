# Code Repository – Master's Thesis

This repository contains the code and supporting files used for the analyses presented in the master's thesis.

## Notebooks

The numbered Jupyter notebooks contain the complete code for the different stages of the research pipeline:

- **01_synthetic_query_generation.ipynb** – Generation of synthetic queries using an LLM.
- **02_query_length_analysis.ipynb** – Analysis and comparison of the lengths of original and synthetic queries.
- **03_lexical_overlap.ipynb** – Analysis of lexical overlap between queries and their corresponding target documents, as well as similarity between original and synthetic queries.
- **04_LLM_relevance_labelling.ipynb** – LLM-based relevance assessment of the generated synthetic queries.
- **05_RoBERT_model_testing.ipynb** – Retrieval evaluation of the RobBERT model.
- **06_mbert_evaluation.ipynb** – Retrieval evaluation of the mBERT model.
- **07_e5_models_evaluation.ipynb** – Retrieval evaluation of the E5 embedding models.
- **08_bge_m3_evaluation.ipynb** – Retrieval evaluation of the BGE-M3 model.
- **09_rank_stability.ipynb** – Analysis of model ranking stability between the original and synthetic query conditions using Spearman's rho, Kendall's tau, and Rank-Biased Overlap (RBO).

The model evaluation notebooks include the retrieval experiments and corresponding statistical significance tests.

## Supporting Data Files

For each of the three datasets (News, Tenders, and Abstracts), the repository contains several supporting files:

- **`*_full_augmented.csv`** – Contains the original queries, the generated synthetic queries, and their corresponding target documents.
- **`*_prompt.txt`** – Contains the prompt used to instruct the LLM during synthetic query generation.
- **`*_tasks.txt`** – Contains the task descriptions provided to the LLM for each respective text domain.

The three domains included in this study are:

- Dutch news articles
- Public tenders
- Scientific abstracts

## Repository Structure

The notebooks are numbered according to the general workflow of the research, starting with synthetic query generation and query analysis, followed by relevance validation, retrieval evaluation, and model rank stability analysis.
