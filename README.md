# ada-2022-project-silvermafia2022
ada-2022-project-silvermafia2022 created by GitHub Classroom

## The role of women in the film industry - what is behind the prejudices?
### Abstract


### Research questions
Part 1: Gender inequality in the movie industry  
1.1 What is the global trend of number of women and men cast in movies?  
1.2. What is the trend in the top 10 most movie-producing countries?  
1.3. What is the trend for different movie genres?  
1.4. For similar careers (length, age), do male actors participate in more movies than women?  
1.5. What are the predictors that define the share of women and men cast in a movie? Movie genre, box office revenue, runtime, country, etc?

Part 2: Steoreotypes and representation of different genders in the movie industry  


### Datsets
There are 5 datasets used in this project (provided by the teaching staff):

1. plot_summaries.txt
2. corenlp_plot_summaries.tar.gz
3. movie.metadata.tsv.gz
4. character.metadata.tsv.gz
5. tvtropes.clusters.txt

From dataset number 2, an additional dataset is created in the Jupyter Notebook "BLABLA" (Mathias).
Apart from those, there are no additional datasets.

### Methods

Part 1: The goal is to look at the evolution of the number of women in movies. This will be done under two different angles: countries and movie genres.
In order to compare the participation of women and men in movies, we look at the female share index, which defined as: 
$$\frac{nb\ of\ women}{nb\ of\ men\ + nb\ of\ women}$$ 
This is computed for all movies (Q1.1), years (Q1.1), countries (Q1.2), and movie genres (Q1.3). 
We look at the female share index rather than the absolute number of women because, as we are interested in the presence of actresses compared to actors.
In this way, we can deal with the fact that the absolute number of actors and actresses both have increased over time, due to an increasing number of films produced per year.

T-tests will be performed (Q1.1-Q1.3) across different periods (to be defined), to assess whether there is significant statistical differences in women participation over time.

For Q1.4, we will perform a matched observational study, matching an actor and actress with similar features (age at first movie, age at last movie, carrier length, most frequent movie country, and most frequent movie genre if applicable). A dataset for treated will contain only men, and the non-treated will contain women. The output of the treatment is the number of movies done during the entire carrer.  

For Q1.5, we will identify if there are predictors for the female share in a given movie, such as movie genre, box office revenue, runtime, country, etc. This will be done using a regression analysis..

### Proposed timeline
W7-W9 (Oct 28 - Nov 18):  
- Define project scope: clearly define the project idea and what are the questions to be answered  
- Datasets cleaning, initial analysis and handling   
- Write the README: develop what is the story we want to tell with our data  
- Have all main necessary dataframes used for the analysis  

W12 (Dec 2 - Dec 8):  
- Start analyses with the defined methods  
- Share results within the group  
- Critical review of approach / results  

W13 (Dec 9 - Dec 16):  
- Re-do analysis if necessary (based on critical review)  
- Create most important graphs for the datastory  
- Outline for datastory  

W14 (Dec 17 - Dec 23):  
- Datastory  
- Last modifications: is the code well explained? Representation of datastory  


### Organization within the team
Balthazar: part 1 (research questions and methods definition, creation of necessary dataframes for the analysis), handling of dataset 3 + datastory part 1
Lara: part 1 (research questions and methods definition, creation of necessary dataframes for the analysis), handling of dataset 4 + datastory part 1
Mathias:
Romana:

Moreover, we have done several weekly meetings with all the group members, to decide what analysis to perform and methods to use for both parts 1 and 2. The above organization describes the "hands-on" tasks that were performed by whom.

