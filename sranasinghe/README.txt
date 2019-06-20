-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Model for Predicting Value of Future NBA draft classes

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Introduction:

With each new NBA draft class, a huge challenge for management is determining who will be their best pick for their draft slot. Getting ideal picks will help immensely,
as these new picks could be potentially the new faces of your franchise, and even if they are not, getting picks with high potential will have more market value,
enabling you to trade for more valuable resources. Because optimization of draft picks can have such a high payoff, we generated a model that will predict how well
a draft pick will do in the NBA, based on their college statistics.


Proposal:


To do this, we will utilize data from the NCAA and from the NBA. Using the full datasets for NCAA and NBA from the past 7 years, we will analyze specifically the players
who had been drafted within those years. In basketball, the primary statistics that are orthogonal from each other are points, rebounds, assists, steals, and blocks (on a per minute basis).
Each of these stats are gained through distinctly different methods during the game, and because of that there is no reason to assume causation between these values. 
I will split rebounds between offensive and defensive, instead of points, split between 2 point field goals, 3 point field goals, and free throws, as well as account
for some negative variables, including missed shots, fouls, and turnovers. While this is all of the data that we are pulling, as we refine our model we might simplify
it depending on the outcome.

Now in order to assess how well a player will do in the NBA, there has to be a metric which can be used to assess performance. Although there are many known metrics that
are out there, my metric of choice is PER. The reasoning behind this is because this metric is calculated using all of the variables which I outlined, and using these
variables we can create a linear regression model which will predict the NBA PER of a player using the college statistics, and based on the PER we can determine how 
valuable the future players will be.
