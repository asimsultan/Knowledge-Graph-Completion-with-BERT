
# Knowledge Graph Completion with BERT

Welcome to the Knowledge Graph Completion with BERT project! This project focuses on completing knowledge graphs using the BERT model.

## Introduction

Knowledge graph completion involves predicting missing links in a knowledge graph. In this project, we leverage BERT to perform link prediction using a dataset of knowledge graph triples.

## Dataset

For this project, we will use a custom dataset of knowledge graph triples. You can create your own dataset and place it in the `data/knowledge_graph_data.csv` file.

## Project Overview

### Prerequisites

- Python 3.6 or higher
- PyTorch
- Hugging Face Transformers
- NetworkX
- Pandas

### Installation

To set up the project, follow these steps:

```bash
# Clone this repository and navigate to the project directory:
git clone https://github.com/asimsultan/knowledge_graph_completion_bert.git
cd knowledge_graph_completion_bert

# Install the required packages:
pip install -r requirements.txt

# Ensure your data includes knowledge graph triples. Place these files in the data/ directory.
# The data should be in a CSV file with two columns: text and label.

# To fine-tune the BERT model for knowledge graph completion, run the following command:
python scripts/train.py --data_path data/knowledge_graph_data.csv

# To evaluate the performance of the fine-tuned model, run:
python scripts/evaluate.py --model_path models/ --data_path data/knowledge_graph_data.csv
