# How do people react to social distancing in the U.S.?

## Problem Statement
Living through a pandemic proposes unique challenges to data science. The Internet contains a wealth of information about how society reacts to a dangerous and stressful situation as a whole, as well as a multitude of individuals. From the prospect of the individual who tries to make sense of the rapidly changing trends and events, this wealth of information can easily turn into the source of misunderstanding and fear. Some states have enacted strictly enforced stay-at-home policies, while others have provided general guidelines. Do stay-at-home policies prevent increases in positive cases? In comparing regional responses to COVID-19, what is the general public sentiment in response to state policies? 

## Executive Summary
Our team began with defining and familiarizing ourselves with Executive Orders per state. We were able to hone in on the top keywords used in policies, in turn we used each keyword as a query when pulling in posts as our data from Twitter.

**Keywords Used:**

1. Business Closures
2. Coronavirus
3. COVID 
4. Election Postponed
5. Emergency Declaration
6. Executive Orders
7. Mandatory Quarantine
8. Restaurant Closures
9. School Closures
10. Shelter-in-Place
11. Self-Quarantine
12. State Mandates
13. Governor

We were successful in pulling 59,000+ posts from Twitter using a Twitter wrapper called [GetOldTweets3](https://pypi.org/project/GetOldTweets3/). The parameters we used were: "query_term" (keyword), "date" (February 2020 - May 10, 2020), "state", and "text" (post). We were able to run a sentiment analysis with our collected data. 

*Disclaimer: at the present time this Twitter wrapper (GetOldTweets3) is not able to pull geo data.

In attempting to answer these questions, our team build an easily accessible and interpretable system that compiles relevant information in real time and reduces it into digestible pieces

View our [INTERACTIVE MAP - 1](https://public.tableau.com/profile/bibor#!/vizhome/COVID-19_15899821421350/FullyInteractive) and [INTERACTIVE MAP - 2](https://public.tableau.com/profile/bibor#!/vizhome/COVID-19DailyIncrease/CovidIncrease). (Phase 1)

To answer our current problem statement, at the moment we are not able to build a reliable statistical model that reflects trends that we have observed. The current sentiment on Twitter is relatively neutral. Times are rapidly changing; therefore sentiment is volatile with uncertainty towards state-mandates.

Future ideas moving forward: 
- Embedding an interactive GIS application (Phase 2)
- Real-time sentiment analysis. Generating live sentiment analysis score. (Phase 2)
- Increasing map information to include Per capita rates. (Phase 2)
- Build a text-recognition system which will automatically download Executive Orders from state government websites. Transform PDF files into easily searchable text. Automatic information updates on the map, build a code to pull data from a tracker to output that same data onto the interactive map. (Phase 3)

**[Presentation]**(Client Project #5.pdf)
