# Data Visualization

## Assignment 1: Participation (Ongoing)

### Requirements:

- During every class, follow along with sample code from the slides. All code that you should be running in Python is formatted as follows:
  
  > If code in a slide looks like this, you should be running it to generate results.

- When there are individual or group activities in submodules, make notes of answers and key points from discussions
- Following each lesson with code, submit a document (either .py or a Jupyter notebook) containing the functioning code from that day's lesson, along with any written notes or comments.
## Lesson 1 functioning code and comments 
# Notes 

To design good data visualizations, we need to consider three major principles: aesthetic, substantive and perceptual. From an aesthetic, visualization should be pleasing to look at while from a substantive point of view, visualization should accurately and truthfully present the data. from a perceptual perspective, the visualization should convey the intended message, and the audience should understand it. 

## Lesson 2 functioning code and comments 
# Codes
fig, ax = plt.subplots(figsize=(5, 3))
ax.hist(y)

ax.grid(axis = 'y')
ax.grid(axis = ‘y’
, color = "blue"
, linewidth = 2, linestyle = '-.')

# Note
A matplotlib is an open source package for data visualization in Python.

## Lesson 3 Functioning code and comments 

# Notes 
Reproducibility is the process of generating the same results, if the steps and techniques used in a dataset or a proportion of a dataset, are available for other researchers. Reprodicibility is ethical and it enhances the credibility of a research project. It is helpful to include our final code and the revisions we made, when we started coding and when we ended and what decisions we made when we coded. We we comment out our codes, we need to be descriptive and plain; use language that is understable to those in our fields.  There are four major principles for repprodicibility: findability, accessibility, interoperability and reusability. 
 
## Lesson 4 Functioning code and comments 
# code
fig, ax = plt.subplots(figsize=(5, 3))
ax.plot(x,y1)
ax.plot(x,y2)
fig.show()

font1 = {' family':'serif'
,
'color':'indigo'}
fig, ax = plt.subplots(figsize=(5, 3))
ax.scatter(x,y1, label = "Person 1")
ax.scatter(x,y2, label = "Person 2")
ax.legend(loc='lower right')
plt.xlabel('Shiny New X Axis!'
, fontsize = 18, fontdict = font1)

# Notes 
Data visualization has multiple purposes including persuading, comarping, evaluating and exploring. It should consider the audience. The audience can be any group of individuals, including children, adults, specialists including doctors, professors or engineers. Furthermore, data visualization can take place through various media including print, web and posters. 

## Lesson 5 Functioning code and comments 
# Notes
Effective data visualization for advocacy purposes need to use three modes of persuasion suggested by Aristotle. The first is rational appeal, based on which, providing the audience with facts will allow them to make the right conclusion about an issue. While rational appeal evokes the audience's moral values, enoptional appeal intends to make people feel empathy and commpassionate and build on these feelings to advocate for a particular issue. 


### Why am I doing this assignment?:

- This ongoing assignment ensures active participation in the course, and assesses the learning outcomes:
*	Create and customize data visualizations from start to finish in Python
*	Apply general design principles to create accessible and equitable data visualizations
* Use data visualization to tell a story

### Rubric:

| Component          | Scoring                 | Requirement                                              |
|--------------------|-------------------------|----------------------------------------------------------|
| Completion         | Complete/Incomplete for each class| - All required work from a given class is included in the file |
| Markdown file format | Complete/Incomplete for each class| - File is readable and contains functional code, when needed |

## Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Note:

* You should make a commit after each session with that lesson's code and notes. Your PR should have the same number of commits as there are sessions. It is important to make the commits to your branch in a timely manner right after each class.

### Submission Parameters:
* Submission Due Date: 23:59 -  2026-06-16
* The branch name for your repo should be: `assignment-1`
* What to submit for this assignment:
    * The `participation` folder/directory should be populated with the above mentioned .py/.ipynb files along with any written notes or comments (preferably in .md or .txt format).
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/visualization/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `assignment-1`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via our Slack. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
