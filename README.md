Swarm Intelligence Agents for OCR-based Receipt Processing

A research-focused project leveraging swarm intelligence algorithms and computer vision to process scanned receipts, perform OCR, and extract relevant data. Designed for reproducible AI/ML research and collaborative academic development.

 

Table of Contents

- Project Overview
- Features
- Getting Started
- Installation
- Usage
- Project Structure
- Data Sources
- Results & Evaluation
- Contributing
- License
- Acknowledgements

 

Project Overview

This project investigates the use of swarm intelligence-based agents for document analysis, focusing on scanned receipts. It features a complete end-to-end pipeline from preprocessing to OCR and information extraction, with experiments on CORD, SROIE, and synthetic receipt datasets.

 

Features

- Multi-agent swarm intelligence for task allocation
- Python-based modular pipeline with Jupyter notebooks
- Integrated OCR using Tesseract/PaddleOCR
- Dataset support: CORD, SROIE, and synthetic receipts
- Custom dataset preprocessing scripts (CSV, JSON)
- SQLite database integration
- Evaluation metrics for information extraction

 

Getting Started

# Prerequisites

- Python 3.8 or higher
- Recommended: Conda or virtual environments

# Installation

1. Clone the repository
   git clone https://github.com/your_username/swarm-ocr-receipt.git
   cd swarm-ocr-receipt

2. Create virtual environment (optional)
   python -m venv venv
   source venv/bin/activate

3. Install dependencies
   pip install -r requirements.txt
   or, for Conda:
   conda env create -f environment.yml
   conda activate swarm_ocr

 

Usage

- Run the main receipt processing pipeline:
  python src/main.py --config configs/base_config.yaml

- Notebooks for experiments and analysis:
  See notebooks/ for step-by-step walkthroughs and evaluations.

- Database management:
  SQLite scripts are in src/database/.

- Synthetic data generation:
  Run src/utils/generate_synthetic_receipts.py.

 

Project Structure

swarm-ocr-receipt/
│
├── src/
│   ├── agents/           # Swarm agent definitions
│   ├── ocr/              # OCR pipelines and wrappers
│   ├── database/         # SQLite integration
│   └── utils/            # Preprocessing, synthetic data
├── notebooks/            # Research/analysis notebooks
├── data/                 # Sample or link to datasets
├── configs/              # YAML/JSON configs for experiments
├── requirements.txt
├── environment.yml
├── LICENSE
├── README.md
├── CONTRIBUTING.md
├── CHANGELOG.md
├── .gitignore

 

Data Sources

- CORD: Receipt image dataset for information extraction research.
- SROIE: Task-specific OCR dataset.
- Synthetic generator: Pre-configured script for creating synthetic receipt images.
- Note: Due to size constraints, actual data may be accessed via download scripts or links in data/README.md.

 

Results & Evaluation

Key results are summarized in the evaluation section of notebooks/evaluation.ipynb, including:

- Entity extraction precision, recall, F1
- OCR accuracy benchmarks
- Dataset-wise comparison  
Feel free to run or extend evaluation code for your experiments.

 

Contributing

Contributions are very welcome! Please see CONTRIBUTING.md for guidelines and open issues.

 

License

Distributed under the MIT License. See LICENSE for details.

 

Acknowledgements

- CORD and SROIE dataset providers
- Open source OCR libraries (Tesseract, PaddleOCR)
- Swarm intelligence algorithms reference papers
- Academic supervisor and project contributors

 

For detailed documentation, see the docs/ folder or open issues for help or suggestions.

