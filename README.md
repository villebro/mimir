# mimir
Yahtzee AI experiment

## Installation

It is recommended to use pipenv. To install the environment, do the following:

```bash
pipenv install ipykernel
pipenv shell
python -m ipykernel install --user --name=`basename $VIRTUAL_ENV`
```

If you don't already have Jupyter installed, do that by running

```bash
pip install jupyter
```

After that you can start jupyter:

```bash
jupyter notebook
```

## Developer's guide ##

The `requirements.txt` file is dynamically generated using `pip-tools`. To
bump all dependencies to the latest versions run

```bash
pip-compile -U --output-file requirements.txt requirements.in requirements-dev.in
```
