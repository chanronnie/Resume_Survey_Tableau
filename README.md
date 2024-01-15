![Most Common Mistakes](https://github.com/chanronnie/Tableau_Most_Common_CV_Mistakes/assets/121308347/07310181-f298-4943-8c1b-8325f2d4651b)
## About this project

#### Objective

The goal of this project is to create my own dataset by collecting data from an online survey that studied the most common resume mistakes, and to use this data to build an effective and engaging visualization. The key steps involved in this process include:

1. Data collection using web scraping techniques with Python in Jupyter Notebook
2. Data visualization creation using Tableau
3. Data visualization makeover.

#### Data Source

The data is collected from the CareerBuilder website using **Python** code. It consists of a survey conducted in 2018 by The Harris Poll on behalf of CareerBuilder regarding the most common mistakes found in the resumes.

## Tools Used
![Python](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)
 ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
 ![Tableau](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=Tableau&logoColor=white)

## File Contents
* [data_scraper.ipynb](data_scraper.ipynb): This notebook contains the Python code for data scraping.
* [data_survey.csv](data_survey.csv): This file contains the raw dataset.

## Approach

### The Data Extraction

The data survey are represented on the CareerBuilder website in both short paragraphs and bullet points forms. The data needed for our specific visualization are in list form, and there are only 7 records to extract. Using Python code and Python libraries (such as *BeautifulSoup* and *requests*), the data is easily extracted from the website.

:rocket: Please **[click here](data_scraper.ipynb)** for more details about the Python code.

### `data_survey.csv`

<details>
 <summary>View Table</summary>
 Here is the collected data.

mistakes | percent 
--- | ---
Typos or bad grammar	| 77
Unprofessional email address	| 35
Resume without quantifiable results	| 34
Resume with long paragraphs of text	| 25
Resume is generic, not customized to company	| 18
Resume is more than two pages	| 17
No cover letter with resume	| 10

</details>


![comparision](https://github.com/chanronnie/Tableau_Most_Common_CV_Mistakes/assets/121308347/4fd2a8f8-a0ca-436a-84a6-0e7ed5b0a29a)

### The Original Visualization

Resume mistakes are categorical data. A horizontal bar chart is an effective method to visualize this particular data. However, applying the default Tableau design to the bar chart may introduce unnecessary visual noise. The categorical labels have lengthy text spanning over two lines, making the chart less appealing to read. The presence of the gridlines and the axis labels makes the visualization appear clustered... Hence, the bar chart can be somehow more effective with fewer elements.

### The Makeover

I wanted to keep to one visualization that effectively communicates the survey's message. To achieve this result, here are the modifications I made:

- Removed the gridlines and axis labels from the chart to minimize visual noise.
- Labeled each bar with its corresponding value to make the visualization more informative. 
- Shortened categorical labels for extensive data by renaming variable aliases in Tableau.
- Transferred lengthy categorical text to the right side of the chart using a dummy variable created through a calculated field.
- Added a header and a description on top of the visualization to provide more context to the audience.

📍 To view my visualization on *Tableau*, please **[click here](https://public.tableau.com/views/MostCommonResumeMistakes/MostCommonMistakes?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)**
