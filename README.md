# ArchExtract

Notebooks for named entity recognition (NER) and relation extraction (RE) with Flair, GLiNER, and GLiRE.

## Datasets

The notebooks use datasets to train and test models available at: [https://doi.org/10.6084/m9.figshare.28970633](https://doi.org/10.6084/m9.figshare.28970633).

The NER datasets are in **CoNLL-03 format**, with `token` and `label` columns, while the RE datasets are in **JSONL format**, with `text`, `ner`, and `relations` fields. Links are also provided directly in the notebooks.

## Notebooks

### `ner_finetune_flair.ipynb`

Fine-tuning Flair NER models using stacked embeddings on Portuguese general-domain dataset.

### `ner_flair.ipynb`

Running inference with Flair NER models on general-domain and domain-specific archival datasets.

### `ner_gliner.ipynb`

Running inference with GLiNER NER models on general-domain and domain-specific archival datasets.

### `re_glire.ipynb`

Running inference with GLiRE RE models on general-domain and domain-specific archival datasets.

## Requirements

* python 3.10+
* flair==0.15.1
* gliner==0.2.24
* glire==1.2.1
* pandas==2.3.3
* torch==2.3.1 # install the version matching your CUDA setup if using GPU
* tqdm
