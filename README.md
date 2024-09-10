# Webscapper for Dashboard

## Developer Requirements

- Python 3.12 or greater
- Selinium
- Openpyxl

## Developer Setup

Python, Openpyxl Selinium are  required for development. Python is used to
run code and tests. Selinium is to scrape the web and Openpyxl is used to open and store data in the excel file.

### Conda

Create a Conda or Mamba environment using [environment.yml](/environment.yml).

`environment.yml` includes the following information:

- Environment name: `Webscrapping_env`
- Environment dependencies: Python , Selenium and Openpyxl

These tools are available in many distributions, including the following:

- [Miniconda](https://docs.anaconda.com/free/miniconda/index.html) provides a
  minimal installer for Conda

####Create and activate an Environment with Conda

```shell
conda env create --file=environment.yml
conda activate Webscrapping_env
```
# Run the code by schduling or running directly.


