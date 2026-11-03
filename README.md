# Jupyter-Pandas-Practice-Lab
## Jupyter Data Analysis Bootcamp

A 7-day, hands-on practice project for learning **Jupyter Notebook, Python, Pandas, data visualization and basic machine learning**, using realistic (synthetic) manufacturing and supply-chain datasets.

By the end you will be able to independently **create, run, explain, debug and document** a reproducible notebook workflow, from messy raw data to a clean dataset, charts, conclusions and exported files.

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![License](https://img.shields.io/badge/License-MIT-green)

---

## Who this is for

- Beginners and career changers preparing for data analyst or notebook-based technical assessments
- Anyone who wants practice cleaning messy data and explaining their work clearly
- Learners who prefer project-based practice over passive tutorials

## What you will practise

| Skill area | What you demonstrate |
| --- | --- |
| Jupyter Notebook | Cells, execution order, kernels, Restart and Run All, exporting |
| Python | Functions, loops, dictionaries, comprehensions, exceptions, file handling |
| Pandas | Loading, cleaning, transforming, grouping, merging, exporting |
| Visualization | Matplotlib and Seaborn charts with interpretation |
| Documentation | Markdown structure: objective, method, findings, conclusion |
| Debugging | Reading tracebacks, fixing common errors, explaining the cause |
| Reproducibility | Relative paths, fixed seeds, requirements file, ordered cells |
| Machine learning | Train/test split, classification, precision, recall, F1-score |

## The 7-day plan

| Day | Topic | Dataset(s) | Outcome |
| --- | --- | --- | --- |
| 1 | Jupyter fundamentals | `day1_sales.csv` | A clean, documented first notebook |
| 2 | Python fundamentals | `day2_machine_log.txt`, `day2_parts_inventory.csv` | Functions, loops, files, exception handling |
| 3 | Pandas cleaning and analysis | `day3_production_raw.csv`, `day3_lines_lookup.xlsx` | Messy data to a clean CSV plus defect analysis |
| 4 | Data visualization | `day4_monthly_kpi.csv` | Six or more charts, each explained |
| 5 | Debugging and file management | `day5_broken_notebook.ipynb`, `day5_orders.xlsx` | Seven deliberate bugs found and fixed |
| 6 | Machine learning basics | `day6_defect_prediction.csv` | A trained and evaluated classifier |
| 7 | Mock assessment | `day7_deliveries_raw.csv`, `day7_suppliers.xlsx` | A full end-to-end, 90-minute, screen-recorded task |

Each day's folder contains the data and a `TASKS.md` with numbered tasks, questions to answer in Markdown, a deliverable and a "done when" check.

## Repository structure

```text
jupyter-data-analysis-bootcamp/
├── README.md
├── requirements.txt
├── day1/   day1_sales.csv
├── day2/   day2_machine_log.txt, day2_parts_inventory.csv
├── day3/   day3_production_raw.csv, day3_lines_lookup.xlsx
├── day4/   day4_monthly_kpi.csv
├── day5/   day5_broken_notebook.ipynb, day5_orders.xlsx
├── day6/   day6_defect_prediction.csv
├── day7/   day7_deliveries_raw.csv, day7_suppliers.xlsx
└── solutions/   self-check numbers (open after finishing each day)
```

## Getting started

1. **Clone the repository**

   ```bash
   git clone https://github.com/<your-username>/jupyter-data-analysis-bootcamp.git
   cd jupyter-data-analysis-bootcamp
   ```

2. **Create a virtual environment (recommended)**

   ```bash
   python -m venv .venv
   source .venv/bin/activate        # macOS / Linux
   .venv\Scripts\activate           # Windows
   ```

3. **Install the requirements**

   ```bash
   pip install -r requirements.txt
   ```

4. **Start JupyterLab**

   ```bash
   jupyter lab
   ```

Prefer the cloud? Upload a day's folder to **Google Colab** and run it there.

## Requirements

`requirements.txt`:

```text
jupyterlab
pandas
numpy
matplotlib
seaborn
scikit-learn
openpyxl
```

## How to work through each day

1. Open the day's `TASKS.md` and read the goal and tasks.
2. Create **one notebook per day**, named like `day3_pandas_cleaning.ipynb`, in the same folder as the data.
3. Write Markdown **before** each code block (what and why) and **after** each result (what it shows).
4. Answer the day's questions in Markdown cells at the end of the notebook.
5. Finish with **Kernel > Restart Kernel and Run All Cells**. Fix anything that fails.
6. Compare your results with the self-check numbers in `solutions/` **only after** you finish.

### Golden rules

- Use **relative paths**, never `C:\Users\...` style absolute paths.
- Never submit code you cannot explain line by line.
- Every cleaning step needs a visible check showing before and after.
- Every chart needs a title, labels and one or two sentences of interpretation.

## About the data

All datasets are **synthetic** and generated with a fixed random seed. They contain no real people, companies or confidential information. Several files are intentionally messy (duplicates, inconsistent text, missing values, placeholder text, impossible sensor readings, mixed date formats, header rows in the wrong place) so you can practise real cleaning work.

## Day 7 final assessment

Treat Day 7 as the real thing:

- Set a **90-minute** timer.
- **Record your screen** and explain your decisions aloud.
- Use these notebook sections: Objective, Data loading, Data inspection, Data cleaning, Feature engineering, Analysis, Visualization, Conclusion and recommendations, How to reproduce.
- Export the notebook to HTML and save the output CSV files.

## Contributing

Suggestions are welcome: new datasets, extra exercises, typo fixes or improved explanations. Open an issue or submit a pull request.

## License

This project is released under the MIT License. You are free to use, share and adapt the materials. See `LICENSE` for details.
