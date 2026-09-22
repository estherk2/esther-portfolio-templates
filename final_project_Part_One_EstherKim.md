| [home page](https://github.com/estherk2/esther-portfolio-templates) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final_project_Part_One_EstherKim) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

## Outline 
This project explores how K-pop has spread across global music markets by analyzing daily Spotify chart data from 73 countries. 
Using artist name, song title, country, daily rank, and daily movement, I will identify which countries K-pop artists chart in, how high they rank, and whether their position is rising or falling.

The goal is to show a geographic pattern of K-pop's reach, highlighting countries where K-pop has strong, stable chart presence versus countries where it is newly emerging or losing ground.

[Project Structure]

The story opens with a filled map of all 73 countries, colored by how many K-pop tracks appeared in daily Spotify charts at any point between August 2024 and June 2025. 
The reader's first reaction should be surprise at how wide the color spreads. This establishes the scale first.

The view shifts to a line chart tracking the number of charting K-pop tracks per country, month by month. Most lines stay flat and low. 
A handful rise steadily. One or two spike sharply within a single month. 
I annotate these spikes directly on the chart, naming the country and the month. 
This is where the reader starts asking why.

I split the countries into two groups and place them side by side. 
The first group holds the steadiest presence across all eleven months, deep but slow. 
The second group shows the sharpest month-over-month growth, fast but recent. 
A few countries land in both groups, and I call that out specifically, because it is the most interesting finding: markets that started strong and are still accelerating.

[User Stories]
- As a music industry analyst, I want to see which countries have the most consistent K-pop chart presence, so I can identify markets worth long-term investment.
- As a label executive, I want to see which countries show the fastest recent growth in K-pop streaming, so I can prioritize where to launch a new artist or tour.
- As a casual reader, I want a single map I can look at and immediately understand where K-pop is strong and where it is emerging, without reading a report.

## Initial sketches
The sketch follows my story arc: a map of K-pop's reach (setup), monthly growth with key spikes (rising action), steady vs. fast-growing markets (climax), and what it all means (resolution).
<img width="1312" height="1199" alt="Final Project 1 Sketch" src="https://github.com/user-attachments/assets/d3542877-4b31-4eb4-8d21-a58e677c8229" />

## The data
This project uses the "Top Spotify Songs in 73 Countries (Daily Updated)" dataset, published on Kaggle by user asaniczka. 
The dataset tracks the most popular songs on Spotify across 73 countries, updated daily, and includes artist name, song title, country, daily rank, and daily movement (the change in rank from the previous day). 
I downloaded a copy covering August 2024 through June 2025.

I plan to filter this dataset down to K-pop artists only, using a manually compiled list of major K-pop acts (e.g. BTS, BLACKPINK, NewJeans, Stray Kids, TWICE). 
From there, I will aggregate the number of charting K-pop tracks per country per month to show where K-pop has a steady presence versus where it is newly emerging. 
Daily movement will help identify countries with the sharpest recent growth.

Name : Top Spotify Songs in 73 Countries (Daily Updated)
URL : https://www.kaggle.com/datasets/asaniczka/top-spotify-songs-in-73-countries-daily-updated

## Method and medium
I plan to build the data visualizations in Tableau, then use Shorthand to build the narrative structure around them. 
Each Tableau chart (the filled map, monthly line chart, and market comparison bar charts) will be published to Tableau Public and embedded directly into the Shorthand story, following the story arc from my outline: setup, rising action, climax, and resolution.

## References
Kaggle dataset: "Top Spotify Songs in 73 Countries (Daily Updated)" by asaniczka. 

## AI acknowledgements
I used ChatGPT to help create the sketch image for this proposal. 
I also used Claude to help answer some questions I had while working on this assignment. 
I reviewed and edited all content before submitting.
