# C4V-Py

## Installation

Use pip to install the package:
```
pip install c4v-py
```

## Development

The following tools are used in this project:
- [Poetry](https://python-poetry.org/) is used as package manager.
- [Nox](https://nox.thea.codes/) is used as automation tool, mainly for testing.
- [Black](https://black.readthedocs.io/) is the mandatory formatter tool.
- [PyEnv](https://github.com/pyenv/pyenv/wiki) is recommended as a tool to handle multiple python versions in your machine.

The library is intended to be compatible with python ~3.6.9, ~3.7.4 and ~3.8.2. But the primary version to support is ~3.8.2.

The general structure of the project is trying to follow the recommendations
in [Cookiecutter Data Science](https://drivendata.github.io/cookiecutter-data-science/).
The main difference lies in the source code itself which is not constraint to data science code.

## Pendings

- [ ] Change the authors field in pyproject.toml
- [ ] Change the repository field in pyproject.toml 
- [ ] Move the content below to a place near to the data in the data folder or use the reference folder.
Check [Cookiecutter Data Science](https://drivendata.github.io/cookiecutter-data-science/) for details.
- [ ] Understand what is in the following folders and decide what to do with them.
    - brat-v1.3_Crunchy_Frog
    - creating_models
    - data/data_to_annotate
    - data_analysis
- 

## brat-test

This repo contains the first iterations of Code For Venezuela's Named-Entity Recognition for public services outages in Venezuela. The goal of this project is to identify the following entities and attributes in tweets that utilize the public services-related tweets. E.g. #SinLuz, #SinAgua, #SinGas, #SinGasolina, etc...

### Data and Notebooks

- First iteration of annotations can be found at [./brat-v1.3_Crunchy_Frog/data/first-iter](https://github.com/dieko95/brat-test/tree/master/brat-v1.3_Crunchy_Frog/data/first-iter)
- Jupyter Notebooks with descriptive analytics about the annotations can be found at [./data_analysis](https://github.com/dieko95/brat-test/tree/master/data_analysis)

### Steps to annotate

#### Change to Brat's directory
`cd brat-test/brat-v1.3_Crunchy_Frog`

#### Run Brat's standalone server
`python2 standalone.py`

#### Login into brat
Once inside brat, click login on the right top corner of the browser.
- User: admin
- Pass: admin

#### Annotate
Click on Collections and select the file to annotate

### Entities and attributes

Entities as bullet points and attributes as sub-bullet points:

- water
  - with-service
  - without-service
- electricity
  - with-service
  - without-service
- gas
  - with-service
  - without-service
- gasoline
  - with-service
  - without-service
- social-report
- circumstantial-information
  - duration
  - location
  - time
  - reason
- twitter-account
  - politician
  - utility-company
  - news-company
  - other
