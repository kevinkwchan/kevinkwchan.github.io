---
title: Guiding a team to make product decisions by debunking assumptions
tags: [PlanGrid, Research, Interviews, Workshop Facilitation, Quantitative Data Analysis]
thumb: /assets/images/pguxr/thumb.jpg
---
<div class='mw7' markdown='block'>
{% capture intro %}
As a user research intern on PlanGrid's Growth Team, I combined quantitative analysis with user and internal stakeholder interviews to identify value propositions, customer segmentations and prioritize target populations.
{% endcapture %}

{% include blockquote.html content=intro %}

## Company background
PlanGrid builds project management and field productivity software for the construction industry. The company launched in 2013 with an iPad app that allowed users to markup blueprints on a mobile device and eliminates the need for bringing expensive paper blueprints to construction sites. Over the years, PlanGrid has expanded its scope to cover many more construction related tasks.

</div><!-- wrapper -->


{% include figure.html
	src="../assets/images/plangrid_website.png"
	alt="Screenshot from the PlanGrid website"
	caption="PlanGrid, an Autodesk company builds software for construction productivity."
	width="mw8"
%}

<div class='mw7' markdown='block'>
## Business problem
Most customers follow a typical funnel when becoming a paying customer. They first interact with marketing content of some sort, explore the product on their own, then get in contact with sales to purchase a license.

As a product organization, we noticed that there was a significant portion of new users that drop off very early. This makes it difficult for sales reps to reach out to them and work with them to fit PlanGrid to their needs before trying to close a deal with them. 

As of early 2019, our 30-day retention graph looked a little like this:
</div><!-- wrapper -->

{% include figure.html
	src="../assets/images/pguxr/retention.png"
	alt="Graph showing 30-day retention. Steep drop-off on day 1."
	caption="30-day retention for new users that sign up for PlanGrid."
	width="w60"
%}

<div class='mw7' markdown='block'>
Many new users drop-off after the first day. This initial drop highlighted how important a users early experience with PlanGrid was. If we could increase retention past day 1, our sales organization would have a bigger pool of potential customers to work with.

## Initial approach
When I joined as a user research intern, the Growth Team at PlanGrid had already been trying to solve this problem. At first, they tried to think through different reasons as to why there was such a steep drop-off on day 1. Was our pricing too high? Was our initial experience confusing? Did people have the wrong expectations going into our product? There are a lot of potential reasons why someone might leave your app or website. 

After looking at some of the data, we noticed that many of the new users that drop off on the first day go through the sign-up process, click around in the app, then leave. The Growth Team hypothesized that through a better onboarding process, we could help people better understand the value proposition PlanGrid has to offer and thus increase retention within the first few days of a user's experience with our product.

From there, the team designed and released to users a set of onboarding flows that bucketed users into different categories and taught them how to complete certain tasks that would help them understand PlanGrid's value on construction projects.
</div><!-- wrapper -->

{% include figure.html
	src="../assets/images/pguxr/onboarding_designs.png"
	alt="Welcome messages and survey questions in the new onboarding flow."
	caption="Welcome messages and survey questions in the new onboarding flow."
	width="mw8"
%}

<div class='mw7' markdown='block'>
## Results
I joined the team after the designs had been launched for a few weeks and quantitative results were just starting to come in.

The team had released the new designs to an experimental group of users for a 4-week period. Unfortunately, it did not have the results the team was hoping for. 1-day and 4-week retention had only improved 1-2% (not a statistically significant result based off our sample sizes) and in some cases performed worse than the original design. 

On top of this, people were not responding the way we expected to the survey question that we used to route them into one of two onboarding flows. 
</div><!-- wrapper -->

{% include figure.html
	src="../assets/images/pguxr/survey_question.png"
	alt="Question with multi-select: Tell us about your role."
	caption="When new users signed up for PlanGrid, they were presented with this single-select question."
%}

<div class='mw7' markdown='block'>
The team thought that there are two types of people that would get value out of PlanGrid.

If a user selected "I manage and distribute information like sheets and documents" or "I do both" they were prompted to upload a set of blueprints. If they selected "I read or markup sheets and documents" or "I'm not sure" then they would be shown PlanGrid's annotation tools on a set of sample blueprints.

The team expected that most people would fall into one of these two categories, but the results were the opposite. 

{% include figure.html
	src="../assets/images/pguxr/survey_results.png"
	alt="Diagram dividing two user roles and motivations."
	caption="Survey results for the 'Tell us about your role' prompt."
%}

We included options for "Both" and "Not sure" out of curiosity, but they came out as the top-two selected results! The team was stumped and didn't know how to proceed. 

## Identifying assumptions
When I joined the Growth Team, the first thing I did was try to understand the process they took to arrive at the designs they did. The following diagram illustrates my understanding of the project.

{% include figure.html
	src="../assets/images/pguxr/mental_model.png"
	alt="Diagram dividing two user roles and motivations."
	caption="Diagram dividing two user roles and motivations."
	width="mw6"
%}

Without research, the team made assumptions about how to divide users, what their value propositions would be, and how to showcase these theorized value propositions through design. If any of these assumptions were proven to be wrong, the new onboarding flow wouldn't achieve the results we wanted it to.

