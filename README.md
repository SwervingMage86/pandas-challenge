# pandas-challenge

# Heros of Pymoli

# Reason of Choice

I chose this problem because it is breaking down what clients are buying and how much money they are spending.
I felt that this was more relatable to what I eventually want to be doing with data analytics, and felt it would be good practice.

# Step One : Player Count

Finding total players is a fairly easy task. Find the column name, break it down to unique names, and count the number of names.
Then build the result into a dataframe.

# Step Two : Purchasing Analysis (Total)

I counted the number of unique items the same as I did unique player names.
I found the total revenue by adding up the values of the 'price' column.
I then found average price by dividing the revenue I just calculated by the number of values in that column.
I then used the 'purchase id' column to find the total number of purchases.

I then built all these values into a dataframe and cleaned it up.

# Step Three: Gender Demographics

I started this table by sorting to all males by using the loc function to filter down the 'gender' column.
I then used this filtered dataframe to count the unique players, and used that value by the total number of players found earlier to get the percentage of male players.

I repeated this process to find the same values for both female and non-disclosed players.
I then built all the values into a cleaned dataframe.

# Step Four: Purchasing Analysis (Gender)

This step was basically a combination of steps two and three, was more typing and copy/paste then anything else.

# Step Five: Age Demographics

I created bins and bin names to add a new column to the original dataframe that showed which age group each user fell under.
Then it got really frustrating for me, as I ended up filtering each age group and counting each unique user. The same way I found gender counts.
While this worked, it was a lot to type out and I spent a lot of time trying to find a cleaner way to make this calculation, but couldn't come up with anything.

After finding the count of each individual group, I added all these values to a list, then divided this list by the total number of players to get my percentages.
I then built the list of group counts and the percentage lists into a data frame, setting my index as the bin names.
I cleaned it up and it was what I wanted, however painstaking.

# Step Six: Purchasing Anaylsis (Age)

For this step I grouped by the 'age group' column I created and then performed the same functions as I did in the previous purchase analysis steps.
I built the values into a dataframe and cleaned it up.

# Step Seven: Top Spenders

For this step i grouped the original dataframe by user ID, then basically did the same steps as previous purchase analysis steps.
The exception on this step is I sorted the 'total purchase value' column in the final dataframe in descending order to show the highest values on top.
I then cleaned it up and only printed the first five rows.

# Step Eight: Most Popular Items

I created a new dataframe from the original only using the 'item id', 'item name' and 'price' columns for less values to look at.
I then grouped by both 'item id' and 'item name' to pull the unique values
I then performed basic functions to find the values I was looking for and built it into a dataframe.
I sorted the 'purchase count' column, again in descending order.
I then cleaned it up and printed the first five rows.

# Step Nine: Most Profitable Items

I used the same table I created in the previous step, I just sorted it by the 'total purchase value' column instead, by descending order.
One note is I had to run the previous step with the format lines hashtagged out as it turns the float values into strings and won't sort correctly.
So after I ran this cleaned up cell, I had to go back and re-insert my format lines into the previous cells and run it again to get my cleaned up dataframe.

# Observations

While there are many trends that are evident in after sorting through the data, I will point out the two that stand out most to me.

The first is that this game is very obviously geared toward the male population, as they make up nearly 85% of the user population and nearly the same amount of the revenue.
The second is age group seems to be fairly normally distributed, with the height of the curve being 20-24 year-olds at 50% of the population and then evenly spread out either way.


