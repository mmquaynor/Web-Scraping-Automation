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

### Create and activate an Environment with Conda

```shell
conda env create --file=environment.yml
conda activate Webscrapping_env
```
# Run the code by schduling or running directly.
You can run the file by downloding the activating the python environment and running the scrape.py file direcly.Alternatively you can use Windows Task schduler to automate running the file.
## Running Manually

1. Download and activate the Python environment.
2. Run the scrape.py file directly using:
```shell
python scrape.py
```
## Automating with Windows Task Scheduler 
1. Go to Start and search for Task Scheduler.

2. Under the Actions pane in the top right corner, click Create Task.

3. Specify a Name for the task and add the Triggers to set the task to run at a specific time.

4. Click the Actions tab and click New.

5. Set the Action to Start a program. Set the Program/Script to the path of your Python executable (python.exe). Add the path to scrape.py in the Add arguments field.

6.Click OK to save the task.

