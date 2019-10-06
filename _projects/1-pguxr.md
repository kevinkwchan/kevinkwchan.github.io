---
title: Debunking assumptions about the construction industry
question: Can user research unblock a team that doesn't know what to do next?
tags: [user interviews, stakeholder interviews, quantitave + qualitative data, assumptions modelling]
thumb: https://images.unsplash.com/photo-1531834685032-c34bf0d84c77?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1974&q=80
role: PlanGrid • UX Research
---

## Background
PlanGrid, an Autodesk Company builds productivity software for the construction industry. 

When I joined as a user research intern, the Growth team had already started working on a new onboarding initiative but were stuck on what to do next. As a researcher, I modeled assumptions and used quantitative data to expose assumptions, conducted research to validate those assumptions, and worked with the team to figure out a course of action.

## Business problem: customer acquisition
As the name suggests, PlanGrid's Growth team is tasked with growing our customer base. Vital to achieving this goal is understanding how the company acquires new customers.

Most customers follow a typical funnel when becoming a paying customer. They first interact with marketing content of some sort, explore the product on their own, then get in contact with sales to purchase a license.

{% include figure.html
	src="../assets/images/pguxr/pg-sales-funnel.svg"
	alt="Welcome messages and survey questions in the new onboarding flow."
	caption="PlanGrid's sales funnel can be broken down into lead generation, product trial, negotiation and close."
%}

Before I joined, the team had studied this funnel and found that there was a large drop in conversion on the second step: free trials. After some investigation, they learned from analytics that many of the new users that drop off on the first day go through the sign-up process, then leave without really doing anything.

{% include figure.html
	src="../assets/images/pguxr/funnel-dropoff.svg"
	alt="Welcome messages and survey questions in the new onboarding flow."
	caption="The drop-off from the free-trial to sales step was by far the largest in our sales funnel. "
	
%}

Many new users drop-off after the first day. This initial drop highlighted how important a users early experience with PlanGrid was. If we could increase retention past day 1, our sales organization would have a bigger pool of potential customers to work with.

## An experience-centered approach
With this knowledge, the Growth team hypothesized that the existing in-product onboarding experience needed to do two things better for new users:

1. Discover PlanGrid's features that were relevant to them
2. Learn how to use the features to get work done

From there, the team designed and released to users a set of onboarding flows that bucketed users into different categories and taught them how to complete certain tasks that would help them understand PlanGrid's value on construction projects.

{% include figure.html
	src="../assets/images/pguxr/initial-onboarding-designs.png"
	alt="Welcome messages and survey questions in the new onboarding flow."
	caption="Welcome messages and survey questions in the new onboarding flow."
	width="mw8"
%}

Success was to be measured quantitatively by an increase in customer retention.

## Disappointing results
I joined the team after the designs had been launched for a few weeks and quantitative results were just starting to come in.

The team had released the new designs to an experimental group of users for a 4-week period. Unfortunately, it did not have the results the team was hoping for. 1-day and 4-week retention had only improved 1-2% and in some cases, performed worse than the original design.

## Assessing the situation
When I joined the Growth Team, the first thing I did was try to figure out how they ended up in this situation. By speaking with project stakeholders and digging through documentation, I learned that while the team had good intentions of improving the user experience, they hadn't conducted any qualitative research and were operating primarily on assumptions that included...

- how to divide users
- what their value propositions would be
- and how to showcase these theorized value propositions through design

If any of these assumptions were proven to be wrong, the new onboarding flow wouldn't achieve the results we wanted it to. Realizing this, I thought the team needed to take a step back and validate these assumptions with user research before moving forward.

## Preparing tools
I created a visual model of the assumptions that were being made to help illustrate this to the team.

{% include figure.html
	src="../assets/images/pguxr/assumptions-model.jpg"
	alt="Welcome messages and survey questions in the new onboarding flow."
	caption="The model highlights 3 core assumptions: users, value propositions and design implications."
	width="mw8"
%}

The team thought that there are two types of people that would get value out of PlanGrid. We referred to people who distribute construction documents as _administrators_ (admins for short) and people who use construction information to do work as _collaborators_ (collabs for short).

{% include figure.html
	src="../assets/images/pguxr/survey-question.jpg"
	alt="Welcome messages and survey questions in the new onboarding flow."
	caption="When new users sign up, they were presented with a multi-select option that would route them to different flows."
	
%}

If a user selected "I manage and distribute information like sheets and documents" or "I do both" they were prompted to upload a set of blueprints. If they selected "I read or markup sheets and documents" or "I'm not sure" then they would be shown PlanGrid's annotation tools on a set of sample blueprints.

The team expected that most people would fall into the admin or collab categories, but the results were the opposite. 

{% include figure.html
	src="../assets/images/pguxr/expectations-v-reality.svg"
	alt="Welcome messages and survey questions in the new onboarding flow."
	caption="When new users sign up, they were presented with a multi-select option that would route them to different flows."
	width="mw8"
%}

## Getting buy-in for user research
I presented visual model for assumptions and used the quantitative survey data to reinforce my thesis. Many of the Growth team members were not fully aware of the assumptions that were made and how they were influencing design decisions.

{% include figure.html
	src="../assets/images/pguxr/assumptions_presentation.png"
	alt="Welcome messages and survey questions in the new onboarding flow."
	caption="I held a meeting to help the team realize the assumptions we were making and align on next steps."
	width="mw8"
%}

The discussion naturally led to next steps. We decided to try to verify the assumptions we made through qualitative research.

