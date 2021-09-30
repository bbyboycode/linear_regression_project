# Predicting A Movie's Lifetime Gross Earnings
Stanley Guo
## Abstract
The goal of this project was to use data about movies and put together a viable linear regression model to predict a movie's future lifetime gross earnings. I worked with data scraped from boxofficemojo.com. I scraped the top 1000 movies ranked by lifetime gross earning from each MPAA rating, spanning from NC-17, all the way down to G. After, I performed data wrangling and data cleaning in order to have useable data in my regression model.
## Design
This project was designed with the goal that it can be used by investors who want to generate returns on their money by investing in the entertainment industry and more specifically, movies.
## Data
The dataset scraped from Box Office Mojo originally consisted of 3374 movies, with each row representing an individual movie. Columsn consisted of features such as MPAA rating, run time, genere(s), and domestic distributors. I had a total of twelve columns. As I progressed throughout the project I added a couple of rows such as run time in minutes format instead of the original hour and minute, I also added a release season column which, depending on the month that the movie was released, classified movied as a summer, fall, winter or spring releases.
## Algorithims
Some of the data that I scraped to use for the project was categorical and not numberical which meant that I had to create dummy varibles in their places. I did this for genres, and release season and domestic distributors.

After my data cleaning and wrangling to prep the data to be used, I ran a simple linear regression model using domestic opening (how much a movie made on its opening day) and run_time as my independent variables and used lifetime gross earnings as my target variable.

I then wanted to see if I could improve the R^2 score that I got from my base linear model by using feature engineering and added generes as another variable in the model.

I repeated this feature engineering method further by adding variables such as release season and a movie's domestic distributor to see how much more I would be able to increase my R^2 score without modifying it too much to that point that it would overfit my training data.
### Tools
* Beautiful Soup for web scraping
* Pandas and Numpy for data manipulation, cleaning and wrangling
* Matplotlib and Seaborn for data visualization
* scikit-learn for modeling
# Communication
I found that domestic opening was the biggest factor when predicitng a movie's lifetime gross earnings. When conducting feature engineering, I was not able to improve my R^2 score that significantly, often times the R^2 score would only improve by .1%.
