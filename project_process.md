---
layout: page
title: Project Management Process
desc: "Our Project Management Process is designed to ensure that the objectives defined during the Sales Process are achieved."
permalink: /project-management/
---

This process has a number of components:

1. Tasks to complete during the project.
2. A system for maintaining a shared actions and issues log with the customer.
3. A set of internal tools for tracking issues and sharing information.



## Project Tasks

All projects should include the following activities.

**A Project Plan**

During the Sales Process a high level timescale may have been discussed. At the beginning of the project, a detailed project plan (based on the timeline that was discussed) should be produced and shared with the customer. 


The sooner this happens the better. If there are issues with meeting the customer’s expectations (e.g. Maybe a deadline was discussed in a sales meeting but the project was not approved for several weeks) it's better to find out sooner rather than later.


The project plan should detail what project deliverables (either documents, or ‘user stories’) will be delivered and when. On a project delivering more than a handful of ‘user stories’ the stories will typically be broken down into multiple ‘sprints’. Sprints should last between 1 and 4 weeks and should end with a release of the software to the customer.

**Kick Off Meeting**

At the beginning of the project, a meeting should be organised to discuss the following items:

* Present and agree the project plan.
* Agree a schedule for regular project meetings/calls.
* Agree key individuals and who should be involved in decision making.
* Agree the approach for logging tasks and issues. (Ideally trello, see below).

**Regular Meetings/Calls**

It is important to have regular scheduled contact with the customer. This is an opportunity to:

* Update the customer on our progress.
* Review the tasks/issues that we've flagged as being blocked or requiring more information, and get these issues unblocked.
* Agree changes to the project plan

**Design Documents**

Design documentation should be produced and sent to the customer for approval. Depending on the context, this may include:


* UX Wireframes
* Technical Specification
* UI design 


See the Business Analysis and User Experience design process for more information.

**Test Plan**

A test plan should be created. See the testing process for more information.



## Shared Action and Issue Log

It is important to have an action and issues log that both the customer and D4 can see. Our preferred tool for this is Trello. Each project should have a Trello board. Every issue/question/bug/feature etc will become a card on that Trello board. 


At the beginning of the project, a Trello card should be created for each of the user stories agreed as ‘in scope’ during the sales process.


Trello cards should also be created for each of the design documents that will be produced.


The customer will be invited to the Trello board and all relevant discussions about the requirements or specification of the system should be either conducted via Trello messages or the outcome of those discussions should be copied onto the Trello card. This is so that every agreement is recorded, making it much easier for us to refer back to something. 


For each card in Trello there should only be one topic. If a client has diverged from the original topic or has asked other questions or raised other bugs, a new card should be created for each individual topic.


If the customer is not happy with using Trello, a shared online spreadsheet is the next best option.

All actions or issues on the log should move through a series of statuses, these are:


* Blocked / Info Required
* Ready to Begin 
* In Progress
* In Review
* Done


In Trello these are represented by columns.

The meaning of these statuses, what should happen at each stage, and where the work item can go next, is defined below:

<table border="1">
  <tr>
    <td> Status </td>
    <td> Meaning </td>
    <td> Next Step </td>
  </tr>
  <tr>
    <td> Blocked / Info Required </td>
    <td> This is where new items should be created initially.
         <br><br> 
         Once created, each item should be labelled as one of the following:
         <br><br>
        <ul> 
          <li>Question </li>
          <li>Project Deliverable </li>
          <li>Minor Change </li>
          <li>Change Request </li>
          <li>Bug </li>
          <li>Info / Doucmentation </li>
        </ul>
        <br>
        The issue may need to be replicated and/or clarified which may involve messaging the client and/or uploading files to this Trello card.
    </td>
    <td> The issue may need to be replicated and/or clarified which may involve messaging the client and/or uploading files to this Trello card.</td>
  </tr>
  <tr>
    <td> Ready to Begin </td>
    <td> Items will remain here until the development team is ready to begin the sprint in which this item lives. </td>
    <td> The D4 project manager will move this item into In Progress once they begin to work on this item’s sprint.</td>
  </tr>
  <tr>
    <td> In Progress </td>
    <td> When an item has this status, the development team is actively working on this item’s sprint. </td>
    <td> Once this item has been developed and tested by someone other than the developer, and the feature is now available for the customer to test, the item can be moved to In Review. </td>
  </tr>
  <tr>
    <td> In Review </td>
    <td> Items are moved here once they have been completed, tested by D4, and released to the customer. This is where the customer tests that everything is working the way they expected, and/or provide us with their feedback.</td>
    <td> If the subject of the card passes the customer’s testing, the customer should move this item to Done. <br><br>
        This process should be explained to the customer during the kick off meeting. However, customers sometimes do not embrace these duties. Instead, if the customer indicates that they are happy with the software release, we may move it to Done for them.<br><br>
        If it is not approved, the item can be moved back into Ready to Begin with a comment explaining the issue.
    </td>
  </tr>
  <tr>
    <td> Done </td>
    <td> Items in this status have been completed, tested and released. The customer has carried out their testing and indicated they are happy with what's been delivered. The item is now resolved.</td>
    <td> </td>
  </tr>
