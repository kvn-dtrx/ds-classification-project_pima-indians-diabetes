# DS Classification Project: Pima Diabetes

## Synopsis

This repository presents an analysis of a data set concerning diabetes among the [Pima](https://en.wikipedia.org/wiki/Akimel_O%27odham) people based near Phoenix, Arizona. The data set is retrieved from the [*neue fische*](https://www.neuefische.de) database. It is very similar to <https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database> but contains contaminations deliberatively injected by the instructors for exercise purposes.

For more details about the assignment, please refer to [this file](./archive/assignment.ipynb).

In seeking to predict the prospective diabetes status of individuals, we evaluate our models using the true positive rate (i.e., recall with respect to the presence of diabetes).

As a baseline model, we choose a *logistic regression* with age and BMI (body mass index) as predictors, resulting in a true positive rate of approximately $0.70$.

As the main ML model, we employ a *decision tree* classifier, resulting in a true positive rate of approximately $0.76$.

## Repository Organisation

The organization of the repository follows common conventions and therefore requires little explanation. Our analysis notebooks (with technical details) are subordinated to [`notebooks/`](./notebooks/).

## Installation

### Requirements

- Python 3.11.3
- pyenv

### Setup

1. Navigate to a working directory of your choice, then clone the repository and enter it:

   ``` shell
   git clone https://github.com/kvn-dtrx/ds-classification-project_pima-diabetes.git &&
       cd ds-classification-project_pima-diabetes
   ```

2. Choose the right setup option based on your operating system:

   - `make unix`: macOS/Linux.
   - `make win`: Windows (PowerShell).

   If you prefer to run the commands manually yourself or want to inspect what a `make` target does first, use the `-n` flag for a dry run. This prints the commands without executing them:

   ``` shell
   make -n <target>
   ```

3. Activate the virtual environment:

   - On macOS/Linux, run:

     ```shell
     source .venv/bin/activate
     ```

   - On Windows (PowerShell), run:

     ``` powershell
     .\.venv\Scripts\Activate.ps1
     ```

## Colophon

**Author:** [kvn-dtrx](https://github.com/kvn-dtrx)

**Template:** This repository was derived from the [Neue Fische DS Diabetes Challenge Repository](https://github.com/neuefische/ds-diabetes-challenge).

**License:** [MIT License](license.txt)
