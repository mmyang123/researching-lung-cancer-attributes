# Project 4 Requirements

## Overview
This project allows you to show off your skills in machine learning and the other technologies you've practiced during boot camp. 

## Grading
This project will be graded by your TAs and me, and grading will be both objective (i.e., how well did you satisfy the requirements) and subjective (i.e., how well you did you do compared to the other groups in the class). 

Since the project materials are due on the final day of class, much of the grading will be done during informal, in-person visits to your breakout room in the days leading up to the presentations. We will definitely look into your repos as well, but please don't expect our feedback to be quite as thorough as for previous projects, simply due to the lack of time. 

## Additional Time Outside of Class
You'll have ample time to work on this project in class, but please expect to spend additional time outside of class as well.

## Project Schedule
Please note that there will always be announcements at the beginning of every class.  

* Monday (11/21): Group formation and project kick-off
* Tuesday (11/22): **Project Proposals Due** at the end of class
* Thursday (11/24): **No class in observance of Thanksgiving Day**
* Friday (11/25): Study Hall from 3:00 PM - 6:00 PM Central Time (totally optional)
* Monday (11/28): Group time
* Tuesday (11/29): Group time
* Thursday (12/1): Group time
* Monday (12/5): Group time
* Tuesday (12/6): **Project Presentations and Final Celebration**

## Tips for Success
1. Read the requirements and consult them frequently throughout the project. 
1. Practice good attention to detail. 
1. Don't try to change the world.
1. Choose a high-quality dataset that's suitable for machine learning. 
1. Commit to your topic early, so you can maximize the remaining time. 

## Proposal Requirements
Please assume the proposal is the **_starting point for a discussion_** with me, and please anticipate a variety of questions about your topic, your dataset(s), and the way you plan to divide the work. My entire goal in this discussion is to ensure that you're set up for success and not attempting to do more than you can handle in the time provided. Proposals will be reviewed on a first-come, first-served basis, and you will not be allowed to move forward until your proposal is approved. Please DO NOT wait until the last minute to submit your proposal. 

1. You must submit your project proposal directly to me, via direct message on Slack (not email), no later than the end of the class period specified above.  
1. Your proposal must be written in one of the following:
    * A Google Doc (in which case you'll send me a link that has sharing enabled)
    * The `README.md` from your group's repo (in which case you'll send me a link)
    * DO NOT send me a Word document