## User interviews
We decided to interview users to answer two main research questions:

1. What are different value propositions a new user can experience with PlanGrid?
2. What did their journey from a new user to becoming a paying customer look like?

By answering these questions, we would have a better idea of what different user groups exist and how to show upfront value for them.

From these research questions, we developed a set of screener criteria which included:

- user signed up and converted within the past year
- user was not invited by another user
- the first user to sign up from their organization

These criteria were intended to give us users who had found PlanGrid on their own, gone through the previous onboarding process, and decided to convert.

{% include figure.html
	src="../assets/images/pguxr/user-learnings.svg"
	alt="Welcome messages and survey questions in the new onboarding flow."
	caption="User research identified three key learnings about user groups, feature spread and the journey towards conversion."
	
%}

After synthesizing our observations from our five user interviews, we identified three key trends:

1. These users were only using a limited feature set that solved a tightly scoped problem they ran into in their construction work
2. The users we spoke to were primarily using PlanGrid on their own
3. Conversations with sales played a large part in them understanding the product

These insights troubled the Growth Team. We had discovered a way of using PlanGrid that didn't align with our expectations; and we wanted to learn more. Specifically, we wanted to know:

- How big of a group are these "single-player" users?
- What other categories of customers are there?
- What does the engagement with PlanGrid sales reps look like?

To answer these questions, we decided to turn to our own internal employees and interview some sales reps.

## Sales rep interviews
We interviewed five of our own sales reps from across the United States to answer the questions above. We asked them how they build interest with the customers they talk to and if there are any ways they categorize users. We had two key takeaways.

{% include figure.html
	src="../assets/images/pguxr/affinity-diagram.jpg"
	alt="Welcome messages and survey questions in the new onboarding flow."
	caption="Excerpt from our team's synthesis session."
	
%}

**Value propositions change depending on company type**

When we asked the sales reps about the different kinds of clients they talk to, they said there were some people who wanted to use PlanGrid on their own, but most customers fell into three categories.

*Owners* are companies that purchase property and initiate the construction project. This could be the government, universities, or a company. It turns out their primary value proposition is getting visibility into the the construction site to make sure things are running smoothly and on time.

*General contractors* are companies that are hired by the owner to manage all the construction operations. They will be the ones hiring sub-contractors to carry out specific trade tasks and managing the budget and timeline. For them, their value proposition is generating reports and getting construction documents to the field.

*Sub-contractors* are companies in charge of carrying out different trades such as painting, plumbing, electrical, and mechanical. They care about simplifying work on the field to save time and prevent re-work.

{% include figure.html
	src="../assets/images/pguxr/customer-categories.jpg"
	alt="Welcome messages and survey questions in the new onboarding flow."
	caption="We identified three customer categories: owners, general contractors, and sub-contractors."
	
%}

**Many users are mandated to use PlanGrid and have low expectations about the software because of their previous experiences**

General contractors are often already using some software system in this day and age. Because they manage the construction project, they have the authority to mandate the sub-contractors they hire to use PlanGrid. The sub-contractors learning about PlanGrid this way don't receive a proper explanation from their general contractors and don't understand how PlanGrid is different from other clunky software they've used (like FTP servers).

All of the sales reps we spoke to mentioned this population of users as being a group that they usually have to work very closely with to show them how PlanGrid can be applied to their work. They think there's a huge opportunity here to help users better understand how PlanGrid is different from other software systems during onboarding.

## Conclusions and prioritization
I don't think the Growth Team's initial approach of showing new users the parts of PlanGrid that can deliver upfront value during the onboarding process was not inherently flawed. However, through qualitative interviews, we found that the assumptions the team made about how to split up users and the value propositions for their user groups were not entirely accurate.

Although my internship ended before the team began revamping their onboarding designs, I left off by helping the team make decisions about concrete next steps based off the research. 

First, we would segment new users by whether they were an owner, general contractor, or sub-contractor and tailor the onboarding experience based off the value propositions we learned about. Then, we decided to focus primarily on the sub-contractor demographic first. We understood there was a problem for this population that needed to be solved and an opportunity for onboarding to help them. We would attempt to use onboarding to move the needle on this population first to validate our approach before attempting to build out full flows for the general contractor and owner demographic.

## Learnings
I had an amazing time as a user research intern at PlanGrid. Over the four months, I learned how to plan and execute research studies, facilitate discussions, and advocate for our users when making product decisions. Here are my top reflections from the term.

**Combine qualitative and quantitative data**. The Growth team started off purely looking at numbers without building a solid qualitative understanding of their users. The data we collected from the initial survey question served as a great signal that an assumption we were making was wrong. This signal served as a guide to direct our qualitative user research. Using both methods were key to telling a complete story.

**Using customer proxies to supplement the research process.** To be clear, customer proxies are *not* a replacement for talking to real customers. However, they can help you understand a larger context for the data you're collecting. For example, when we recruited users, we found only single-player customers. Only after speaking with sales reps did we realize this was a small minority of our user-base.

**The researcher as a guide.** A user researcher needs to have a good handle on how their team is operating in order to be effective. As the one often facilitating discussion around user-centered topics, the researcher has the opportunity to reveal to the team their own implicit decision making process and provide a path to collect the research they need.

## Acknowledgements
Shout outs to my manager Christiana, my teammates Peter and Ronald and the rest of the Growth team for their support and collaboration in this project. Most of all though, thank you to Joe Kappes, my research mentor, for developing my love for and way I view user research.