# dvis4-examples

## Setup

Prepare a virtual environment
```
python -m venv venv
source venv/Scripts/activate
python -m pip install --upgrade pip
```

Either install all requirements ...
```
pip install -r requirements.txt
```

... or separately install Jupyter and some standard libraries ...
```
pip install jupyterlab pandas vega_datasets
```
... and install visualization libraries
```
pip install altair
pip install plotly==5.6.0
pip install ipywidgets
pip install matplotlib
pip install jupytab
```

Optional, if you use classical Jupyter Notebooks instead of Jupyter Lab:
```
pip install vega
jupyter nbextension install --sys-prefix --py vega
jupyter nbextension enable vega --py --sys-prefix
jupyter nbextension enable --py widgetsnbextension --sys-prefix
```

## Start Jupyter Labs

```
source venv/Scripts/activate
jupyter lab
```


## JupyTab server
cp. <https://towardsdatascience.com/interactive-simulation-with-tableau-and-jupytab-c26adb1be564>

setup a separate virtual env. for the server
```
python -m venv venv-server
source venv-server/Scripts/activate
python -m pip install --upgrade pip
pip install jupytab-server
```

create a kernel (in the jupyter virtual environment)
```
python -m ipykernel install --user --name jupytab-demo
```

start JupyTab server
```
jupytab --config=config.ini
```