1. Your proposal must be readable, grammatically correct, and well formatted. Otherwise, I'll send it back without reading it. 
1. Your proposal must include the following: 
    * Group number
    * List of all group members
    * Topic
    * An overview of what you plan to do
    * Links to the specific dataset(s) you plan to use. Note: it is NOT ok to say, "we'll find a dataset that contains ...." You must commit to your dataset(s) before I approve your proposal. 
    * The size of each data file
    * Work breakdown or list of major tasks
    * Which project track you intend to pursue: Research or Prediction. If you choose the Prediction Track, also indicate who will lead the hosting effort. This person will then create both the Heroku account and the shared repo. (The Heroku account doesn't have to happen right away. I will provide details later.)
    
## Technical Requirements
In the text that follows, a requirement is a statement that contains the word "must." The remainder of the text is there for clarity. 

Please read and understand these requirements, and consult them frequently throughout the project. **You will lose points for failing to satisfy a requirement.**

Note that these requirements supercede any requirements from slides or other materials. In the case of a conflict or contradiction, these requirements win.

1. Your project must have a website that displays or summarizes your work. It’s not required that the website directly interact with your machine learning model, but some students choose to implement one that does. 

1. Your website must fall into the **Research Track** or the **Prediction Track**.
    1. The **Research Track** is a website that summarizes and presents the results of your machine learning project. Think of this as a reserach paper on the web. 
    1. The **Prediction Track** is a website that summmarizes and presents the results of your machine learning project, AND allows the user to make a prediction. 
        1. Most websites on the **Prediction Track** will require Hosting to Heroku, which adds additional complexity to the project. An example might be a website that makes predictions from a classification model. 
        1. Websites that only use linear regression or multiple linear regression *can* (but don't have to) make a prediction from a website hosted on GitHub pages instead of Heroku. Rather than using the model itself, these projects will use a JavaScript function to crunch the coefficients and intercept generated by the model. 

1. Your project must use scikit-learn or another machine learning library (or both).

1. Your project must use at least two of the following: Pandas, Matplotlib, HTML/CSS/JS/Bootstrap, Plotly, Leaflet, D3, PostgreSQL, SQLite, MongoDB, Amazon AWS, Tableau. 

1. Your website must be hosted to GitHub Pages, Heroku, or another hosting service of your choice; i.e., you must ultimately be able to distribute the URL for your project to a future employer. Remember: GitHub Pages can only host static pages, which means it can’t host a Flask server or a database. Accordingly, GitHub pages cannot be used for projects on the Prediction Track (except as noted above). 

1. If you choose a hosting method other than GitHub pages or Heroku, we will be unable to provide technical support. 

1. Note that a database is NOT required, and using one may complicate your project (especially if you wish to pursue the Prediction Track). 

1. If you choose to use Tableau for visualization, you must embed those visualizations in your website rather than sending the user to Tableau Public. 

1. If you intend to pursue the Prediction Track, please see the section below on Hosting to Heroku. 


## Repo Requirements

1. Your project must be submitted in a single GitHub repo that contains all source files, data files (see exceptions below), and any other materials needed to recreate your work. 

1. If your data files (usually CSVs) are too large for GitHub’s 100MB limit, you must reduce the size using Pandas, not Excel. 

1. In the case where your project truly uses Big Data, I may grant an exception to pushing your data files to GitHub, in which case you should consider a database or an AWS S3 bucket instead. (See me to discuss.)

1. Your GitHub repository must have a professional looking `README.md` that contains an overview of your project and any instructions needed to recreate and run it. The audience for these instructions is someone who wishes to use the repo, *not* someone who wishes to write the code.

1. If your project contains a database, your instructions must specify how to populate the database. 

1. Your GitHub repo must be shared by all members of your project team. For credit, each team member will submit a link to this shared repo on BCS, and that link will be submitted before you present. 

1. Your repo must have a descriptive name that relates to your project topic. Do not call your repo `Project 4` or `Final Project.` (It's possible to rename a repo after you've created it, but you should always re-clone the repo when you do.)

1. Your project must use Git for version control. Do not try to circumvent this requirement by sharing Zip files.

## Hosting to Heroku
Hosting a website to anything other than GitHub pages goes beyond the scope of this boot camp. 

But, as a courtesy to the class, I'll provide instructions and a demonstration repo that show how to host a website and Flask application to a service called Heroku, which will allow you to make web-based predictions from your machine learning model. (Note: projects that use only linear regression or multiple linear regression can be hosted on GitHub Pages.)

Hosting to Heroku comes with the following complexities and limitations: 

1. Projects Hosted to Heroku are limited to scikit-learn models. Tensorflow and neural networks will not be supported. (Yes, it's possible to host a Tensorflow-based neural network; but that goes beyond the scope of this courtesy.)
1. Heroku will discontinue its free hosting tier on November 28th, and the next best option costs you $5.00 per month. You'll have to figure out a way for your group to pay for this.
1. I cannot provide you with information about the GitHub Developer Pack, which may facilitate some sort of discount. 
1. I cannot provide you with an `@umn.edu` email address, which may facilitate some sort of discount. (UMN doesn't offer these addresses to non-degree students.)
1. Beware: Heroku provides cryptic error messages and is difficult to debug. 
1. Hosting to Heroku is for advanced students only; those with some existing technology experience, who follow instructions well, and who are competent and comfortable with debugging their own code.
1. Hosting to Heroku will add additional work to your project; e.g., creating a Flask application. At times, this additional work can become significant; e.g., if you're stuck debugging a series of cryptic errors from Heroku. 
1. Hosting to Heroku cannot be attempted until your group has a fully functional project that runs on your local computer. 
1. Hosting to Heroku cannot be started any later than 9:00 PM on Thursday, 12/1. There simply won't be enough time. 

## Presentation Requirements
Presentations are Show & Tell, similar to the previous presentations in this course. 

1. Due to the large class and combined celebration, your presentation must last no longer than TBD minutes. 

1. All group members must take a turn and present something. 

1. All group members must have their cameras on while the group presents. (You're supposed to have your cameras on anyway, but you'll fail the project if you don't.)

1. Tip: Show off your website before you talk about the code. Otherwise, people tend to lose interest.

1. Tip: We don't need or want to see every line of code. Keep the focus on the website and show us only highlights of the code. 

1. Tip: Don't read your presentation. Unless you're an exceptional and dynamic reader, the audience will tune out. 

1. Tip: Skip the introduction. We all know who you are and which class this is, so dive right in and talk about your project. 

1. Tip: Use a timer and make sure you don't exceed the time you're allotted, especially if you're the first presenter in your group. 

1. Tip: Rehearse your presentation with your group to make sure the timing works. 

1. Tip: Instead of proceeding in a sequence and having each person speak only once, use a round-robin style that gives everyone several different opportunities to speak. That way, if the presentation runs long and the group runs out of time, nobody will be excluded from presenting. 

1. Tip: Do exactly what you did for Project 3. Those presentations were outstanding. 


