# Boston house prices dataset

The dataset can be found in `housing.csv`. It contains information about house values for census tracts in Boston, Massachusetts from 1978 (variable MEDV = median value of owner-occupied houses). The goal is to predict the house values from the other attributes, which are:
- RM: average number of rooms among houses in neighborhood
- LSTAT: percentage of Boston homeowners with greater net worth than homeowners in neighborhood
- PTRATIO: ratio of students to teachers in primary and secondary schools in neighborhood

The data has been cleansed already by Udacity (see notebook for details, 489/506 rows left, 3/14 attributes used). The original dataset is from [here](https://archive.ics.uci.edu/ml/datasets/Housing).

Check out `boston_housing.ipynb` for a solution to this task.

You can see the solution at the [GitHub page](https://dominicbreuker.github.io/boston_housing/)

## Getting started

### Virtual environment and packages

All requirements are freezed in `requirements.txt`. Set up a virtual environment with `pyvenv venv`. Then run `source venv/bin/activate` to switch to the environment. Then install packages with `pip install -r requirements.txt`. You can deactivate the environment with `deactivate`.

If you ever add new packages, keep `requirements.txt` updated. Run `pip3 install <package_name>` to install packges and `pip3 freeze > requirements.txt` to save requirements to the file.

### Running jupyter notebook

Run `jupyter notebook boston_housing.ipynb` to work on the dataset.


### Troubleshooting

I am using OSX with python 3.5.1 and pandas 0.18.1. On importing pandas, I get a "ValueError: unknown locale: UTF-8".

Run the following code before starting the notebook to solve the issue.
```bash
export LC_ALL=en_US.UTF-8
export LANG=en_US.UTF-8
```