# Python Intro — Prog1 exam helper

This folder contains a single self-contained Jupyter notebook that demonstrates basic Python concepts useful for a Programming 1 (Prog1) university exam.

Files
- `Test_Phase.ipynb` — the notebook with the demo and short examples. This is the only source file for the exercise; all code is inlined in the notebook.

What the notebook shows
- Variables and basic types (int, float, str, bool)
- Control flow (if / for loops)
- Data structures (list, dict, set, list comprehensions)
- Functions (examples and reusable helpers) and simple algorithms (factorial, primality test)
- Exception handling (raising and catching errors)
- Small interactive checks students can run in the notebook

Requirements
- Python 3.8 or later installed (for running locally or using Jupyter).
- Jupyter (optional) or VS Code with the Python extension to run notebook cells interactively.

How to run

1) Open and run interactively in VS Code

	- Open `Test_Phase.ipynb` in VS Code.
	- Use the Run Cell / Run All Cells buttons to execute the notebook.

2) Open in Jupyter Notebook / JupyterLab

	- From PowerShell, start Jupyter Lab or Notebook (if installed):

```powershell
python -m pip install --user jupyter
python -m jupyter lab
# or: python -m notebook
```

	- In the browser, open `Test_Phase.ipynb` and run the cells.

3) If `python` is not found in PowerShell

- Windows sometimes does not have `python` on PATH. Install Python from https://python.org and check "Add Python to PATH" during installation, or run using the full path to your python executable.
- Alternatively open the notebook in VS Code and use the Python interpreter picker (bottom-right) to select an installed Python interpreter.

Teaching suggestions / next steps
- Split the large demo cell into smaller concept-focused cells with short explanations and questions for students.
- Add short exercises (e.g., "implement and test reverse_list()") and expected outputs so students can practice.
- Convert the demo into a printable handout or slides.

If you want, I can split the notebook into separate cells with explanatory Markdown and small practice problems ready for your exam revision session. Tell me how many sections or which topics you want emphasized and I will update the notebook accordingly.
