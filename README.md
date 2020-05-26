# MovieRating
<h3>Summary of Project</h3>

For our project we would like to create a model that predicts the success rate of a box office movie such as a fail, hit, or superhit. The premise of this project stemmed from answering the question of whether we could predict the success of the movie only knowing data about a movie prior to  release.<br>

While answering this question, a few question we first asked ourselves were:
* What parameters best predict the success rate of the movie (genre, director, budget, etc.)?
* Which cast or actor best predict the movies?
* Can we look at the genre of the movie to help classify?
* Does the time the movie is released throughout the year influence how the movie does?

<h3>Plan of Action</h3>
Use the movie data from The Movie DB which has data on over 5000 movies
The data that is found in this database include:
Budget
List of film genres
Release date
Cast members
Crew members
Keywords about the movie
Released during time of year
Problems?
columns store lists inside of them so we will need to make a library to sort through these lists or multiple tables
movies have a large cast and crew so we will have to take some time to sort through what cast and crew members are important to use
decide how many movies to train our model on and how many predict on

<h3>Machine Learning</h3>
When implementing Machine Learning into our project, we had to re-clean and restructure our data
We the introduced a “grade scale” to rate out movies. The following is the scale:
0-3 VA* → 1 = bad, 3-5 VA* → 2 = okay, 5-7 VA* → 3 = good, 7-10 VA* → 4 = excellent
These would be used as buckets
We then used Feature Selection to test our model using K-Nearest-Neighbors (KNN)
After plotting the relationship between K and testing accuracy, we used this to choose our K-value→ 8. This was the optimal value of K so that we would not overfit the model
