# ITMO Scientific Python 2026

Coursework repository for the ITMO Scientific Python track. The notebooks cover API work, object-oriented Python, biological sequence parsing, and exploratory data analysis.

## Repository Contents

| Folder | Topic | Main files |
| --- | --- | --- |
| `HW2/` | Bioinformatics API requests and parsing for UniProt and Ensembl IDs | `HW2.ipynb`, `API_requests.ipynb`, `test_data.txt` |
| `HW3/` | OOP, iterators, class/static methods, and Open-Meteo API usage | `HW3.ipynb`, `car-snippet.py`, `weather-snippet.py` |
| `HW4/` | FASTA parsing with Biopython, database lookup, and `seqkit` statistics | `HW4.ipynb`, FASTA examples |
| `HW5/` | Exploratory data analysis for the Heart Failure Prediction dataset | `HW5.ipynb`, `heart.csv`, `titanic.csv` |

The root also contains `image_encoded0.txt` and `image_encoded1.txt`, which are encoded image-recovery exercise inputs.

## Quick Start

Create and activate a local Python environment:

```bash
python -m venv .venv
source .venv/bin/activate
```

Install the Python packages used across the notebooks:

```bash
pip install jupyter pandas requests openmeteo-requests biopython matplotlib seaborn ipython
```

Then launch Jupyter:

```bash
jupyter notebook
```

Open the notebook for the homework you want to inspect, for example `HW5/HW5.ipynb`.

## External Tools

`HW4/HW4.ipynb` calls `seqkit` through `subprocess` for FASTA statistics. Install `seqkit` separately and make sure it is available in `PATH` before running that part of the notebook.

## Notes

- Some notebooks call public APIs, so those cells require internet access.
- Data files are kept with the homework folders to make each notebook runnable from its own directory.
- The encoded image files can be restored by reversing the character shift and decoding the resulting textual representation back into a PNG.
