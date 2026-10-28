# Student Rent Predictor

## Summary
An AI tool that predicts the monthly rent of a student apartment from its features, such as size, distance to the university, and number of rooms. It helps students check whether an offered price is fair.

## Background
Students often rent apartments in a hurry and don't know the typical price in a city. Overpriced listings are common. A simple price estimate helps students negotiate and avoid overpaying.

## How is it used?
The student enters the details of an apartment: size in m², number of rooms, distance to the university in km, and distance to public transport. The tool returns a predicted monthly rent. If the listed price is much higher than the prediction, the student can negotiate or keep looking. It would be used mostly when searching for a new apartment.

## Data sources and AI methods
The data would be collected from public rental listings, with each apartment described by its features and its actual rent. The method is linear regression: the predicted price is a weighted sum of the features, and the weights are fitted by minimizing the squared error between predicted and actual prices. The model would be tested on apartments that were not used for training.

## Challenges
The model only works well for the city and time period of the training data. Prices depend on things that are hard to measure, such as the condition of the apartment or the landlord. A linear model can't capture every nonlinear effect, and the tool should never be the only basis for a decision.

## What next?
Add more features such as floor, furnishing and neighborhood, try other methods such as nearest neighbors, and expand the data to more cities.

## Acknowledgments
Inspired by the linear regression exercises in the Building AI course by Reaktor and the University of Helsinki.# student-rent-predictor
