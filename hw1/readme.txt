CSE 512 Assignment 1
Evan Komp

The dataset contains 5 relevaant columns: latitude, longitude, city, sunshine, and month. The sunshine column is a clear measurable of the dataset, while the other columns are independant variables. Latitude and longitude constitute one variable, the quantitative geographic location, while city encodes these locations nominally. Month is an ordinal time unit, and so sunshine is measured during a given month in one of the locations. 

Given that there are two independant variables (location, time) and one dependant variables, we need to think to aggregate across one of them somehow. Given that the location is both geographically and nominally encoded, we have some flexibility.

I choose to ask the questions:

1. "How does the sunshine experienced in a city differ by geographic location?"
2. "How does sunshine experienced in different cities differ over the year?"

I hypothesize for Q1 that cities at higher latitudes will have overall less sunshine, while for Q2 that all cities will have peaks in Summer (given that all cities are northern hemisphere) but further north will lead to more drastic variances.

To answer Q1 I aggregate over the months of the year to produce average monthy hours of sunshine and plot these as bubble size on a geographic map of the US. Colors correspond to the city. Color is not inherantly beneficial for this first plot but is useful when viewing both plots together, as it allows for the two plots to be easilly connected by the viewer. We can see that the hypothesis was generally correct, the most south city (Miami) has close to the most average sunshine, with California as the most by 1.5%. The most north city (Seattle) indeed has the least *cries a little*. Most suprising was that the averages were less varied, such that bubble size is difficult to distniguish. For this reason I marked the value of the average sunshine as text. 

To answer Q2 I plotted mothly sunshine as lines accross months. One might argue that bars would be better as months are technically orndinal, but we as humans see months as a continuous time spectrum, and given that I chose to play all cities in the same plot, so many bars may be cluttered. I utilized colors to distinguish between cities, importantly the same colors as on the first map plot for easy reference. Indeed each city has a peak in summer, and it is less drastic for more south cities.