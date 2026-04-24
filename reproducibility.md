## Reproducibility Guide

This guide explains how to run the analysis notebooks and reproduce the figures in this repository.

No advanced Python experience is required, only a terminal and Python installed.

## Steps

### 1. Clone the repository

```bash
git clone https://github.com/arkeshdas/med-admissions-gap-year-analysis.git
cd med-admissions-gap-year-analysis
```


### 2. Create a virtual environment

#### Mac / Linux

```bash
python3 -m venv .venv
source .venv/bin/activate
```

#### Windows

```bash
python -m venv .venv
.venv\Scripts\activate
```


### 3. Install required packages

```bash
pip install -r requirements.txt
```


### 4. Launch Jupyter

```bash
jupyter notebook
```


### 5. Run the notebook

Open:

```text
notebooks/admissions_gap_year_analysis.ipynb (REPLACE with the file path of whichever notebook you are trying to run)
```

Then run:

* **Kernel → Restart & Run All**

This will regenerate all figures used in the project.


## Data availability

* Public datasets used in the analysis are included in the `data/` directory.
* Some extended analyses rely on AAMC data that cannot be redistributed. See `private_data_notes.md` for details.


## Notes

* The notebook performs all data processing and visualization.
* Figures are displayed inline and may also be saved to the `figures/` directory depending on configuration.


## Common issues

### Python not found

Try:

```bash
python3 --version
```


### Jupyter not launching

Try:

```bash
python -m notebook
```


### Environment issues

If something breaks:

```bash
pip install --upgrade pip
pip install -r requirements.txt
```


## Done

You should now be able to run the notebook and reproduce the analysis.

To exit the environment:

```bash
deactivate
```
