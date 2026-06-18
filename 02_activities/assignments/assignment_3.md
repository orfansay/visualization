# Data Visualization

## Assignment 3: Final Project

### Requirements:
- We will finish this class by giving you the chance to use what you have learned in a practical context, by creating data visualizations from raw data. 
- Choose a dataset of interest from the [City of Toronto’s Open Data Portal](https://www.toronto.ca/city-government/data-research-maps/open-data/) or [Ontario’s Open Data Catalogue](https://data.ontario.ca/). 
- Using Python and one other data visualization software (Excel or free alternative, Tableau Public, any other tool you prefer), create two distinct visualizations from your dataset of choice.  
- For each visualization, describe and justify: 
    > What software did you use to create your data visualization?

    > Who is your intended audience? 
    
    > What information or message are you trying to convey with your visualization? 
    
    > What aspects of design did you consider when making your visualization? How did you apply them? With what elements of your plots? 
    
    > How did you ensure that your data visualizations are reproducible? If the tool you used to make your data visualization is not reproducible, how will this impact your data visualization? 
    
    > How did you ensure that your data visualization is accessible?  
    
    > Who are the individuals and communities who might be impacted by your visualization?  
    
    > How did you choose which features of your chosen dataset to include or exclude from your visualization? 
    
    > What ‘underwater labour’ contributed to your final data visualization product?


# Visualization 1
Source: https://data.ontario.ca/dataset/college-enrolment/resource/07fdeefd-fe44-4df8-bd7d-5419a79f90ec

# The link to Excel datasheet and visualization
https://utoronto-my.sharepoint.com/:x:/r/personal/sayeed_orfan_mail_utoronto_ca/Documents/college_enrolment_headcount_2024-25.xlsx?d=wcba762b44cc5459f8e5162e37297fdb2&csf=1&web=1&e=cDLNvW 

# Responses to questions for visualization 1

I used Microsoft Excel to create the data visualization, and my intended audience includes policymakers and government officials, college administrators and researchers interested in college activities. The key purpose of the visualization is to compare enrollment of domestic students with international students on Ontario colleges. The key message is that the number of international students in Ontario colleges has significantly increased compared to domestic students. I considered several aspects of design including contrasting colors that make it easy to distinguish between groups.  A line chart is used for student groups while bars are used to show the total. I used two axes; the left axis shows percentage while the right axis shows total number of students. I have used clear labels and legends as well. 
The data was analyzed and visualized in Excel in a structured table format (year, student type, and total). I used filtering and grouping to prepare data for visualization. Following these steps make the visualization reproducible. I have made the visualization accessible through various ways including using contrasting colors, clear legends and labels, and using readable font sizes. Various groups including domestic students, international students, colleges, government policymakers and local communities might be impacted by the visualization. Based on the purpose of my visualization, I have decided to include fiscal year, student type (domestic and international students), and total number of enrollments in Ontario Colleges while excluding college level data. Various underwater labor, including cleaning data, aggregating data across all colleges, grouping data, calculating proportion, choosing chart type, colors, layout, formatting and labeling have contributed to my final visualization. 

# Visualization 2
Source: Source: https://data.ontario.ca/dataset/college-enrolment/resource/07fdeefd-fe44-4df8-bd7d-5419a79f90ec

# The Link to Excel datasheet and visualization (I have include my chart generated in Python in Excel file named "Visualization 2)
https://utoronto-my.sharepoint.com/:x:/r/personal/sayeed_orfan_mail_utoronto_ca/Documents/college_enrolment_headcount_2024-25.xlsx?d=wcba762b44cc5459f8e5162e37297fdb2&csf=1&web=1&e=cDLNvW 

# Responses to questions for visualization 2

I used Python with the Seaborn and Matplotlib libraries. My intended audience includes college administrators, policymakers in Ontario's education sector, researchers interested in gender representation and advocates of equal gender representation in higher education. The visualization conveys changes in college enrollments in Ontario over time across different gender categories. I used various design principles, including different colors to distinguish each gender category, placing bars for each year side by side to make comparison between gender groups easy, clear and concise labels and titles and rotated the x-axis label to prevent overlap between years. I documented the data source and recorded the code used to produce the visualization. Anyone with access to the dataset and code can reproduce the same chart. I have made my visualization by applying multiple techniques, including clear and descriptive title, labels and legends, high contrasting colors and simple chart structure without overcrowding the visualization with too many words or visuals. The potential groups who might be affected by the visualization are college administrators, government agencies allocation funding for colleges, and advocates of gender inclusion and representation. The focus of my visualization is gender representation in Ontario college students across years; therefore, I included years, gender and enrollment counts. However, I excluded variables, such as country, language, and age. Underwater labor that contributed to final visualization included locating dataset, reviewing, cleaning and formatting, deciding which variable to include, selecting the appropriate chart type and customizing the cart. 

# codes for visualization 2 generated in Python 

import pandas as pd
df = pd.read_csv("/Users/sno/Downloads/gender11.csv", encoding="latin1")
df.head()

import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

fig, ax = plt.subplots(figsize=(12, 8))

sns.barplot(
    data=df,
    x="Fiscal Year",
    y="Headcount Full-Time Fall",
    hue="Gender Description",
    estimator=sum,
    errorbar=None)

plt.title("College Student Enrollment by Gender and Year (2012-2025)",fontsize=12)
plt.xlabel("Fiscal Year", fontsize=12)
plt.ylabel("Number of Students", fontsize=12)

plt.xticks(rotation=45)
plt.tight_layout()

- This assignment is intentionally open-ended - you are free to create static or dynamic data visualizations, maps, or whatever form of data visualization you think best communicates your information to your audience of choice! 
- Total word count should not exceed **(as a maximum) 1000 words** 
 
### Why am I doing this assignment?:  
- This ongoing assignment ensures active participation in the course, and assesses the learning outcomes: 
* Create and customize data visualizations from start to finish in Python
* Apply general design principles to create accessible and equitable data visualizations
* Use data visualization to tell a story  
- This would be a great project to include in your GitHub Portfolio – put in the effort to make it something worthy of showing prospective employers!

### Rubric:

| Component         | Scoring  | Requirement                                                                 |
|-------------------|----------|-----------------------------------------------------------------------------|
| Data Visualizations | Complete/Incomplete | - Data visualizations are distinct from each other<br>- Data visualizations are clearly identified<br>- Different sources/rationales (text with two images of data, if visualizations are labeled)<br>- High-quality visuals (high resolution and clear data)<br>- Data visualizations follow best practices of accessibility |
| Written Explanations | Complete/Incomplete | - All questions from assignment description are answered for each visualization<br>- Explanations are supported by course content or scholarly sources, where needed |
| Code              | Complete/Incomplete | - All code is included as an appendix with your final submissions<br>- Code is clearly commented and reproducible |

## Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `23:59 -  2026-06-16`
* The branch name for your repo should be: `assignment-3`
* What to submit for this assignment:
    * A folder/directory containing:
        * Two distinct data visualizations (for example, PNGs, PDFs, or screenshots)
        * Two Markdown files answering all questions for each visualization (including a link to your dataset in both files)
        * One Python file contains the complete code and visualization, and another file (with or without code) contains the visualization.
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/visualization/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `assignment-3`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via our Slack. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