I presented my understanding of the process to the team along side the results we were getting from the data. Along the way, I highlighted the assumptions that were made and how it impacted the way they designed the new onboarding process. Many of Growth Team members were not fully aware of the assumptions that were made and how they were influencing design decisions.
</div><!-- wrapper -->

{% include figure.html
	src="../assets/images/pguxr/assumptions_presentation.png"
	alt="Meeting with boy standing in front of TV"
	caption="That's me presenting assumptions in front of the TV!"
%}

<div class='mw7' markdown='block'>
After my presentation to the team, we discussed next steps. We decided to try to verify the assumptions we made through qualitative research.

## User interviews
We decided to interview users to answer two main research questions:

1. What are different value propositions a new user can experience?
2. How did their journey from a new user to becoming a paying customer look?

From these research questions, we developed a set of screener criteria which included:

- user signed up and converted within the past year
- user was not invited by another user
- the first user to sign up from their organization

These criteria were intended to give us users who had found PlanGrid on their own, gone through the previous onboarding process, and decided to convert.

After synthesizing our observations from our five user interviews, we identified three key trends:

1. These users were only using a limited feature set that solved a tightly scoped problem they ran into in their construction work
2. The users we spoke to were primarily using PlanGrid on their own
3. Conversations with sales played a large part in them understanding the product
</div><!-- wrapper -->

{% include figure.html
	src="../assets/images/pguxr/interview_learnings.png"
	alt="Diagram of 3 icons: Single Player, Limited Feature Spread, Contact with Sales"
	caption="We spoke to many 'single-player' users with a limited feature spread that likely only converted due to their engagement with PlanGrid sales reps."
	width="mw8"
%}

<div class='mw7' markdown='block'>
These insights troubled the Growth Team. We had discovered a way of using PlanGrid that didn't align with our expectations; and we wanted to learn more. Specifically, we wanted to know:

- How big of a group are these "single-player" users?
- What other categories of customers are there?
- What does the engagement with PlanGrid sales reps look like?

To answer these questions, we decided to turn to our own internal employees and interview some sales reps.

## Sales rep interviews
We interviewed five of our own sales reps from across the United States to answer the questions above. We asked them how they build interest with the customers they talk to and if there are any ways they categorize users. We had two key takeaways.
</div><!-- wrapper -->

{% include figure.html
	src="../assets/images/pguxr/affinity.png"
	alt="Photo of stickynotes on wall"
	caption="Excerpt from our team's affinity diagramming process to uncover insights."
	width="mw8"
%}

<div class='mw7' markdown='block'>

#### 1. Value propositions change depending on company type
When we asked the sales reps about the different kinds of clients they talk to, they said there were some people who wanted to use PlanGrid on their own, but most customers fell into three categories.

*Owners* are companies that purchase property and initiate the construction project. This could be the government, universities, or a company. It turns out their primary value proposition is getting visibility into the the construction site to make sure things are running smoothly and on time.

*General contractors* are companies that are hired by the owner to manage all the construction operations. They will be the ones hiring sub-contractors to carry out specific trade tasks and managing the budget and timeline. For them, their value proposition is generating reports and getting construction documents to the field.

*Sub-contractors* are companies in charge of carrying out different trades such as painting, plumbing, electrical, and mechanical. They care about simplifying work on the field to save time and prevent re-work. 

#### 2. Many users are mandated to use PlanGrid and have low expectations about the software because of their previous experiences

General contractors are often already using some software system in this day and age. Because they manage the construction project, they have the authority to mandate the sub-contractors they hire to use PlanGrid. The sub-contractors learning about PlanGrid this way don't receive a proper explanation from their general contractors and don't understand how PlanGrid is different from other clunky software they've used (like FTP servers).

All of the sales reps we spoke to mentioned this population of users as being a group that they usually have to work very closely with to show them how PlanGrid can be applied to their work. They think there's a huge opportunity here to help users better understand how PlanGrid is different from other software systems during onboarding.

## Conclusions and next steps

The Growth Team's initial approach of showing new users the parts of PlanGrid that can deliver upfront value during the onboarding process was not inherently flawed. However, through qualitative interviews, we found that the assumptions the team made about how to split up users and the value propositions for their user groups were not entirely accurate.

Although my internship ended before the team began revamping their onboarding designs, I left off by helping the team make decisions about concrete next steps based off the research. 

First, we would segment new users by whether they were an owner, general contractor, or sub-contractor and tailor the onboarding experience based off the value propositions we learned about. Then, we decided to focus primarily on the sub-contractor demographic first. We understood there was a problem for this population that needed to be solved and an opportunity for onboarding to help them. We would attempt to use onboarding to move the needle on this population first to validate our approach before attempting to build out full flows for the general contractor and owner demographic.

## Learnings

I had an amazing time as a user research intern at PlanGrid. Over the four months, I learned how to plan and execute research studies, facilitate discussions, and advocate for our users when making product decisions. It was super interesting being on the Growth Team because they have traditionally leaned very heavily on quantitative research, so I got to learn about data science and how to blend qualitative and quantitative research together.
</div><!-- wrapper -->