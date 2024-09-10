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
## The steps for using the windows task Schduler are below:
1.  Go Start and search for Task Scheduler

![image](https://github.com/user-attachments/assets/2189ba29-8c6b-4e3a-a053-292dca336459)

2.  Under the Actions panein the top right corner , click Create Task

![image](https://github.com/user-attachments/assets/16e99ebe-4c1d-4cf0-b1e9-d15d5dbfc36f)

3.  Specify a Name for the task and add the triggers to run at a specific time
![image](https://github.com/user-attachments/assets/e8d1e4a3-5d51-4d10-9670-bf7088a1c841)

4.  Click the Actions tab and click New 
 ![image](https://github.com/user-attachments/assets/0df58a5e-9564-4dcc-a29d-355ee5414b97)
 
5.  Set the Action to Start a program.  The Program/Script needs to be set to the path of your python executable (python.exe).Add the path to the scrape.py as the Add arguments.
![image](https://github.com/user-attachments/assets/cd0e31d2-1105-494b-a6a5-a80abee998f7)

The script should be work after hitting ok to save the file.
