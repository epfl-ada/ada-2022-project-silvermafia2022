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

From dataset number 2, an additional dataset is created in the Jupyter Notebook "BLABLA" (matthias).
Apart from those, there are no additional datasets.

### Methods

Part 1: The goal is to look at the evolution of the number of women in movies. This will be done under two different angles: countries and movie genres.
In order to compare the participation of women and men in movies, we look at the female share index, which defined as: 
$$\frac{nb\ of\ women}{nb\ of\ men\ + nb\ of\ women}$$ 
This is computed for all movies (Q1.1), years (Q1.1), countries (Q1.2), and movie genres (Q1.3). 
We look at the female share index rather than the absolute number of women because, as we are interested in the presence of actresses compared to actors.
In this way, we can deal with the fact that the absolute number of actors and actresses both have increased over time, due to an increasing number of films produced per year.

T-tests will be performed (Q1.1-Q1.3) across different periods (to be defined), to assess whether there is significant statistical differences in women participation over time.



### Proposed timeline


### Organization within the team
