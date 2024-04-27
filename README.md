## Data Science Job Data Dashboard

### Dashboard Link : https://app.powerbi.com/groups/me/reports/3f182181-f9bc-499a-bdee-e9a0d94a91ae/ReportSectioncbe73a82aa2851c7d773?experience=power-bi    

## Problem Statement

The main goal of this interactive dashboard is to highlights trends in different roles and titles. I'm focusing on things like experience, employee residence, and salary information to provide a clear picture of the job market landscape.  

The underlying reason for selecting this domain was that the job market is dynamic with changes happening in the industry with the evolving market. Job salaries are important for job seekers, employers, and policymakers who want to understand what's happening in the job market.   



### Steps followed 

- Step 1 : Loaded data into Power BI Desktop, dataset is a csv file downloaded from kaggle.com. This dataset downloaded from kaggle has been made by an aggregation of job data by scraping: https://ai-jobs.net/.  The kaggle dataset can be accessed with: https://www.kaggle.com/datasets/ruchi798/data-science-job-salaries  

   Then the dataset was opened with power query editor to check for duplicated values and data type detection issues. 

- Step 2 : Descriptive analysis using python

  The data set contains 11 variables.from these  11 variables,
  Numerical columns identified: work year, salary, salary in USD, Remote Ratio
  categorical columns identified: company location, job title, Experience level, salary currency, employee residence 

- Step 3 : Data preprocessing

    --Renamed the empty column of the index as “job id” 

    --Replacing values  in the Experience column 

        EN -Entry-level
        MI -Mid-level
        SE -Senior-level
        EX -Executive-level  

    --Replacing values in the employment type column 

        PT -Part-time 
        FT -Full-time
        CT- Contract
        FL –Freelance  

    --Replacing values in the Company size column 

        S- small
        M- medium
        L- Large 

 
- step 4: Power BI visuals (report view) 

The following plots were created to accurately reflect the findings from the data. The slicers on top with years allow filtering all data visuals by the year. The card visuals on top display the most critical numerical statistics.

Pie chart and donut chart visuals were used to show the total percentage distribution of company sizes and job distribution by emploment type. 

Line plot visual maps the overall trend of the number of jobs and  average salary variation by the year. Table visual shows the top countires with their count of jobs. The correlation heatmap depicts the relationship between the employement type and numerical columns average salary and remote ratio. 



 

# Snapshot of Dashboard (Power BI Service)

![Screenshot 2024-04-27 174253](https://github.com/subhanu-dev/Data-Science-Job-Data-Analysis-Dashboard/assets/120291970/ab062cb4-a111-46e4-a059-2c103b60f0fe)
 
 

# Insights

In conclusion, this dashboard analysis of the data science jobs brings several insights about the landscape of jobs in data science. The average annual salary of a data science professional exceeds 100,000$(112,000$) with a standard deviation of $70,957 .There is an overall positive growth in the trend of jobs count and salaries in data science and most of the hires are done by medium and large-scale companies.

Senior/lead/principal positions yield more salaries.When it comes to the number of jobs listed, more than 50% of the jobs are from the US, and over 96% of the jobs are full-time. Though most of these jobs are full-time, almost all these jobs allow hybrid or fully remote work with an overall remote ratio of 70.92% More experienced senior professionals who work in contract and full-time positions have a higher correlation with a higher salary. 
