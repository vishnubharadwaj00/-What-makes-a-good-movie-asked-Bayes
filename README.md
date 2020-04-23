# What makes a good movie? asked Bayes
Bayes wanted to know whether he could predict the movie ratings. At least that's what he would have asked if he were alive today. So, on his behalf, his statistical methodologies are used in this project.

### The Data

Rotten Tomatoes and the TomatometerT rating is the most trusted measurement of quality entertainment. As the leading online aggregator of movie and TV show reviews from professional critics, Rotten Tomatoes offers the most comprehensive guide to what’s fresh. The world famous TomatometerT rating represents the percentage of positive professional reviews for films and TV shows and is used by millions every day, to help with their entertainment viewing decisions. Rotten Tomatoes designates the best reviewed movies and TV shows as Certified Fresh. That accolade is awarded with Tomatometer ratings of 75% and higher, and a required minimum number of reviews. Weekly Rotten Tomatoes podcasts can be found on RottenTomatoes.com, iTunes, Soundcloud and Stitcher, and Rotten Tomatoes’ entertainment experts make regular TV and radio appearances across the US.

**Data Collection**

*Generalizability*

The present data were derived from an observational study. The data set is comprised of 651 randomly sampled movies produced and released from 1970 to 2014. According to IMDb, there have 9,962 movies been release from 1972 to 2016 so that the 10% condition (9,962*0.01 = 996) is met. Since the sampling size is large enough and less than 10% of population, it can assume that the random sampling is conducted. Therefore we can conclude that the sample is indeed generalizable to the entire population.

*Causality* 
The data cannot be used to establish a causal relation between the variables of interest as there was no random assignment to the explanatory and independent variables.

### Programming Environment

All programming was done with R, using the RStudio IDE. The full code can be found in the Rmd file. 

## Conclusion

The predictive model presented here is used to predict the audience scores for a movie. Using Bayesian model averaging and many factors like BIC, ZSC, AIC, etc, many models can be constructed to perform better predictions.

The proposed linear model shows a ‘fairly good’ prediction rate, **(around 85%)** but it should be noted that the model is based on a very small sample. The fact is that imdb_rating has the highest posterior probability, and that basically all of the newly created features were not that useful to support a better prediction. Creating a model, which has a high predictive power is not so easy to reach. Using Bayes for better prediction is only one part of the game. It might be beneficial to gather more data or try to extend the feature engineering part, which means to creating new meaningful features from existing or gather data for new features.

Perhaps in a future project, for higher accuracy, we could have included all the remaining factors as well, and then eliminated them one by one. Even though such models might be prone to overfitting or underfitting, these problems can certainly be mitigated using expert opinion on which factors are actually useful.