</table>

## Internal Tools

**Jira**

Jira is used within our own team. Every card in Trello should have a corresponding Jira ticket (the ID of which should be recorded on the Trello card to keep things clear). 

If there are any bugs or tasks we come across in our own testing, then these should be raised as tickets in Jira.

Jira tasks will then be grouped into sprints. Each sprint will be worked on in turn.

Within a sprint, Jira tasks will move through a series of statuses, these are:

* To Do 
* In Progress
* In Test
* Done

The meanings of these statuses, what should happen at each stage, and where the work item can go to next, is defined below:

<table border="1">
  <tr>
    <td> Status </td>
    <td> Meaning </td>
    <td> Next Step </td>
  </tr>
  <tr>
    <td> To Do </td>
    <td> Work on this item has not started yet. </td>
    <td> The project manager must:
      <br><br>
      <ul>
        <li>Set the priority of this work item.</li>
        <li>Assign this work item to a developer.</li>
        <li>Add more design detail to this work item so the developer and tester know what to build/test.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td> In Progress </td>
    <td> The developer is actively working on it. The project manager will not re-assign the work item to a different developer. </td>
    <td> Once the developer has completed development of the work item and tested the change themselves, the work item will be set to “In Test” but will remain assigned to the developer until the item is available for testing in the test environment. <br><br>
         Before testing is carried out, there will be ‘test handovers’ between the developer and tester for each ‘significant’ work item. This ensures discussions are had about the changes/fixes that have been carried out and that there aren’t any mix ups about what is required. <br><br>
         This also makes it easier for the tester to know exactly what changes have been made. <br><br>
    </td>
  </tr>
  <tr>
    <td> In Test </td>
    <td> The work item has been developed and tested by a developer and is ready to be tested by a tester. <br><br>
         Or, the tester is actively testing the work item. <br><br>
         All members of the team will have testing responsibilities. <br><br>
    </td>
    <td> Depending on the outcome of the testing, the work item will either be set to “Done” or to sent back to “To Do”, or left at “In Test” and sub-tasks created to document each of the bugs.<br><br>
         If the item is sent back, or any bugs are raised, the tester will add details of: <br><br>
         <ul>
          <li>What they did (steps to reproduce)</li>
          <li>What they expected to happen</li>
          <li>What actually happened</li>
         </ul>
         If only minor bugs are found, the tester may move this work item to “Done” but also create new work items in “To Do”.<br><br>
         See the Testing Process for more information.
     </td>
   </tr>
   <tr>
    <td> Done </td>
    <td> The work item has been developed, tested and released to the customer. </td>
    <td> </td>
  </tr>
</table>

**Slack**

Slack allows for private one to one instant messaging with each member of the team. There is also the team chat which can be used to convey messages to all members of the team.

Slack is great for:

 * Chatting and "being present" with the team
 * Asking a quick question where a meeting would be overkill
 * Optional stuff e.g. "Hey, checkout this interesting article I read"

But Slack doesn't have a "flag for follow up" feature like email does, it's easy to miss important things in amoungst the team chatter, and search is limited on the free tier. So:

 * If you need someone to see a thing, email it to them.
 * If you need someone to do something, email them
 * If you think the person might want to find this information again later on, email it to them

**Project Folder (Google Drive)**

Each project will have a project folder created in Google Drive. This will be used to store documents about the project such as the Design Documents. It is also a good place to store files that the team need to share.
      
      
    


