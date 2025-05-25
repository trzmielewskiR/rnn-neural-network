# Named Entity Recognition — RNN on CONLL-2003

This project performs Named Entity Recognition (NER) using a recurrent neural network (RNN) trained on data in the IOB format (CONLL-2003 style).

## Task

Given a sentence, predict for each word its entity label:

- `B-XXX` — beginning of an entity (e.g. `B-LOC`)  
- `I-XXX` — inside an entity (e.g. `I-ORG`)  
- `O` — outside of any entity  

## Project Structure

- `train/` — training data (`train.tsv`)  
- `dev-0/` — validation input (`in.tsv`) and labels (`expected.tsv`)  
- `test-A/` — test input
- `rnn.ipynb` — main notebook for training and evaluating the model  
- `requirements.txt` — list of required Python packages  
- `.gitignore` — ignored files and folders (e.g. models, cache, virtualenvs)  
- `README.md` — project description and usage instructions  

## Getting Started

### 1. Set up the environment

It's recommended to use a virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

### 2. Run the model

Open and run `rnn.ipynb` to train and evaluate the model.