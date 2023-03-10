# Phase 1 Project Report
# Microsoft New Movie Studio

## Project Overview

In this project, I used exploratory data analysis to generate recommendations to invest in a new movie studio called Microsoft Movie studio.
The recommendations are useful as they will enable Microsoft to determine the best movies to produce which guarantee highest return on investment.

## Business Understanding
Microsoft has seen big companies create original video content, and they have dediced to enter in the industry. However, they have no understanding of the movie industry. As a data scientist, they have hired me to help them better understand the film industry. I am tasked with exploring the type of films that are currently best performing at the box office. I will be exploring the type of films that are currently performing best at the box office and then i will translate these findings into actionable insights that the head of the Microsoft New Movie studio will use to decide what type of films to create.
## Data Understanding

The following movie datasets were provided in the zipped folder `zippedData`:

* [Box Office Mojo] https://www.boxofficemojo.com/
* [IMDB] https://www.imdb.com/ 
* [Rotten Tomatoes] https://www.rottentomatoes.com/
* [TheMovieDB] https://www.themoviedb.org/ 
* [The Numbers] https://www.the-numbers.com/ 

The specific datasets used were :

1. Box Office Mojo Movie gross (domestic & worldwide)
2. Movie information
3. The Movie databse information (TMDB)
4. Movie budgets
5. Movie reviews
## Data Understanding 

This data was collected from different locations and the different files were in different formats which were CSV (comma-separated values),  TSV (tab-separated values) files that I opened using Pandas inbult function `pd.read_csv`. The data from IMDB was located in a SQLite database and i fetched it using SQL querries. A movie data erd was provided which was helpful to determine the relationship among the tables.

## Analysis Objectives/Questions to be answered?
What type of data do I have for analysis?
I had mixed data for data analysis and i selected the most relevant data which were Information Movies Database where i selected the tables
movie basics, movie ratings, movie akas, directors and writers. I also used Box offic mojo gross, movie budgets, movie information and movie reviews datasets. 
How was this data selected and why is it important to answer the above business problem?
Data was selected from various sites as listed in line 15 to 19. These sites store important information about the movie industry across the globe and hence they were rich datasets. 
What type of movie genres are currently existing in the market?
There are many types of movie genres but this study filtered the top 10 movie genres based on their Returns on investment. 
What is the cost of production of these movie genres?
The cost of production was measured relative to the ROI to give an objective performance metric that could be compared among different movies. This is because even though some movies were low budget movies,this didnt translate to high gross boxes. 
What are the features of these movie genres? Duration, Directors, Actors, Studios produced, etc?
These independent variables were ploted against the independent variable Return on Investment.
What are the movie box offices for these genres?
This was again measured relative to ROI
What are the net incomes of these movie genres?
What are the Returns on Investment for these movie genres?
What type of movie genres are most profitable?
Recommendations were made at the end on the best movies that Microsoft should consider for investment. 

### Independent variables

The dependent Variables
Averaging Rating
Genres
runtime in Minutes
Number of votes
Studio
Production budget
## Methods

I combined data from 5 different sources
● Generated new performance metric, Return on Investment as dependent variable
● I analyzed ROI against independent variables
● I generated various plots to examine how these independent variables vary with ROI
● I generated recommendations from the insights gained.



# Recommendations & Conclusion

1. Best performing Movies had a runtime of less than 80 minutes were bad performing. This means Short movies do not Perform best
Long movies with runtime of over 100 mins had low Return on investment. Therefore Microsoft should focus on producing a movie that has a runtime of between 80 Minutes and 100 minutes since this is the optimal runtime that produced best ROIs.
2. When it comes to genres, Horror, Mystery, Thriller Movies were best performing. Biography, Documentary also highly preferred. Crime, Drama, Family were least preferred among the top 10 genres i ranked based on ROI. Therefore, Microsoft should focus on producing Horror, Mystery, Thriller movies category.
3. Profitability. Most movies had a positive ROI meaning the industry is highly profitable. Among the more than 3000 movies analyzed, 65% of them had a positive ROI and hence this is an attractive industry for investment.
4. The Correlation coefficient between numvotes and averagerating was 0.5124943038145994. This means Average rating influences the number of votes. Therefore, Microsoft should ensure their movies are highly rated to attract more votes.
5. Movies produced in Croatian, Hebrew and French had the highest ROIs when ranked by Language
6. Movies with highest ROI were ones produced in Ukraine , Dominican Republic and Japan when ranked by region. Microsoft might need to take this into consideration. 
## Further Research
We can examine how  directors, writers, actors within a certain genre and budget affect Performance



