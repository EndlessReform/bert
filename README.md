# Custom BERT Project with WordPiece Tokenizer

This project is an educational effort to implement a custom [BERT](https://arxiv.org/abs/1810.04805) model and fine-tuning code for various tasks. The implementation is designed to load pre-trained BERT and RoBERTa weights, while also exploring transformer inference optimizations.

## Features

- BERT model implementation that supports loading pre-trained BERT and RoBERTa weights.
- Code for fine-tuning the BERT model on various tasks.
- Experimentation with transformer inference optimizations.

## Dependencies

- Python 3.x
- PyTorch
- HuggingFace Transformers (for loading pre-trained weights)
- Additional Python libraries listed in model/requirements.txt

## Getting Started

Install Python dependencies:

```sh
pip install -r model/requirements.txt
```

Run the fine-tuning code for the desired task, e.g.:

```sh
python model/bert/train.py --task_name TASK_NAME
```

## Project Structure

```
project_root/
│
├── model/                  # Machine learning model code (Python)
│   ├── bert/               # BERT model implementation
│   │   ├── __init__.py
│   │   ├── model.py        # BERT model architecture, training, and evaluation
│   │   └── utils.py        # Utility functions for the model
│   └── requirements.txt    # Python dependencies
│
├── data/                   # Data storage for training and evaluation
│   ├── train/
│   └── eval/
│
├── notebooks/              # Jupyter notebooks for experimentation and visualization
│
└── README.md               # Documentation for your project
```

## Fine-Tuning Tasks

The project supports fine-tuning the BERT model on various tasks. To run fine-tuning for a specific task, use the --task_name argument when calling the train.py script. For example:

```sh
python model/bert/train.py --task_name sentiment_analysis
```

## Transformer Inference Optimizations

This project also explores various transformer inference optimizations to improve the efficiency and performance of the BERT model. Details and results of these optimizations can be found in the notebooks/ folder.

## Acknowledgments

Google, obviously
The HuggingFace Transformers library for providing pre-trained BERT and RoBERTa weights

