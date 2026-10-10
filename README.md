# Volatility Forecasting with Large Language Models

## Overview

This repository contains the research code, datasets (where redistribution is permitted), experiments, and evaluation results associated with my master's thesis, *Volatility Forecasting with Large Language Models*.

The project investigates whether information extracted from financial news using Large Language Models (LLMs) can contribute to financial volatility forecasting, and compares forecasting approaches with conventional econometric benchmarks.

## Research Objectives

The main objectives are to:

- Investigate the potential of LLM-based financial text analysis for volatility forecasting.
- Implement conventional forecasting benchmarks, including GARCH and EWMA.
- Extract relevant sentiment and risk-related features from financial news.
- Evaluate forecasting performance using quantitative metrics.
- Discuss the practical benefits, limitations, and reproducibility challenges of LLM-based forecasting.

## Methodology

The research combines financial time-series analysis with financial text analysis.

### Benchmark Models

- **GARCH:** Models conditional variance using past shocks and past conditional variance.
- **EWMA:** Estimates volatility using exponentially weighted historical observations.
- **LLM-based features:** Uses language-model analysis to extract information from financial news, where implemented in the experiments.

### Evaluation

Forecasting performance is assessed using quantitative evaluation metrics. The exact metrics, forecast horizons, data splits, and model specifications are documented in the relevant notebooks and results files.

## Repository Structure

```text
volatility-forecasting-with-llms/
├── data/
│   ├── raw/
│   ├── processed/
│   └── sample/
├── images/
├── notebooks/
├── results/
├── src/
├── thesis/
├── .gitignore
├── README.md
└── requirements.txt
```

The folders contain the datasets, analysis notebooks, Python code, figures, evaluation outputs, and thesis document, as applicable.

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/volatility-forecasting-with-llms.git
cd volatility-forecasting-with-llms
```

### 2. Set up a Python environment

```bash
python -m venv .venv
```

Activate it:

**macOS / Linux**
```bash
source .venv/bin/activate
```

**Windows**
```powershell
.venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 4. Run the experiments

Open the notebooks in the `notebooks/` directory using Jupyter Notebook, JupyterLab, or VS Code.

Run the notebooks in the order indicated by their filenames. Consult the notebook documentation for data requirements, parameters, and execution instructions.

## Data Sources and Reproducibility

Data sources, collection periods, preprocessing steps, and data limitations should be documented alongside the relevant datasets or notebooks.

Some financial datasets or news articles may be subject to third-party licensing restrictions. Where redistribution is not permitted, the repository should provide source references and instructions for obtaining the data rather than publishing the original files.

Results may depend on the data version, model configuration, random seed, software versions, and availability of external LLM services.

## Limitations

LLM-based financial text analysis has limitations, including potential interpretation errors, sensitivity to prompt design, data coverage constraints, computational costs, and reproducibility challenges.

The empirical findings should be interpreted within the scope of the datasets, forecasting horizons, and experimental design used in this research.

## Thesis

The final master's thesis is available in the `thesis/` directory, subject to applicable university and publication requirements.

## Author

**Tanjib Mahmud**

Master's programme: International Management, Marketing and Entrepreneurship  
Otto von Guericke University Magdeburg, Germany

## Disclaimer

This repository is intended for academic and research purposes. It does not constitute investment advice or a recommendation to buy or sell financial instruments.

## License

A license will be specified if and when the repository owner chooses to grant reuse permissions. Third-party datasets, news content, and other copyrighted materials remain subject to their respective terms.
