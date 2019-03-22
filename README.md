# DDS6306_CaseStudy2_G1

MSDS 6306: Doing Data Science

Case Study 02

Due: One hour before Week 15 Live Session

Description: DDSAnalytics is an analytics company that specializes in talent management solutions for Fortune 1000 companies. Talent management is defined as the iterative process of developing and retaining employees. It may include workforce planning, employee training programs, identifying high-potential employees and reducing/preventing voluntary employee turnover (attrition). To gain a competitive edge over its competition, DDSAnalytics is planning to leverage data science for talent management. The executive leadership has identified predicting employee turnover as its first application of data science for talent management. Before the business green lights the project, they have tasked your data science team to conduct an analysis of existing employee data. 

Your team has been given a dataset (CaseStudy2-Data.xlsx) to conduct exploratory data analysis (EDA) to determine factors that lead to attrition.  You should identify (at least) the top three factors that contribute to turnover. There may or may not be a need to create derived attributes/variables. The business is also interested in learning about any job role specific trends that may exist in the data set (e.g., “Data Scientists have the highest job satisfaction”). You can also provide any other interesting trends and observations from your analysis. The analysis should be backed up by robust experimentation and (where applicable) appropriate visualization. Experiments, analysis, and visualization must be conducted in R. If needed, consult with the business owner to get clarifications on the dataset or business goals. 


Deliverables:  

This is a group project so it’s the responsibility of the group members to collaborate accordingly. Team work is important. 

The due date for submission is 1 hour before live session 15. During live session 15, the group will have up to 20 minutes to present their case study report. The goal is to communicate the findings of the project in a clear, concise and scientific manner. Tell me the story. 

Create a GitHub repository with an RMarkdown file containing an executive summary, introduction to the project, all supporting code and analysis, and the group presentation.
Submit a link to the GitHub repository via the space provided for the Case Study 02 page in 2DS. 

Your Presentation should be in this outline
<p>
	Title
<li>   	Authors all listed </li>
 	Presentation Outline
<dl>
<li>     Business Objectives </li>
<li>     Data Sourced </li>
<li>     Methodology </li>
<li>     Evaluation/Results </li>
<li>     Summary </li>
</dl>
<br> ¥	Business Objectives
<br> ¥	Data Source	
<br>     ¥	Where you got it 
<br>     ¥	Basic Statistics (EDA)
<br> ¥	Methodology	
<br>     ¥	Steps 
<br>     ¥	Workflow
<br> ¥	Evaluation/Results
<br>     ¥	Tell me the percentages and why
<br>     ¥	Show me graphs with explanations
<br>     ¥	The top three factors that contribute to turnover
<br>     ¥	Tell me about any job role specific trends that may exist in the data set
<br>     ¥	Provide any other interesting trends and observations from your analysis
<br>     ¥	Other things to consider?
<br> ¥	Summary 
<br>     ¥	Insights
<br>     ¥	Recommendations
<br>     ¥	Improvements
<br>     ¥	Questions
</p>
Have your presentation ready to present on during live session 15. 

NO CODE should be present in your presentation. (ie variable names is Mon_Age this should in your presentation as age). You code should be in your GitHub and RMarkdown File.  


Remember, no late assignments will be accepted, as this is the final.  It has been a pleasure teaching you this semester!  Congratulations on making it through your first semester in the Masters of Data Science program.  Good luck! 

Remember:
A GitHub repository and presentation
a.	Introduction to the project. The introduction should not reference a project, persay. No part of this should be informal.  It should be appealing-looking as well.
b.	The introduction needs to be written as if you are presenting the work to someone who has given you the data to analyze and wants to understand the result. Pretend it’s a presentation for a client. This may take some imagination of whom your client might be. If it sounds like a student presentation, that is not acceptable.
c.	R code for answers concerning the tasks below.  Make it in RMarkdown file format and always include echo=TRUE and include=TRUE for charts.  Keep the .md file so I can readily see everything on GitHub!  Your .md file should mirror the .RMD file.
d.	Give clear, explicit answers to the questions. Just the code to answer the questions is not enough, even if the code is correct and gives the correct answer. You must state the answer in a complete sentence outside the code chunk.
e.	Once you’re finished, be sure to frame a conclusion to the project. The presentation does not stop when you’re done with the questions.  Find a way to wrap it up: summarize your findings from this exercise. Again: the file must be readable in GitHub. In other words, don’t forget to keep the md file!!
f.	You should expand your repository with at least this RMarkdown file, the input file(s), and a README.md that describes the purpose of the project and codebook. The repo can be structured how you like, but it should make sense and be easily navigated.  If things are not clear from the root directory, you will lose points.
You’re working on this as a group. I expect that all will do equal work. All will need to push, add, commit, and pull the GitHub. If I do not see equal effort (and remember, GitHub tracks commits!), I reserve the right to penalize students. This is a collaborative project, so take it seriously and plan ahead with your teammate

Tasks
Tip: I recommend in the code block commenting which number the code answers.  It will help me find your answers more readily.  Something as simple as # 3B helps me.
1.	Formulate your Repo 
a	The client wants this to be reproducible and know exactly what you did.  There needs to be an informative Readme, complete with several sections, as referenced in Live Session.  Give contact information, session Info, and the objective of the repo at least.  
b	You have a large data set, and it needs its own Codebook, formatted in an approachable way.  Make sure you describe peculiarities of the data by variable and what needs transforming.  However, do not make it too long either.
c	Create a file structure that is accessible and transparent.  Document it in the root directory, ideally in the Readme.
2.	Clean your Raw Data 
a	Read the csv into R and take a look at the data set.  Output how many rows and columns the data.frame is.
b	The column names are either too much or not enough.  Change the column names so that they do not have spaces, underscores, slashes, and the like. All column names should be under 12 characters. Make sure you’re updating your codebook with information on the tidied data set as well.
c	Some columns are, due to Qualtrics, malfunctioning.  
d	Make sure your columns are the proper data types (i.e., numeric, character, etc.).  If they are incorrect, convert them. 
3.	Preliminary Analysis
a	Remove all observations where the participant is under age 18.  No further analysis of underage individuals is permitted by your client.  Remove any other age outliers as you see fit, but be sure to tell what you’re doing and why.
b	Please provide (in table format or similar), descriptive statistics on at least 7 variables (age, Income, etc.).  Create a simple histogram for two of them.  Comment on the shape of the distribution in your markdown.
c	Give the frequencies (in table format or similar) for Gender, Education, and Occupation.  They can be separate tables, if that’s your choice.
d	Give the counts (again, table) of management positions.
4.	Deeper Analysis and Visualization 
a	Note: You should make all of these appealing looking.  Remember to include things like a clean, informative title, axis labels that are in plain English, and readable axis values that do not overlap.
b	Create bar charts in ggplot or similar. The bars should be in descending order, Use any color palette of your choice other than the default.
c	Is there a relationship between Age and Income?  Create a scatterplot and make an assessment of whether there is a relationship.  Color each point based on the Gender of the participant.  You’re welcome to use lm() or similar functions to back up your claims.

d	What about Life Satisfaction?  Create another scatterplot.  Is there a discernible relationship there to what?   
