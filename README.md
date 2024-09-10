# Webscapper for Dashboard

## Developer Requirements

- Python 3.12 or greater
- Selinium
- Openpyxl

## Developer Setup

Python, Openpyxl and Selinium are  required for development. Python is used to
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
# Running the Script

You can run the script manually or schedule it to run automatically using the Windows Task Scheduler.

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

## Using Power Query to Summarize Data

1. **Summarize Data with Power Query**

   The Excel file uses Power Query to summarize weekly data for the dashboard.

2. **Update Queries**

   To update the queries, click on **Queries & Connections** in the Excel file:

   ![Queries & Connections](https://github.com/user-attachments/assets/0a8fb5b1-b314-4f61-93b4-60e89d1de69c)

3. **Add a Custom Query**

   You can add a custom query similar to the one shown below:

   ![Custom Query](https://github.com/user-attachments/assets/ae872101-8ea1-4994-a3fa-0f67c2bd12e0)

4. **Refresh Data**

   To run the query and refresh the data, click **Refresh All** under the **Data** tab in the Excel file. Ensure that the source is the appropriate location where your dashboard file is stored:

   ![Refresh Data](https://github.com/user-attachments/assets/11dffed8-a361-47b8-9caf-4d386f80d1f8)


## Sending Summarized Data by Email Using Power Automate

### Access Power Automate

- Go to [Power Automate](https://flow.microsoft.com/).

### Create a New Flow

1. Click on **Create** and choose **Automated flow**.
2. Provide a name for your flow and select a trigger. For example, you might use a schedule trigger to run the flow at specific times.

### Add Actions to the Flow

- **Get File Content**: Use the **Get file content** action to retrieve the Excel file from your storage location.
- **Send Email**: Use the **Send an email (V2)** action to send the summarized data. Configure the email with the recipient, subject, and body. Attach the Excel file if necessary.

### Test and Save the Flow

1. Test your flow to ensure that it works as expected.
2. Save and activate the flow to automate the process of sending the summarized data via email.


