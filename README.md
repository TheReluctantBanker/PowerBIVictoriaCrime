# PowerBI- Visualizing Crime Data from Victoria
Data Visualization on Victoria Crimes Data using Power BI

To view the visuals, please refer the PDF document which is the exported version of the .pbix created.

Background 
Crime is a topic that matters to us all. Most of us are fortunate enough to be safe all the same, however that does not mean we let down our guard. We worry about our safety as well as the safety of our loved ones and the larger community that we are a part of.
I thought of using the crime related data that Victoria Police publishes periodically for doing a data analysis and visualization project.

Objectives

[1] Gather relevant data relating to crime provided by Victoria Police

[2] Perform data cleaning / standardization as required for analysis.

[3] Perform data modelling to connect (relate) the different datasets.

[4] Create data visualizations that show composition, trends, metrics, and patterns relating to crime data.

[5] Use the visuals to gather some insights into crime related data for the available period.

Screenshots from Dashboard
![OVERVIEW](https://github.com/user-attachments/assets/5a80256e-3f8e-4f79-9b0c-6a0b1493d84e)

![INCIDENCE](https://github.com/user-attachments/assets/0080ec90-10c2-415b-8c87-816dac43027e)

![Text Analytics](https://github.com/user-attachments/assets/ca35ec55-5ae2-488e-930d-ebb58006cef6)

![Suburbs](https://github.com/user-attachments/assets/db3bae38-e130-4ee6-b40b-c22f77fd7ca9)

![Check Suburb](https://github.com/user-attachments/assets/6e41a74e-9cd3-4ada-a43d-4a3cbea7ad05)

![Financial Cost](https://github.com/user-attachments/assets/de13bdea-6b39-4f7c-869f-910def0d6034)









Data Sources
All the data used for this project was gathered from publicly available sources. Victoria Police has published crime related data both in https://www.data.vic.gov.au/ and https://www.police.vic.gov.au/crime-statistics. Data was gathered over the period 2016 till 2024. 


Understanding the data
Before proceeding to create data visualizations, it is necessary to understand the data on hand. It is useful to understand the datasets available, key data fields in each dataset and how the different datasets can be related. Since this was an open-ended project, where I worked independently with the data, I had to also think about the different ways I would perform data analysis. In a real-world setting, as a data visualization analyst, I would typically collaborate with business users to gather their requirements and key focus areas as a vital input.

Here is a summary of the different data sets and the information they contain.

![List of Files](https://github.com/user-attachments/assets/94e35a7f-df54-4f99-8a81-8c758e981658)

Data Preparation/Transformation tasks

For each data set imported into Power BI Desktop, some data cleaning/preparation tasks were required, they were performed using Power Query Editor, which provides a simple yet powerful interface for preparing and transforming data. The following were the typical data preparation tasks performed.

[1] Remove top rows which are redundant

[2] Use the row containing field names as the header row.

[3] Remove columns not required

[4] Filter rows not required

[5] For some files, the column containing the “actual” metrics was not clean. The numbers had unintentional spaces within them, which meant Power Query could not assign an appropriate data type for this situation. For example, “914 362” in row 1 in screen shot below instead of 914362 or the value against “Total Output Cost”). This was tackled in a multi-step process (convert the column to text, remove spaces and then convert to numeric data type).

[6] After data for different years was imported and cleansed, they were appended 

Data Modelling 

The data modelling task is required to be done to create an appropriate set of “fact tables” (which contain observations) and “dimension tables” which contain the reference or categorical information which are then used for creating filters in the visualizations. 

Such dimension tables were created separately in excel and then imported as a data source. Model relationships were also created between the dimension tables and the fact tables. Here is a screenshot of the “Model View” which shows how Power BI represents the relationships between the different datasets.

![Data Model](https://github.com/user-attachments/assets/ac60ea1d-656a-42d7-81d6-ad5ed0843e1d)


Creating data visualizations

Once the necessary data sets are available, I created several visuals based on the data analysis done. I approached this task by deciding the different areas I would focus on and grouped the visuals in the different “tabs” of the Power BI dashboard.

Visuals, Data Interpretation, and Insights 

![Insight Summary](https://github.com/user-attachments/assets/94ae5581-1452-4ac8-be0f-65d332097610)


Key Housekeeping tasks 

As a matter of practice, some standard tasks are done to finalize the dashboard.

[1] Hiding unnecessary tables from report view so that user doesn’t have to interact with them.

[2] Used tooltips with visuals to provide helpful information on the visual – see an example here

[3] Formatting of the visuals for consistency. See example here for a tool tip used

[4] Adding a “Clear All” filters button and use it as a bookmark for the “unfiltered” state of each tab. This way, the user can use the button to return the visuals to their original state.



