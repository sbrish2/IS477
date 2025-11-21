# Overview
<p>My goals for the project have not changed. I will still be examining how Hollywood film budget, genre, and ratings are related to box office performance. I have kept the datasets from Kaggle and Mendeley Data the same. I am examining all of the same research questions that I initially had proposed.</p>

# Contributions
<p>I am the only member of my team, so I have taken care of all analysis and work associated with the project. I will break down my entire process. My initial timeline looked like this:<br>Timeline:<br>

* Week 1: Define project plan and get datasets
* Week 2/3: Clean and join datasets using pandas
* Week 4: Perform exploratory analysis and summary statistics on the data
* Week 5: Analyze correlations and produce visualizations
* Week 6: Finalize report<br><br>
I have loosely followed this schedule, and now, in my 6th week of project work, I have done most of my analysis and made most of my visualizations. I do not think that these are my final observations, but I think I have made decent headway into what I’ve planned on completing for the project. Starting off, I loaded each of my datasets into my Jupyter notebook individually.<br>For the first dataset, movie_info.csv from Mendeley Data, I renamed the ‘title’ column to have a capital T so that it would match the other dataset’s column name, in order to later merge on this column. Next, I put the data from “release_date” into a new column “Year” so that it would match the other dataset, to make things simpler for myself. In doing this, I also standardized the formatting of the column’s rows, taking them from ‘Released Dec 16, 1970,’ to ‘1970,’ for example. Then, I dropped the features that were unnecessary for my analysis: ‘url’ and ‘release_date’ (since we had made the new column ‘Year’ using its data). Then, I dropped any duplicate films from the dataset. After this, I converted the rows of ‘critic_score’ and ‘audience_score’ from string values (ex: 79%) to numeric values (ex: 79.0) for analysis later on. After that, I dropped any rows with NaN values. This took the dataset from its initial 12,413 rows down to 8,056 rows after all the cleaning was said and done.<br>
For my second dataset, ‘Highest Holywood Grossing Movies.csv,’ after loading it in, I dropped the columns that were unnecessary for my analysis: 'Distributor', 'International Sales (in $)', 'World Wide Sales (in $)', 'Running Time', 'License', 'Movie Info', 'Unnamed: 0', 'Release Date'. Some of these were simply dropped because they were not relevant to my research questions, and others, like ‘International Sales (in $)’ and ‘World Wide Sales (in $)’, were dropped for simplicity. Since I only had domestic box office info, I decided to narrow my analysis down to domestic sales only. ‘Release Date’ was dropped only because it was redundant, as the column ‘Year’ already existed in the dataset. After this, I dropped duplicate rows, and standardized formatting of both budget and box office info, similar to what I did with the release date data from the first dataset. Then, I dropped NaN values. After I was done with my cleaning, the dataset went from 1,000 rows to 763.<br>After merging the two datasets on ‘Title’ and ‘Year’, I was left with 539 rows across my eight chosen features. </p><br>I’ve separated the project into four segments, one for each of my research questions. For each one, I’ve created relevant correlation tables or specificized datasets, along with visualizations examining the relationship between the variable pairings I’ve chosen. I plan to explain conclusions that I draw from these, and possibly go even further with my analysis.</p>

# New Timeline<br>
* Week 1: Define project plan and get datasets
	* Status: **Complete**
* Week 2/3: Clean and join datasets using pandas
	* Status: **Complete**
* Week 4: Perform exploratory analysis and summary statistics on the data
	* Status: **Not Complete**
* Week 5: Analyze correlations and produce visualizations
	* Status: **Not complete**
* Week 6: Finalize report
	* Status: **Not complete**<br><br>
<p>The new timeline for the rest of the semester’s time will look like this. I’ve completed some analysis, and created some visualizations, but I want to finalize these things and possibly go more in depth in my analysis. Once that is complete, I will create my final report, going over everything.</p>

# Changes
<p>Not much changes for me about the project, especially considering that the feedback I received for my initial project proposal was entirely positive. Unless there are changes observed from the progress I have made so far, I think I am on track to continue as I have been going without changing much beyond what I have outlined so far. That said, there are a few minor things that I will address.<br>First, I originally proposed one of my research questions as asking how strongly IMDB ratings correlate with box office performance. This was an oversight of mine, due to not examining the data closely enough before downloading. The ratings instead come from Rotten Tomatoes, so I’ve rephrased the question as simply asking about “ratings” instead.</p>

# Notes
<p>As I mentioned before, I decided to focus on domestic sales for my analysis. My reasoning is that it will make sure that my analysis is consistent, and it will keep me from having to adjust for any regional differences. In the same vein, I mentioned inflation and significant events like the Covid-19 pandemic as potential gaps in my initial project proposal. After looking at the data, I decided that I was right that these would be too outside of the scope of this project for me to explore in-depth enough. I would need a lot of external data, and would need to carefully select it all to ensure proper analysis, and my timeline simply will not provide me with enough room for this. With these changes, I can acknowledge them as limitations and maintain clarity in my project scope. The same goes for analyzing the specific content of each film review.<br>
I also would like to note the size of my merged dataset is much smaller than I had expected after all of my cleaning. This may mean that my analysis, based on a smaller amount of data, may not be as reflective of real-life industry trends as I had initially hoped. All in all, my research questions and fundamentals of my project remain the same, but I acknowledge the limitations of what I can complete here.
