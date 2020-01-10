# The Effect of Income Disparity on Bank Customer Complaints

## Context:
When it comes to money, everyone has a love-hate relationship. People love it when they get their
first paycheck, but once they begin to run out, they hate the concept of relying on a piece of paper
to acquire their needs. Instead of looking within themselves, they turn to outside factors, such as
their banks, to blame their problems on. Don’t get me wrong, banks are far from perfect. They
make mistakes that need to be pointed out because they have a plethora of customers to handle.
Due to this logic, banks receive numerous consumer complaints about various financial issues in
hopes that the corresponding bank can solve them.

## Problem: 
We investigate if there is there is a certain cause behind customer complaints besides the
issue stated with their bank. Out of all the probable causes, we wanted to examine if there is
correlation between income disparity and the number of bank complaints. Since feelings are deeply
intertwined with complaining, we wanted to utilize an objective variable that could aid us in
discovering a variable that deeply influences the actions of bank customers.

## Analysis:
We wish to combine two datasets to investigate into this problem. One dataset purely states the
customer complaints in 2012-2019 from Consumer Financial Protection Bureau and contains
metadata regarding the location, date and product name. In the other dataset, U.S. Environmental
Protection Agency describes the total household income levels nationwide by county. By converting
county names into zip codes (the library “sp” in R contains this functionality), we merge those two
datasets over zip code and date to account for inflation.
To visualize the relationship, we will use “ggmap” to color code the nation by the income levels and
overlay the number of complaints in each zip code or state, depending on which method is better.
However, correlation does not mean causation – conducting statistical tests such as t-tests and
regression methods will depict if there’s a relationship between the two variables. Furthermore,
machine learning techniques such as PCA and SVM will allow us to classify the complaints and
predict if a certain area will file more complaints in the future. 
