# Webscapper for Dashboard

## Developer Requirements

- Python 3.12 or greater
- Selinium

## Developer Setup

Python and Selinium are both required for development. Python is used to
run code and tests. Selinium is to scrape the web.

### Conda

Create a Conda or Mamba environment using [environment.yml](/environment.yml).

`environment.yml` includes the following information:

- Environment name: `gsdl`
- Environment dependencies: Python and Selenium

These tools are available in many distributions, including the following:

- [Miniconda](https://docs.anaconda.com/free/miniconda/index.html) provides a
  minimal installer for Conda

####Create and activate an Environment with Conda

```shell
conda env create --file=environment.yml
conda activate gsdl
```


