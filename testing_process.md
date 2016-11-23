---
layout: page
title: Testing Process
desc: "How we test our software."
permalink: /testing/
---

*Because “works on my machine” isn’t going to cut it.*


Once a project is ready to begin we can start to build a test plan. A test plan uses the set of user stories that were outlined in the proposal given to the client in the [sales process](https://d4software.github.io/the-process/sales/). 


Depending on the nature of the project, we may be given web pages, or a working test version of the site or application, and this will help in the construction of the plan.


The first step to writing a test plan is to identify as many possible options or routes though the system as possible. **It is often helpful to list these options in a [truth table](https://en.wikipedia.org/wiki/Truth_table)**. 

**For example, A User may sign in;**

a) using Facebook,

b) Twitter, or 

c) using their email and password. 



**Users might be;**

a) ‘normal users’, 

b) ‘managers’ or 

c) ‘admins’. 



Once the truth table of options is built, we should create a list of scenarios that should be tested for each user story. It is never possible to test every possible permutation so some judgement is required.


**For example;**
We might reasonably assume that testing signin; 

a) as a ‘manager’ using Facebook,
b) as a normal user using Twitter and
c) as an admin using email and password, is a reasonable set of test scenarios. 


The final test plan can then be written. It should consist of one user story per sheet. Each story then has a list of several easy and straightforward steps, with each step being assigned a ‘test status’ of either: “Passed”, “Failed” or “Not Run” as testing commences. 

Those steps will cover the scenarios that were identified for testing. Havings lots of small steps, rather than a few broad tasks, ensures thorough testing and also a much better understanding of the software. 

Below is an example of a user story in the test plan:


![Test planning](https://d4software.github.io/the-process/img/testing-test-plan.png)



As each step has its own test status, it is therefore useful to have a Results sheet outlining the number of steps that have each passed, failed or have not been run (the test status will be “Not Run” only if that part of the software is not yet functional or the code for it has not been written).

You can then have a chart (a pie chart is nice) to illustrate clearly the fraction of steps set to each status and the progress through the project's testing phase.



![Test results chart](https://d4software.github.io/the-process/img/testing-test-results.png)



In addition to having a test plan, all of the user stories have tickets created for them in Jira.

These are both used in conjunction with one another with Jira taking the lead as it contains both tickets for the user stories, and it will be where any bugs or other tasks are recorded.

Once testing begins, any Jira tickets relating to user stories should be tested by following the steps on the relevant sheet in the test plan. If they cannot be passed, the original ‘user story’ Jira ticket remains ‘In Test’ and a new sub-task Jira ticket is created to track the bug.

**It is important to record the steps that lead to the bug.** This also goes for any other bugs that are found. **Without detailed steps to reproduce, it is difficult for the developer to fix the issue.**



![Testing with Jira](https://d4software.github.io/the-process/img/testing-jira.png)



As you reach the end of a sprint, it is worthwhile going back to the test plan and running through it again, end to end.

This gives you the chance to double check that everything is working as it should and to raise any bugs that may have been missed previously.

