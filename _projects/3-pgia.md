---
title: Mapping information architecture for construction documents
question: How do mental models of construction documents map to a digital space?
tags: [product design, usability testing, information architecture]
thumb: https://images.unsplash.com/photo-1503387762-592deb58ef4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=900&q=60
role: PlanGrid • Product Design
---

## Background
PlanGrid, an Autodesk Company builds productivity software for the construction industry.

As a product design intern on PlanGrid's Field Reports team, I conducted looked at usage analytics, conducted interviews, and ran tests to identify usability issues with our information architecture and suggest design changes for our reporting tool.

## Issues with the current design
PlanGrid has a product called Field Reports that helps construction workers fill out reports and send them to their supervisors. These reports can include daily logs, safety checklists and time sheets and are required for legal liability purposes on the construction site.

{% include figure.html
    src='../assets/images/pgia/sample_reports.jpg'
    width='mw8'
    caption='Examples of field reports that a user might fill out on PlanGrid.'
%}

In Field Reports, report *managers* can upload blank PDF templates and assign them to *submitters* to fill them out. In the system, blank PDFs are referred to as *templates* and submitted documents are referred to as *reports*.

The problem was that the way they were represented in our interface caused people to constantly get confused between the template and report objects. We had a high volume of customer support tickets stating users were confused by the functionality of each of the objects. On top of this, PlanGrid employees would constantly mistake one of the objects for the other during internal meetings!

{% include figure.html 
    src='../assets/images/pgia/reports_templates.jpg'
    caption='The table view for reports (top) and templates (bottom) looked extremely similar. '
%}

When users open Field Reports, they are shown a list of templates. If they want to create a new report or see a list of submitted reports, they need to click a template in the table view, then they'll see all the reports submitted using that template.

The purpose and functionality of reports and templates are drastically different. If users were getting confused between them, it would cause serious usability issues. For example, if a user wants to submit a daily report but instead creates a template, they are brought to a completely different process that could get them disoriented in the interface.

## Usability Testing
To test our hypothesis, I ran 5 usability tests with different construction workers that had never used PlanGrid before. 45-minute long sessions were held with each of the users. The sessions began with a brief overview of the Field Reports process then the users were asked to complete a set of tasks and to think aloud as they proceeded.

Depending on their occupation, users were assigned to either act as a manager and create templates for other users to submit or fill out and submit a report to a hypothetical supervisor.

## Findings
There were three key usability findings that were noted by the team after running the usability tests.

### 1. People indeed get confused by templates and reports
All the participants were confused between templates and reports in some way. Often, users would be confused by by the view. They weren't sure whether they were looking at a list of templates or reports. In worse cases, users would accidentally create templates when they were trying to create a report and get extremely confused.

> I want the checklist thing... I have no idea how to create a report. <br> All I see is 'Add'. -P4

In the excerpt above, the 'Add' the participant is referring to creates a new template. 

### 2. Can't find specific reports
Users also had difficulty finding individual report submissions. Whether they were acting as a manager looking for a report their subordinate filled or a submitter looking for a report they previously submitted, users had trouble parsing the list of reports. Users noted they wanted to be able to easily find reports they recently submitted to ensure they were submitted correctly and refer back to them for future submissions.

While the reports view does offer the functionality to filter reports by specific characteristics such as date and status, none of the participants noticed this functionality. The inability to locate reports was also likely exaggerated by the similarities of the template and reports views because different filtering options are available for reports and templates.

### 3. It's hard to edit templates

Users that served as managers had difficulty editing templates that currently existed. Editing existing templates wouldn't be a common task, but could be required to reassign permission levels or if a PDF template needs to be updated. However, all the users were completely lost when asked to edit report permissions.

> There's a feature like that? I can't find it. -P2

## New design proposal
After synthesizing the findings from the usability testing, my internship was coming to a close. Before I left PlanGrid, I explored a few different information architecture and navigation patterns to address the usability issues we discovered. These early explorations were handed off to another designer that ended up refining them and launching the new designs. 

My design explorations focused on different navigation patterns. One exploration emphasized filtering and searching heavily, another kept the same navigation pattern, but tried to visually distinguish the template and report objects. The exploration that ended up getting implemented was *tabbed navigation*.

{% include figure.html 
    src='../assets/images/pgia/new_design.png'
    caption='A mock of a tabbed navigation that introduced top-level destinations for Home, Reports, Templates and Insights'
    width='mw8'
%}

The tabbed navigation separated reports and templates into two separate tabs and added a new home and insights page. The decision to split reports and templates into two separate tabs was supported by the realization that the objects are often associated with different roles. Report managers are often thinking about the interface in terms of templates whereas report submitters are often thinking about their tasks in terms of reports. As [Jakob Nielsen highlights](https://www.nngroup.com/articles/tabs-used-right/), a good use of tab navigation is when users don't need to see content from multiple tabs simultaneously. 

## Updated results
While my internship ended before I could conduct a second round of testing, the new design I proposed was implemented and tested after I left. 

Through usability tests, the new designs proved to decrease the confusion around templates and reports and help new users find specific reports, but still left users confused about how to edit templates. 

From a quantitative perspective, after the new design launched, there was an improvement in the number of weekly submitted reports, a key success metric, that was statistically significant. 

## Learnings and next Steps
In my 6-week period with the Field Reports team at PlanGrid, I learned the value of information architecture and testing on maintaining a positive product experience. Even after making design changes and decreasing the confusion around the product, there's still lots of room to improve. If I were to continue this project, I'd take a deeper dive into the interaction patterns we are using for editing templates and continue to explore how they align with the mental models of our users.