# Question and Need
For this project I'll be building a model to predict a movie's lifetime gross earnings which in turn will help investors decide whether or not they should invest in a movie.

Investors would find this model useful because ultimately they want to invest in movies that are predicted to have high lifetime gross earnings since that will generate more returns on their initial investment.
# Data Description
I plan to use movie data from Box Office Mojo and scrape 1000 movies ranked by their top lifetime grosses.

The data from Box Office Mojo will be retrieved using Python packages built for webscraping such a Beautiful Soup and Selenium.

Features for each movie that I expect to work with include:
* movie title
* lifetime gross earnings
* lifetime gross earnings rank
* release year
* release date
* release season (eg. fall, winter, spring, summer)
* distributor
* budget
* MPAA rating
* running time
* genre

The target that I want to predict using my model is a movie's lifetime gross earnings.

I expect to be working with majority text data along with some numerical data sprinkled in.

# Tools
Depending on the stage of the workflow that I'm in, I'll be utilizing several Python packages.
## Webscraping
* Beautiful Soup
* Selenium
## Data Cleaning, Exploring and Manipulation
* Pandas
* NumPy
## Statistical Analysis
* scikit-learn
## Data Visualization
* Matplotlib
* Seaborn

# MVP Goal
My MVP for this project would be to generate pair plots to display the relationship between several different variables and a movie's lifetime gross earnings.
