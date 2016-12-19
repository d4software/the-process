---
layout: page
title: User Acceptance Testing (UAT) Process
desc: "Our UAT process helps the client to identify issues and bugs with the software we have produced and provides a way for them to feed back to us"
permalink: /uat/
---

All software development projects should include a period of time planned in for “User Acceptance Testing” (UAT). Projects may be broken down into phases or taken all at once, either way, at the end of the phase/project, a number of ‘user stories’ (defined during the Sales Process) will be delivered to the customer for UAT.

The minimum unit of delivery should always be the user story. We never deliver half a user story for UAT. If a software release includes some but not all the features of a user story, keep that user story in the ‘in progress’ status (see Project Management Process). 

We should also never deliver features that haven’t passed our internal Testing Process. Even if we’ve told the customer that a certain area is not yet ready for UAT, they will sometimes look at it anyway. When they do, they will find issues, which could undermine confidence in us and hurt the relationship.

The key goal of UAT is to identify issues, bugs or omissions that prevent the project from achieving the customer’s goals.

In order to accurately and efficiently keep track of these issues, and the decisions that are being made, it is very important that we apply some structure to our communications. The process for handling issues arising from UAT is as follows:

![uat process](https://d4software.github.io/the-process/img/uat_process.PNG)

**Capture**

If/when we are made aware of any issue relating to the software we are working on, we should first of all make sure that all of the relevant details are captured in the appropriate system. 

All discussions about the requirements for a system must be stored in a commonly accessible place that everyone involved can see and refer back to easily. The following formats are not appropriate:

* Email
* Phone calls
* Tweets
* Recorded voice memos
* Any form of instant messaging (e.g. SMS, iMessage, WhatsApp, Slack, HipChat etc.)

We typically use a Trello board for each project (see Project Management process) although in some cases we might use a spreadsheet, or the clients’ own systems. 

Following acceptance of our proposal document, the Trello board (or equivalent) should have been populated with a series of tasks that outline what we agreed we would do. Typically this will be the user stories that were documented during the Sales Process and which formed the basis of the project scope.

It should therefore be possible to identify which user story this new issue relates to, and reference it in the description of the issue.

**Catergorize**

Having captured the details of the issue, we should categorize it appropriately. It could be one of the following:

* Question
* Documentation task
* Bug
* Minor change (not strictly defined at the outset, but doable without additional time or money).
* Change Request (something that does not form part of the agreed set of user stories, and therefore chargeable).

It is important that we insist on categorizing this correctly so that, over time, an accurate picture emerges of what we’ve done.

A project portal populated with many bugs should make us question our processes. A project portal with many minor changes should provide the evidence for a frank discussion with the customer. If we do not categorize effectively, neither of those things are possible.

**Reproduce**

Wherever applicable, we should replicate the issues raised in our test environment first.

If we don’t do this, we can’t fix the issues, and even if we do make a change to try and fix the issue, we can’t prove that we’ve fixed it.

This stage also often highlights to us, areas where we need to clarify something with the customer.

**Clarify**

We need to agree with the customer, a form of words that clearly and completely describes what they want.

If the customer is raising a bug, we need a description of (a) the steps to reproduce, (b) the expected behaviour of the system, and (c) the actual behaviour.

We may need to obtain any of the following during this stage:

* The actual error message the customer is seeing
* A screenshot of their system
* A backup of their database
* A copy of the file they’re trying to edit/process/upload
* The error logs from their systems
* A login to their actual system
* The login details of a specific user account that is seeing the issue.

If the customer is stating a requirement, we need one or more sentences of text and/or wireframe drawings and/or diagrams that describes the expected behaviour in it’s entirety.

Some examples of inadequate “requirements” are:

* “**Change the {foo} screen like we agreed on the phone call**” - we cannot reference the phonecall.
* “**Make it like facebook, bug green**” - Too vague
* “**Issue 48567 from our internal system**” - We cannot all easily access their system. If one of us can, we should copy the information from their system into our system.
* “**Make it faster**” - Subjective
* “**Go through the system and just use your common sense, for example…**” - One person’s common sense is not the same as another person’s. We can action any specific example that they give us, but we cannot extrapolate from examples. We need to document the actual requirement.

At this stage it may become clear that this is a change to the original scope, or that it contradicts a previously documented design decision. If so, this is likely to be a chargeable Change Request.

**Assign**

Having captured, categorized, replicated and clarified each issue, we must set up tasks in our internal systems and assign them to someone to action (see the Project Management Process). 

Our internal system of choice is currently Jira. We should populate Jira with all the relevant information necessary in order to complete the task (minus any unnecessary discussion from the project portal) and add links to the project portal so we can cross reference. 

Bear in mind that we may use subcontractors who only have access to Jira and not the project portal.

At this stage, the task should also be assigned to the relevant sprint in Jira.


