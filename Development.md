# Installation
On Ubuntu you need
```bash
sudo apt-get install  jupyter-nbconvert python3-jupyter-console
```

## Setting up local venv

One time command to create directory `venv`
```bash
python3 -mvenv venv
source venv/bin/activate
pip install -r requirements.txt
```


## Convert the Notebook to plain python

```bash
jupyter nbconvert --to python prognoser/ssi_prognose_2020_03_22.ipynb
```

## Run the resulting python cli
```bash
python prognoser/ssi_prognose_2020_03_22.py
```
