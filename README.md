# zomato-kpt-signal-improvement
Improving Kitchen Prep Time prediction using signal reliability framework
# Improving Kitchen Prep Time (KPT) Prediction

## Problem Statement

Kitchen Prep Time (KPT) prediction at Zomato relies heavily on merchant-marked Food Order Ready (FOR) signals. These signals are often biased due to rider-influenced marking and lack of visibility into real kitchen load.

This project proposes a Signal Reliability Framework to improve input signal quality without redesigning the core ML model.

---

## Key Contributions

- Rider-based inferred ready time
- Merchant Reliability Scoring
- Kitchen Load Proxy Features
- Hybrid KPT correction strategy
- ETA error comparison (Baseline vs Improved)

---

## Dataset

Synthetic dataset simulating:
- 50,000 food orders
- 500 restaurants
- 30% merchant bias behavior
- Peak hour rush simulation

Dataset Location:
data/raw/kpt_synthetic_dataset.csv

---

## Results

| Metric | Baseline | Improved |
|--------|----------|----------|
| Avg Rider Wait | 6.4 min | 4.3 min |
| P90 ETA Error | 12.1 min | 7.4 min |
| Delay Rate | 18% | 11% |

---

## Project Structure

- data/ → Dataset files
- notebooks/ → Analysis notebooks
- visuals/ → Charts
- docs/ → Submission document

---

## How to Run

1. Install dependencies:
   pip install -r requirements.txt

2. Run notebooks in order:
   01_dataset_generation.ipynb
   02_exploratory_analysis.ipynb

---

## Author

Shivani Aggarwal
