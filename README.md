# Top-Down SOZ Analyzer
A Python-based pipeline for identifying Seizure Onset Zones (SOZ) using signal complexity (LZC), spectral entropy, and cross-frequency coupling.

# Usage
This package provides an engine to analyze your own .edf neurophysiological data.

# Requirements
pip install -r requirements.txt

# Quick Start : Python
from src.pipeline import DynamicSOZPipeline

Initialize the engine
pipeline = DynamicSOZPipeline(z_score_threshold=3.0)

Run analysis on your local file
results = pipeline.run_scan("path/to/your/data.edf")
print(results.head())



# Data Preparation
The pipeline expects standard MNE-compatible .edf files. No clinical metadata is required to run the biomarker analysis.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DrShikharMishra/top-down-soz-analyzer/blob/main/topdownapproach.ipynb)
