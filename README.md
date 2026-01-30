# NLP

Natural Language Processing tutorials and examples covering text preprocessing, representation, and transformer-based workflows. Implemented in Jupyter notebooks using spaCy, NLTK, scikit-learn, and Hugging Face.

## Prerequisites

- Python 3.8+
- pip

## Installation

```bash
git clone <repository-url>
cd NLP
python -m venv venv
# Windows
venv\Scripts\activate
# Linux / macOS
source venv/bin/activate
pip install -r requirements.txt
```

For spaCy language models (used in several notebooks):

```bash
python -m spacy download en_core_web_sm
python -m spacy download en_core_web_lg
```

For NLTK tokenizers (e.g. in `NLTk vs Spacy`):

```python
import nltk
nltk.download('punkt')
```

## Project Structure

```
NLP/
├── Text Preprocessing/
│   ├── 01 Tokenization in Spacy/
│   ├── 02 Language Processing Pipeline in Spacy/
│   ├── 03 Stemming & Lemmatization/
│   ├── 04 POS Tagging/
│   ├── 05 Stop Words/
│   ├── 06 NER/
│   └── 07 Regex/
├── Text Representation/
│   ├── 01_BagOfWords/
│   ├── 02_BagOfNgrams/
│   ├── 03_TF_IDF/
│   ├── 04_Spacy_WordEmbedding/
│   └── 05_Spacy_NewsClassification/
├── NLTk vs Spacy/
├── Practical NLP using Hugging Face/
│   ├── HF Tokenizers/
│   ├── HF Pipelines/
│   └── HF Model Fine Tuning/
├── requirements.txt
└── README.md
```

## Usage

Start Jupyter from the project root:

```bash
jupyter notebook
```

Open the desired notebook from the directory listing. Each folder contains one or more `.ipynb` notebooks and any required data files.

## Dependencies

Core dependencies are listed in `requirements.txt`:

- **Text preprocessing:** spaCy, NLTK
- **Representation and ML:** scikit-learn, pandas, numpy, matplotlib, seaborn
- **Transformers:** transformers, datasets, torch
