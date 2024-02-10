# CSE151A_UrbanAnimals
Unveiling patterns: predictive modeling of animal disposition in urban settings

Project Goal:
Our goal for our project is to take the data collected from animal control calls, and to be able to determine how many animal controllers should be sent to the location. We also  wanted to take various information and graphs and see what we might find if we noticed anything that we may not have expected. We are taking the data and using incident dates , breed, sex, location, size, etc, to determine the possible temperament of an animal. There are numerous factors that can contribute to an animal being more docile or hostile, whether its mating season, spring/winter, animal type, breed, age, sex, if its injured, etc. Using all this information we should be able to predict if an animal control request is going to impose any danger on the caller or responders, or how high of a priority a call is.


Pre processing data:
We wanted to select all the relevant columns of our data. But there were many values that had NA or unknown.
We took every value that was unknown, replaced it with NaN, and dropped it from our table.

We used a histogram to plot "species", "breed", "sex", "size", "condition"
Noticing many different breeds, we wanted to clean it up so we created a consolidated breed table using some lambda functions to strip away characters so that we could group the correct breeds with each other.
For example, some values were 'XRetriever', or 'X Retriever', this is redundant. They are the same breed, we changed it so its simply 'Retriever'

We also wanted to take the more common breeds and to group them by type.
For example 'Cocker Spaniel' 'Springer Spaniel' is a type of 'spaniel', 'Rooster' is a type of 'Chicken'

Graphs:
Using our processed consolidated breed data, we wanted to do some more analysis
We did some histograms of species by species sex ,conditions, sizes.

We wanted to check which dogs were most commonly reported for incidents. We did a histogram and noticed the primary dog breed that was called was pitbull by a vast majority. Pitbulls were called in almost 4x more than the second dog breed "Labrador".

Also we checked the condition of the dogs.

