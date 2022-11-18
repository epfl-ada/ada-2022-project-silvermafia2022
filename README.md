# ada-2022-project-silvermafia2022
ada-2022-project-silvermafia2022 created by GitHub Classroom

## The role of women in the film industry - what is behind the prejudices?
### Abstract

In recent years, the US movie industry has often been criticised in the media for its lack of female representation. This lack of women representations has a large impact on our society, reinforcing the gender inequality of men doing great things (superhero, pilot, intelligent detective, scientist), and women being of secondary importance. As stated in (Bazzini et al., 1997): "Popular media images are reflections of a culture's attitudes, beliefs, and standards, as well as projections of desired realities [...] To the extent that consumers digest such material as truth, rather than fiction, the depictions laid forth by the media can be influential in the propagation and maintenance of stereotypes". 
This inequality will be explored through quantitative and qualitative analysis of movie data throughout various countries, genres, etc.

### Research questions
Part 1: Gender inequality in the movie industry  
1.1 What is the global trend of number of women and men cast in movies?  
1.2 What is the trend in the top 10 most movie-producing countries?  
1.3 What is the trend for different movie genres?  
1.4 For similar careers, do actors participate in more movies than actresses?  
1.5 What are the predictors of the share of women and men cast in a movie?

Part 2: Steoreotypes and representation of different genders in the movie industry  
2.1 What are the stereotypes according to the tv tropes?  
2.2 Which words are used to describe female and male characters?  
2.3 How did the representation of each gender evolve over time? 


### Datsets
The 5 datasets used are:

1. plot_summaries.txt
2. corenlp_plot_summaries.tar.gz
3. movie.metadata.tsv.gz
4. character.metadata.tsv.gz
5. tvtropes.clusters.txt

6. From dataset number 2, an additional dataset (summary.pkl) is created in a secondary Jupyter Notebook (summaries_treatment.ipynb). For each sentence of a summary, the words/lexic, is associated to the characters implied in the sentence. Thus, the dataframe contains each characters of each summary with their associated words. (WORK IN PROGRESS)
7. An additional dataset is also retrieved from Wikidata using 'sparqlwrapper' in Python. It corresponds to the freebase ethnicity ID and it's corresponding ethnicity.  


### Methods

Part 1: The goal is to look at the evolution of the number of women in movies. This will be done under two different angles: countries and movie genres.
In order to compare the participation of women and men in movies, we look at the female share index, defined as: 
$$\frac{nb\ of\ women}{nb\ of\ men\ +nb\ of\ women}$$ 
This is computed for all movies (Q1.1), years (Q1.1), countries (Q1.2), and movie genres (Q1.3). 


T-tests will be performed (Q1.1-Q1.3) across different periods (t.b.d), to assess whether there is significant statistical differences in women participation over time.

For Q1.4, perform a matched observational study, matching an actor and actress with similar features (age at first/last movie, carrier length, etc.). A dataset for control will contain only men, and treatment, only women. The output is the number of movies done during the entire carrer.   

For Q1.5, identify if there are predictors for female share in a given movie, such as movie genre, box office revenue, runtime, country, etc. This will be done using a regression analysis.

Part2: In contrast to part 1, we analyze the difference of the role of female and male characters in terms of how they are represented. Thus, we are interested in how characters of different genders are described and what words are associated with them.

For Q2.1, the tv tropes dataset (number 5) is used, which contains 72 character types along with 501 instances. The sex is attributed to each TV trope depending on the sex of the actor who played this role. By analyzing what words are used for TV tropes that describe female and male characters respectively, we will create word clouds which show the most abundant words for each gender. Furthermore, the librabry Empath is used to categorize the words into lexical fields. Consequently, we can compare the two gender groups because they are now classified by the same categories. For example, pearson’s correlation coefficient gives the strength of the linear relation between the two variables.

For Q2.2 and Q2.3, we make use of the newly created dataset 6, which conains all words associated with a figure from the summary of the movies. For Q2.2, we will use the approach described for Q2.1 but this time with the more exhaustive dataset. The same methodology is also applied for Q2.3, but in addition, the words for every gender is divided into three to four time periods depending on the release date of the movie. This allows us to observe the change in lexical categories over time for both female and male characters. For this subquestion however, we will go a step further and make a principle compnent analysis (PCA) using the categories created by Empath. By visualizing our different groups (male/female + different time periods) we expect to find a separation between the words of male and female characters. Furthermore, our expectation is to see more variation of the lexical field of female characters between different periods than for male characters.  


### Proposed timeline
W7-W9 (Oct 28-Nov 18):  
-Define project scope 
-Datasets cleaning, initial analysis and handling   
-Write the README
-Have all main dataframes needed for the analysis  

W12 (Dec 2-Dec 8):  
-Start analyses with the defined methods  
-Share results within the group  
-Critical review of approach/results  

W13 (Dec 9-Dec 16):  
-Re-do analysis if necessary (based on critical review)  
-Create most important graphs for the datastory  
-Outline for datastory  

W14 (Dec 17-Dec 23):  
-Datastory  
-Last modifications: is the code well explained? Representation of datastory  


### Organization within the team
Balthazar and Lara: handling of dataset 3/4, research questions, methods definition, creation of necessary dataframes for the analysis and datastory (all for part 1)  
Mathias: part 2 (extraction of all words associated to a movie character and creation of dataset 6), datastory part 2  
Romana: part 2 (analysis of the words, representation in word clouds/Empath categories/PCA), handling of dataset 5 + datastory part2  

Moreover, we have done several weekly meetings with all the group members, to decide what analysis to perform and methods to use for both parts 1 and 2. The above organization describes the "hands-on" tasks that were performed by whom.

### References
Bazzini, D. G., McIntosh, W. D., Smith, S. M., Cook, S., & Harris, C. (1997). The aging woman in popular film: Underrepresented, unattractive, unfriendly, and unintelligent. Sex Roles, 36(7–8), 531–543. https://doi.org/10.1007/BF02766689


