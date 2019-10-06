---
title: Companion app for Toronto's most popular transit pass
question: What do travelers in the GTA need from a transit companion app?
tags: [personal, product design, prototyping, concept testing, user interviews, visual design]
thumb: /assets/images/presto/thumb.jpg
role: Personal • Product Design
---

## Background
This is a personal side project and in no way affiliated with Metrolinx or PRESTO Card. To keep the project as realistic as possible, I was mindful of technical constraints of the existing platform.

{% include figure.html
    src='../assets/images/presto/presto_tapping.png'
    alt='test'
    caption='PRESTO cards and their terminals can be found all cities in Southern Ontario. Source: blogTO'
    width='mw8'
%}

PRESTO is the contact-less payment card used by public transportation systems across Southern Ontario. Users can manage their card in-person at transit terminals or online through a desktop web app. I researched the space and prototyped a mobile app to help travelers on-the-go.

## Hypothesis
When I realized the company was lacking a mobile app to pair with their transit cards, I hypothesized pain points that users might encounter. 

### Loading balance
There are currently three ways for users to load their card:

1. In-person at a transit terminal customer service desk
2. Online through the web app
3. Some GO buses drivers can load PRESTO cards if the passenger pays with cash

Each of these methods propose significant challenges for mobile users. Travelers only go to transit terminals when they board or get off of a bus or train and are usually pressed for time when they arrive or depart. Loading through the web app takes 24 hours for funds to be accessible and loading as you board the bus requires you to bring cash and holds up the line up of passengers behind you.

{% include figure.html
    src='../assets/images/presto/go_lines.png'
    alt='test'
    caption='Long lines make it difficult for travelers that are pressed for time to load their cards. Source: Transit Toronto'
    width='mw8'
%}

## Users
There are [2.8 million PRESTO card users][1] which is 30% of the entire population in Canada’s Golden Horseshoe area, PRESTO’s region of operation. These users are mostly commuters that travel from the suburbs to the city and people that travel occasionally to visit friends and family in different cities.

## First prototype and testing
I quickly designed a [prototype][2] to concept test with users.

This prototype included 5 sections of to the app:

- Home
- Activity
- Card view
- Loading card balance
- Common stops

I tested the prototype with 3 PRESTO Card users that had been using PRESTO for more than 6 months. I asked them about their habits as a traveler, how they used PRESTO and got them to try out different sections of the prototype.

In the following sections, I’ll explain my intentions behind the original design and how the users reacted.

### Home
I designed the Home screen to provide as much at-a-glance information as possible and hoped this would eliminate the need for users to navigate to other sections of the app.

{% include figure.html
    src='../assets/images/presto/v1_home.png'
    width='mw8'
%}

The Home screen included recent trips, balance, upcoming transit times, and cards to set up reminders and destinations. When I showed this to users, many users felt overwhelmed with information. Because of the abundance of cards, users only looked at certain elements on the page.

### Activity and Card View
To mirror the web app functionality, I designed a view for users to manage their card and keep track of their trips and other transactions.

{% include figure.html
    src='../assets/images/presto/v1_activity.png'
    caption='Card screen (left), Activity screen (right)'
%}

There were weren’t many problems with the Card screen, but all the users had some trouble with the table cells in the Activity screen.

I originally designed the list items using a design similar to the transactions items we used at one of my previous internships where I worked on a banking app for TD Bank. However, this design broke down when trying to show start and end points for a trip. No one understood the arrow meant to connect the start point and destination and the text hierarchy did not support the information.

### Loading card balance
I decided to use a bottom card for the Load card flow with the intention of giving users the feeling of a quick and non-obtrusive experience.

{% include figure.html
    src='../assets/images/presto/v1_payment.png'
    caption='The Load card flow used a bottom card to drew on top the current content.'
    width='mw8'
%}

When I showed this to users, the results were opposite from when I originally intended. Because users could still see content underneath the card, it didn’t feel like they had committed to a payment flow. One user even went through the flow without realizing they were adding money to their card, they simply did actions with the intention dismiss what they interpreted as a popup.

### Adding common stops
From the home screen, users could launch a flow that would allow them to add their most commonly visited GO transit stops. The app would provide bus times for those stops and use GPS to send a notification to users to tap off when their approach their stop.

{% include figure.html
    src='../assets/images/presto/v0_stops.png'
    width='mw8'
%}

I realized my assumptions about why people were not tapping off were wrong. All the users I interviewed explained that they only forgot to tap off when they first got their PRESTO Cards — nobody had explained it to them when they got the cards.

While the design of the flow tested well, the concept of push notifications didn’t. Users weren’t sure of how it would work in practice and did not understand the copy that explained it in the app.

What I didn’t expect was users to really like seeing arrival times on the home screen.

{% include figure.html
    src='../assets/images/presto/v1_time_cards.png'
    caption='Prompt for setting up your custom destinations (top), departure times card (bottom)'
%}

## Key learnings
After testing the first prototype, I summarized what I learned.

1. The home screen had too much information. Users felt overwhelmed, so they only looked at the information that caught their eye.
2. Activity cells were confusing, the icons were ambiguous and the type hierarchy did not support the structure of the content.
3. The payment flow did not make users feel like they were committing to a payment.
4. My assumptions about why users erroneously did not tap-off were wrong: once they learned they had to do it, they never forgot.
5. Users liked seeing bus times in the app because it helped them plan their trips preemptively.

## Revised design
Using what I learned, I re-positioned the app to target a broader scope for all of Metrolinx and tweaked the visual style of the app to match Metrolinx’s rebranding.

{% include figure.html
    src='../assets/images/presto/v2_home.png'
    caption="Top level destinations for the app: Home (left), Card (center), Activity (right)"
    width='mw8'
%}

I cleaned up the app Home screen and reduced the content to a card balance and nearby stops. I ditched the concept of common stops and push notifications but kept the transit times — using GPS to locate nearby stops instead.

On the Card screen, I changed the floating action button to a standard button underneath the card to make the action more consistent with the Home screen.

I adjusted the type on the Activity screen and added logos to help users identify which transit system they used.

{% include figure.html
    src='../assets/images/presto/v2_payment.png'
    width='mw8'
%}

I decided to use a full-screen flow for loading the balance on cards to make the whole process give a strong feeling of commitment and added a receipt to the success state to help assure users the transaction went through.

## What I learned

As a product designer, I learned a lot from this project, here were some of my key takeaways:

**Do research first.** On a new project or dramatic overhaul, it’s best to collect data on your
users first to reduce the time spent reworking things when your
assumptions are proven wrong.

**Users can get overloaded.** I originally thought showing the most information upfront would
streamline the experience for users, instead the opposite effect
happened. For something like a home screen, it’s important to critically judge the importance of all the information displayed.

**Payment flows need to instill confidence.** When users are spending money, they want to know that their transaction is secure and be sure that it has processed successfully.

## Next steps
If I were to continue this project, I’d look into ways to educate new PRESTO Card users about tapping off and ways to help users plan their trips ahead of time. I'd also try to run a second round of testing with my new prototype.

[1]: https://torontosun.com/2017/06/27/metrolinx-presto-rollout-millions-over-budget/wcm/f259bfa2-ddd7-4d35-ae99-f9979c2bec86

[2]: https://projects.invisionapp.com/share/B7212631492AE4#/screens