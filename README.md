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
pip install jupyterlab pandas
```
... and install visualization libraries
```
pip install vega vega_datasets ipywidgets altair
```

If you use Jupyter Notebooks instead of Jupyter Lab, it might be necessary to activate some extensions:
```
jupyter nbextension install --sys-prefix --py vega
jupyter nbextension enable vega --py --sys-prefix
jupyter nbextension enable --py widgetsnbextension --sys-prefix
```

## Start Jupyter Labs

```
source venv/Scripts/activate
jupyter lab
```
