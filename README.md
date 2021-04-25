# Data-115-Personal-Project

# Motivation 
With the world reaching almost 8 Billion people soon, I wanted to ask what would the 8 billion and 1st baby be named? This led me to search for answers in the area of what names are the most popular from the Gender by name dataset from UCI https://archive.ics.uci.edu/ml/datasets/Gender+by+Name. This data set is a culmination of 4 datasets of names from the United States, United Kingdom, Canada, and Austrailia. I would like to mention that since the dataset only includes 4 countries, this dataset will most liukely not be representative of all of the worlds people but will give us a good idea of the popularity of names in english speaking countries.

# Data
This dataset combines the raw count of first names of male and female babies through those time periods.
-US: 1880 to 2019
-UK: 2011 to 2018
-Canada: 1918 to 2018
-Australia: 1944 to 2019

-US: https://catalog.data.gov/dataset/baby-names-from-social-security-card-applications-national-level-data 

-UK: https://www.ons.gov.uk/peoplepopulationandcommunity/birthsdeathsandmarriages/livebirths/bulletins/babynamesenglandandwales/previousReleases 

-Canada: https://www2.gov.bc.ca/gov/content/life-events/statistics-reports/bc-s-most-popular-baby-names 

-Australia: https://data.gov.au/dataset/ds-sa-9849aa7f-e316-426e-8ab5-74658a62c7e6/details?q= 



The dataset came with 4 columns of information. 
1. Name, the name that is in question (string).
2. Gender, (M/F) (string)
3. Count, the number of people with the name (integer). 
4. probability, the percentage of people with the name compared to every other name (float).

# Processsing
First of all, since the data did not come with any years or any timeframes of each name, I could not omit any of the data based on the year the person was born in. I would have liked the data to be representative of the current time period. The raw data set contained about 15,000 entries, many with just one name. I first took the data frame and split it into two by seperating male and female entries. Since there were so many names per letter, I decided to combine the counts of each letter. I took the first letter of each name and then summed up the counts. I also went back to the initial dataset to get the total summations of each letter. This is where the count by letter csv files came from. I then also counted the number of names by letter in the total dataset and created a new dataframe that masured the variation of each name per letter. I realized that I should also combine the count and variation datasets to compare them for later. 

# Visualization
Since the dataset was ordered by number of people having a certain name, we could see from just using head(df) that James had the most popular name. with over 5.3 million people. 

# Analysis

# Final thoughts
