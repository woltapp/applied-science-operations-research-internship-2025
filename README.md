# Summer Intern Assignment 2025, Applied Science, Operations Research

**Assignment for candidates**

This is a mandatory assignment for everyone applying for the Applied science internship (Operations Research). Please return your answers along with your application.

> This assignment is exclusively for the Applied Science, Operations Research (OR) intern. If you want to apply to the non-OR position, please solve the corresponding [assignment](https://github.com/woltapp/applied-science-internship-2025).

# Table of Contents

1. [Overview](#overview)
2. [The Dataset](#the-dataset)
3. [Working with the Data](#working-with-the-data)
4. [Your Background and Wolt](#your-background-and-wolt)
5. [Submitting the Assignment](#submitting-the-assignment)

# Overview

Thank you for applying for Wolt's 2025 Applied Science Operations Research Internship! The idea is not to spend an extensive amount of time on this, but to show how you think and approach problems.

There are two parts in the application process:

- First, you get to work on an assignment: 
  - Load the OR dataset, explore it and present your findings to us.
  - Answer the [operations research questions](#operations-research-questions).
- Second, we will also take a look at your academic and extracurricular interests.

There are two things that we would like you to submit.

1. Prepare a concise presentation (up to 7 slides excl. title slide) about the task and the solution you came up with. The answer to the [operations research questions](#operations-research-questions) should be included in the presentation. Make sure to submit the **presentation in a pdf format**. The target audience for your presentation is a potential future peer Applied Scientist/Operations Researcher with relevant business knowledge. You should prepare the presentation according to the audience.
2. Present your analysis and work in a **reproducible way** and in an **open format**. Make sure you **include the code and your reasoning**, too. It pays to have a proper idea of Wolt's product and business, so it might be a good idea to take a look at [our blog](https://careers.wolt.com/en/blog/engineering) or some of the recent articles around the web.

Good communication of our work to others is a key component for success in this role. Hence, we will use the presentation to screen applications, and **to decide which assignments will be reviewed in detail**. So keep it concise and clearly explain to us what you've done in the assignment; spark our interest to look deeper. 

The presentation should contain some context for the relevant insights from the data, justification of selected metrics, as well as discussion around results and potential improvement. It should also include the answer to the Operations Research question.

Don't worry, we're not looking for a massive research poster! Just a clear presentation of what, why, and how you did things in the assignment. We'll grade the presentation based on the technical quality as well as communication skills.

There are many ways to successfully complete this assignment. Show us your skills. This is your chance to set yourself apart and shine!

# The Dataset
We prepared a task allocation dataset for you. The dataset consists of dummy and simulated data from a logistics system. The simulated data set includes events of deliveries, their timestamp, and other event details.
> Disclaimer: The simulated data does not represent Wolt operations nor how we assign tasks to the Courier Partners.

A delivery is a task group of exactly one pickup and one dropoff task. The pickup and dropoff of a given task group can only be completed by the same Courier Partner.
Typically, a delivery would have the following sequence:
- `DeliveryCreated`: An order was placed, with a given delivery time target (dropoff target).
- `DeliveryCommitted`: An order was committed by the Merchant (that is, the Merchant acknowledged the order and accepted to prepare it)
- `PickupStarted`: A Courier Partner started a pickup task. The Courier location at the starting time is stored in the event. 
- `PickupCompleted`: The Courier Partner completed the pickup of the order at the venue. We assume the Courier Partner completes the pickup as soon as the courier partner is at the venue AND the order is ready.
- `DropoffStarted`: A Courier Partner started the dropoff.
- `DeliveryCompleted`: The delivery was completed by the Courier Partner. That is, the dropoff was completed.
- `CourierArrived`: The event corresponds to the time at which a Courier Partner arrived at the target location of the pickup/dropoff task 
- `CourierWentOnline` and `CourierWentOffline` events correspond to the timestamp at which Courier Partner logs in/off in the Courier app.

# Working with the Data
## Exploration
Produce interesting statistics and charts about the dataset. Show the most important operations characteristics and explain what you see. 

Which metrics would you consider to measure the logistics performance? Are there tradeoffs between the metrics?
Based on the data, can you tell if any city is performing better than the others?

## Operations Research Questions
Please, answer the following questions in your pdf presentation (max 2-3 slides out of 7). We do not expect you to code any solutions, only the theoretical answers.

- What type of problem is this logistics system solving?
- Can you state one potential way of solving this problem? What are some pros/cons of that solution?

# Your Background and Wolt
After the practical work, let's discuss what you have learned and what your ambitions are. Write a bit about the problems you like to work with. Have you written your thesis or a larger piece of coursework about something that you would see beneficial for Wolt? If you already have work history, are there some things that you would like to try here? Based on your knowledge about us, are there some problems you would like to help us solve? Do you have some relevant, interesting minors or side projects? We are always interested in enthusiastic people with fresh ideas, and this could be the opportunity to put something you recently learned into use!

# Submitting the Assignment
Bundle everything into a Zip archive and upload it to Google Drive, Dropbox or similar and include the link in the application. Remember to check permissions! If we cannot access the file, we cannot review your solution. Please don't store your solution in a public GitHub repository or otherwise share it.

A good check before sending your task is to unzip the Zip archive into a new folder and check that building and running the project works, using the steps you define in readme.md. Forgotten dependencies and instructions can sometimes happen even to the best of us.
Application without assignment or with an attached file that we cannot open will be rejected.
