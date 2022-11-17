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
2.1 Stereotypes 
2.2 Which words are used to describe female and male characters?
2.3 How did the representation of each gender evolve over time?


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

Part2: In contrast to part 1, we analyze the difference of the role of female and male characters in terms of how they are represented. Thus, we are interested in how characters of different genders are described and what words are associated with them. Will the clichés come true?

For Q2.1, the tv tropes dataset (number 5) is used. Typical character types are identified from .... The sexe is attributed to each trope depending on the sexe of the actor who played this role. By analyzing what words are used for tropes that describe female and male characters respectively, we will create word clouds which show the most abundant words for each sex. This directly shows the most used words for describing a role of each gender. Furthermore, Empath is used to categorize the words into lexical fields. Consequently, we can compare the two because they are now classified by the same categories. For example, pearson’s correlation coefficient gives the strength of the linear relation between the two variables.

For Q2.2 and Q2.3, we make use of the newly created dataset 7, which conains all words associated with a figure from the summary of the movies (dataset 2). For Q2.2, we will use the same approach as describes for Q2.1 but this time with this new and much larger dataset 7. This allows us to examine, if the representation of genders in the tv tropes correspond to the representation of characters in the summaries of the movies. The same methodology is also applied for Q2.3, but in addition, the words for every gender is divided into three to four time periods depending on the release of the movie. This allows us to observe the change in lexical fields over time for both female and male characters. For this subquestion however, we will go a step further and make a principle compnent analysis (PCA) with the classes created by Empath. By visualizing our different groups (male/female + different periods) we expect to find a separation between the words of male and female characters. Furthermore, our expectation is to see more variation of the lexical field of female characters between different periods than for male characters.


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

