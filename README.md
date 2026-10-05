# DL4STG - Programming Assignment 1

**Muhammad Adnan | Roll No. 25280067**

My implementation and experiments for both tasks of the Deep Learning for Space, Time and Graph assignment.

## Contents

- `Task1/PA-1_Task1.ipynb`: main Task 1 notebook, with experiments, outputs and responses.
- `Task1/harness/`: supplied experiment harness.
- `Task1/results/` and `Task1/checkpoints/`: saved results and model checkpoints.
- `Task1/data_exploration.ipynb`: supporting data exploration.
- `Task1/PA-1_Task1-x.ipynb`: alternative notebook version.
- `Task2/Task2_Autoformer.ipynb`: original Task 2 implementation.
- `Task2/Task2_Autoformer-fixed.ipynb`: revised Task 2 notebook for the additional run.
- `Task2/Data/`: training data, test indices and `optional_external_data.csv`.
- `Task2/outputs_task2_fixed/`: outputs from the revised notebook.
- `DL4STG-PA1.pdf`: assignment handout.
- `requirements.txt`: Python dependencies.

## Setup and Execution

Run these commands from the repository root:

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m jupyter lab
```

- Select the environment's Python kernel and run notebook cells in order.
- Keep the data and harness folders in the locations shown above.
- Use the full experiment preset for final results. A GPU is recommended for training.
- Rerunning cells may replace saved outputs and checkpoints.

## Task 2 Notes

- I use Autoformer's decomposition and delay mixing to forecast 168 target values.
- The optional external file provides covariates for both historical and future positions. These help the model use information beyond target history.
- The revised notebook adds training-only scaling, matched input comparisons, ensemble validation and clearer parameter/epoch accounting.
- The additional run is still in progress. I will upload it as optional supporting work; it may not count toward the assignment score. Its results are separate from the completed experiments in the report.

## AI Assistance

I used Codex for code review and help with LaTeX formatting for the report.
