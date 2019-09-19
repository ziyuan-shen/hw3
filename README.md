# STA 523 :: Homework 3

wercker-badge-here

## Introduction

>America does a poor job tracking and accounting for its unsolved homicides. 
Every year, at least 5,000 killers get away with murder. The rate at which 
police clear homicides through arrest has declined over the years until, today, 
about a third go unsolved.
<br/><br/>
The Murder Accountability Project is a nonprofit group organized in 2015 and 
dedicated to educate Americans on the importance of accurately accounting for 
unsolved homicides within the United States.

<img src="map.png" width="600" height="200">

More details can be found at http://www.murderdata.org/p/about.html along with
a data dictionary at http://www.murderdata.org/p/data-docs.html.

## Tasks

#### Task 1

The following questions/tasks will require you to manipulate and summarise
the data. Be sure to consult the 
[data dictionary](http://www.murderdata.org/p/data-docs.html) so you understand
the variables and their set of possible values.

Each answer should include a one to two sentence write up. Your code output
should only contain the necessary rows and variables from the data frame to
answer the question or complete the task.

1. How many distinct counties in North Carolina had a recorded homicide in 2017?

2. Which year and month combinations had the three most homicides in 
	North Carolina from 2013 to 2017?

3. What were the top three states that had the most homicides by 
	"Murder and non-negligent manslaughter" that were solved and crossed racial 
	lines, i.e., where the offender and victim were of different race? Include the counts in your answer.

4. For the state of California, what is the relative frequency of unsolved
	homicides for each year in the data set?

5. Define a variable `age_gap` as the offender's age minus the victim's
	age. For each offender sex level (not Unknowns), what is the median age gap, 10th percentile age gap, and 90th percentile age gap? Your output should
	be in a single data frame.

6. Which five states had the largest change in the number of homicides by 
	"Murder and non-negligent manslaughter" in the
	10 years before and after the 1994 crime bill? Consider 1985 - 1994 and
	1995 - 2004.

#### Task 2

1. Based on your initial (further) analysis, form a narrative of what can be conveyed to
	a reader using the data and possibly supplementary data.

2. Create a visualization or set of visualizations that depict this narrative. 
They should tell an interesting story and / or provide insights into the underlying data. There is no single correct answer for these data and your visualization should depend on what your narrative is for the reader. Your visualization(s) should use `ggplot` or one of its extensions and may be supplemented by outside
data. 

3. Provide a write-up describing your design choices for your visualization(s). Explain why your visualization(s) is effective at elucidating
your narrative.


#### Task 3

Tidy up or decorate your Rmd file. Incorporate some of the features I used in
Lab 3. Feel free to expand beyond these features.

## Essential details

#### Deadline and submission

**The deadline to submit Homework 3 is 11:59pm on Thursday, September 26.** 
Only the code in the master branch will be graded.

#### git / GitHub

Each group will have a master branch and others with a GitHub name as a prefix.
One will be your GitHub name. You will only be able to push to your branch as the master branch is protected. To get your work into branch master (the only branch that will be graded), initiate a pull request on GitHub. This will then merge your work into the master branch upon approval by one of your teammates.

#### Help

- Post your questions in the #hw3 channel on Slack. Explain your error / problem
  in as much detail as possible or give a reproducible example that generates 
  the same error. Make use of the code snippet option available in Slack.

- Visit the instructor or TAs in office hours.

- The instructor and TAs will not answer any questions within the first 24
  hours of this homework being assigned, and they will not answer questions
  within 6 hours of the deadline.

#### Academic integrity

This is a group assignment. You should not communicate specifics about this
assignment with other groups. As a reminder, any code you use or find as 
inspiration must be cited. Include a references section in your Rmd file if
needed.

>Duke University is a community dedicated to scholarship, leadership, and 
service and to the principles of honesty, fairness, respect, and accountability.
Citizens of this community commit to reflect upon and uphold these principles 
in all academic and non-academic endeavors, and to protect and promote a culture
of integrity. Cheating on exams and quizzes, plagiarism on homework assignments 
and projects, lying about an illness or absence and other forms of academic 
dishonesty are a breach of trust with classmates and faculty, violate the [Duke 
Community Standard](https://gradschool.duke.edu/academics/academic-policies-and-forms/standards-conduct/duke-community-standard),
and will not be tolerated. Such incidences will result in a 
0 grade for all parties involved as well as being reported to the [University 
Judicial Board](https://gradschool.duke.edu/academics/academic-policies-and-forms/standards-conduct/judicial-code-and-procedures). 
Additionally, there may be penalties to your final class grade. 
Please review [Duke's Standards of Conduct](https://gradschool.duke.edu/academics/academic-policies-and-forms/standards-conduct).

#### Grading

**Topic**|**Points**
---------|----------:|
Task 1 |  12
Task 2 |  13
Task 3 |   2
Code style and format | 2
2 commits minimum / member | 1
**Total**|**30**

- *Documents that fail to knit will receive a 0*.
