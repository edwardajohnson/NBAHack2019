# NBAHack2019
Final MAPE: 9.81%

Application for the 2019 NBA Hackathon 
Eman Smadi, and myself teamed up to do the business challenge and develop models to predict fan engagement.
 
 https://hackathon.nba.com/#home-overview

Summary
We analyzed and extracted features before running multiple linear regression models

Major components positively influencing the Engagement numbers (most positive influencer first)
- Type of Post : Video
- Day of Week : Sunday, Monday, highest respectively
- Player Count : Number of player tags in the Description
- Contains_tophashtag: One of the top 26 hashtags identified
- Season type : Regular season, as opposed to Offseason, playoffs, and finals (**)
- Timezone: Posts put out in peak EST time zone are found to generate more likes

Main components negatively influencing the Engagement numbers (most negative influencer first)
- All Other tags (@) : posts which have tags which do not contain one of the top 62 tags
- Hr_Mins: the later the post the lower is the engagement
- Total Tags (@) in post. : This means that the number of tags (if more than 2) do not positively increase the fan Engagement for that post
- Team count : The total count of each team in the dataset
- Timezone: Posts put out in peak EDT time zone are found to generate less likes
- Season is Offseason : Less fan engagement in the offseason compared to other season times
- ** The Higher number of likes generated during the regular season may be related to the numbers of NBA teams in competition

Additional ideas
If we had more granular descriptions of the categorization of each post e.g. game highlight, player birthday of story, statistics or game time score, we would have been able to deliver a better MAPE.

We decided to focus on linear regression to create the models ( predicting continuous variables), but we could have investigated using NLP (NLTK/SpaCey) techniques.

- On Saturday, September 21st, 2019, students, statisticians, developers and engineers will take part in the fourth annual NBA Hackathon. 

