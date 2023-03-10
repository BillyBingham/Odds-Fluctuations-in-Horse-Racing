# Odds-Fluctuations-in-Horse-Racing
Using Odds Fluctuations in Australian Horse Racing to predict a winner

Using sportsbet.com.au, information relating to 820 individual Australian horse races has been collected. 
Statistics collected include; race winner, location of race (town/suburb), location of race (State), race number, opening price (odds when the race was initially put online – approximately 3 days prior to race start), starting price (odds when the race starts), percentage of odds fluctuation between opening price and starting price, whether the winning horse was the biggest or second biggest fluctuation in the race, whether the winning horse was the favourite at the start of the race, jockey name, trainer name, and ground type.
A full Data Dictionary is included in the word document. 
14 of the 820 races had no information post-race relating to the opening price. 
These observations have been deleted from the dataset as they would not be useful for the analysis as it was not possible to tell whether or not they would fall within the biggest fluctuations or not. 
In total, 806 individual races had full data available, and thus is the final dataset that has been used for this analysis. 
This analysis will look at the viability of looking at the odds fluctuations of winning horses to be able to predict future winners, and whether or not this is more or less likely at a specific location. 
This has been done using the data above and analysing it in Tableau, as well as using a logistical regression model in python. 
Of the three success metrics chosen for the hypothesis, one of these three was met – to have an overall average odds fluctuation of 10%+ across all races (10.85%). 
A hit rate of 40%+ winning horses being in the top 2 fluctuations of its race was missed (36.5%), whilst a total of 70%+ of winning horse’s odds reducing between opening price and starting price was also missed (66.63%). 
Digging deeper into separate locations did find some results where all three success metrics were met. 
The logistic model that has been created, along with cross-validation against the dataset, could correctly identify with 80% (+/- 5%) accuracy, whether the horse was likely to be in the top 2 biggest fluctuations of its race. 

