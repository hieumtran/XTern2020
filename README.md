# XTern2020

![](ScatterPlot/Average%20Cooking%20Time.png)

## I) Overview
The XTern2020 dataset is a very interesting dataset. It has a lot of variables, such as ratings or average cost, to analyze the data and has many missing data. After analyzing the XTern2020 dataset, I draw 4 conclusions: 
  1) The longitude and latitude does not have affect on the rating, votes, reviews, average cost, minimum order, or cooking time. 
  2) Many people will tend to use the delivery system with different types of cuisines.
  3) The most trending delievery system is the one with 7 different cuisines.
  4) The optimized average cooking time is 40 minutes.

## II) Conclusion 1:
When I first comes to the data, I see that the data has a variety of different longitude and latitude. So I ask myself that can a particular zone be favored more than other zones? Therefore, I use Flourish ( an online data visualization which has similar mechanics to Tableau) to graph the longitude and latitude combining with other variables. 

![](ScatterPlot/Rating%20(%20Latitude%20and%20Longitude).png)
![](ScatterPlot/Votes%20(%20Longitude%20and%20Latitude).png)
![](ScatterPlot/Reviews%20(%20Longitude%20and%20Latitude).png)
![](ScatterPlot/Average%20Cost%20(%20Longitude%20and%20Latitude).png)
![](ScatterPlot/Minimum%20Order%20(%20Latitude%20and%20Longitude).png)
![](ScatterPlot/Average%20Cost%20(%20Longitude%20and%20Latitude).png)

Note: From the top to the bottom: rating, votes, reviews, average cost, minimum order, and cooking time

However, from all the scatterplots above, I could not see any relationships between the location and other factors.Therefore, I draw a hypothesis conclusion that the location from this data has no affect to the rating, votes, reviews, average cost, minimum order, or cooking time.

 Also, one aspect I notice in the scatter plot 2 and scatter plot 3 is that they are not really different much. Maybe, their correlation is really close to 1.

## III) Conclusion 2:
Leaving the longitude and latitude behind, I find the Cuisines variable very interesting. It has a lot of unique values and has different combinations. So, I create dummy variable "Count_Cuisines" to calculate the different types of cuisines a delivery system has in each delivery system. Then, I create a pivot table with the Count_Cuisines as the index and average of ratings, votes, and reviews to see how do people think about the different delivery system.

![](ScatterPlot/Reviews%20and%20Cost.png)
![](ScatterPlot/Average%20Rating.png)

The first scatter plot shows the relationship of the average of votes and average of reviews. In the graph, the votes dots and the reviews dots are really close to each other. Therefore, I calculate the correlation of the votes and the reviews. The result is 0.9644514962195193. It is really close to one. Therefore, their relation ship are really close to perfectly linear. In other words, they are highly related to each other and do not different from each other a lot. I can use votes to predict reviews and vice versa if either of them is hidden. Therefore, I choose to use the average of votes.

On the right hands, the scatter plot of the average ratings is very interesting. Similar to the scatter plot on the left, the 
