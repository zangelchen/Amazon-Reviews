# Amazon Reviews

## Digital vs Vinyl/CD sales & top ranked brands in the industry!

*Collaborators: Angel Chen, Amr Ismail, Roger Zatarain, & Drew Barnhart*

# Background

We developed a code using JSON files extracted from Amazon Reviews. Our aspirration was to examine categories within the Music Genre and create analysis based on the reviews provided. Our Data gave multiple categories to choose from and allowed us to compare and contrast manageable and easily accessible data source for example: CD & Vinyls and Digital music.

Link from where data was derived: https://nijianmo.github.io/amazon/index.html

# Objective

Determine the total sale and average rating for each artist to derive potential correlations between the two data points to inform future stakeholders whether the higher rating guarentees higher sales. Our goals was to provide better understanding of customer opinions, preferences, and top genres to help: Music consumers, producers, & musicians. 

# Research Questions
What is the distribution of digital music vs physical music and does that provide any indication on the quality of the data?

How does the distribution of digital music vs physical music overall rating compare with each other?

What are the top 20 most popular songs? 

Does popular music mean higher rated reviews? 

# Part I  
1. Original raw data was provided in a raw JSON format that was visually difficult to decipher. Our initial task was to read it into our Jupyter Notebook and then create a data frame that provided more accessible depiction of the data. 
2. initially we Extracted JSON Digital Music, Meta Digital Music, CD, & Meta CD
3. Created a For Loop to Read JSON
4. Merged Digital Muisc and Meta Digital Music 
5. Merged CD and MetaCD
6. Finally, we created a DataFrame groupby ASIN (Product ID specific to Amazon)

# Part 2
We begin a two pronged strategy for anlyzing 2 seperate categories:

A. Comparative analyis of digital music vs that of CD/Vinyl 

B. Compared the total sales vs average ranking and found top 20 ranked/selling artists/bands
  
# A: Digital Music vs CD/Vinyl 

##### Graph 1

![image](https://user-images.githubusercontent.com/116226080/215923525-25d6abf5-c233-4287-8375-39970359c116.png)
We created a graph from our merged DataFrame to establish a count of total count of ratings compared to actual rating (1-5)
Within this graph we integrated the distribution to show the spread independent to each rating as well. We found that majority of the reviews given were generally positive 4 & 5's while lower rankings were a minority.

We then counted the cummulative ratings of Digital Music and Vinyl/CDs and depicted them via Pie Charts 

#### Digital Music Overall
![image](https://user-images.githubusercontent.com/116226080/215924754-e16b139d-ce5c-4a5a-bfcf-22ba9151f7c9.png)

![image](https://user-images.githubusercontent.com/116226080/215924855-0b4312d0-3a12-466b-a4cb-da4cee7747ed.png)

Its interesting to note that there were more 5’s in CD & Vinyl (65% vs 55%), But less 4’s & 3’s compared to Digital Music. However the median ranking between either of them was comparable. This observation was further re enforced by the box & whisker plot we developed. 

![image](https://user-images.githubusercontent.com/116226080/215932277-a85328f0-5a0e-4734-bf34-2d7329a1c12b.png)
The Box & Whisker plot below shows how comparable these means and findings from Quartile calculations. With nearly identical ranges!

The graph below depicts the number of reviews given to an album vs. Avg Rating in the digital music dataset. 

![image](https://user-images.githubusercontent.com/116226080/215932600-73afaa5f-4a98-4cec-be7d-a149e2ade3df.png)

Finding: When plotted the graph shows a very weak negative correlation between these two variables. The ranking did relate to the review count, with higher rankings tending to have more cummulative reviews. We initially suspected that more prople would leave a review when disatisfied with the product. But the result was the opposite. Potentially our initial assumption would be true for other genre like Food, Toys, etc. 

# B: Total Sales, Highest Ranking, Top 20 & Comparative Analysis

Worked off of both Digital Music and CD & Vinyl


<img width="384" alt="Screenshot_20230130_083524" src="https://user-images.githubusercontent.com/116226080/215922333-02a45caa-df60-45f1-869e-b7fc8345fc95.png">


<img width="483" alt="Screenshot_20230130_080802" src="https://user-images.githubusercontent.com/116226080/215922541-dca94816-028b-40b9-b78c-c772dd063644.png">


<img width="515" alt="Screenshot_20230130_083228" src="https://user-images.githubusercontent.com/116226080/215922364-e9c8c131-b932-4546-83e2-4012f04c0371.png">


<img width="459" alt="Screenshot_20230130_080306" src="https://user-images.githubusercontent.com/116226080/215922577-324cdd31-299e-45e3-affc-7585a1734381.png">


Findings: There is a very week positive correlation between Total Sales and Average Ratings. While the highest sales did have high ratings, there are also artists that had high ratings but few reviews. 

Software Used:
- Python

Functions used: 
- Groupby
- Creating dataframe
- Sort_Value
- Ascending
- Plt.Scatter
- Plt.Bar
- Plt.Pie


RAW DATA VISUALIZATION
<img width="891" alt="Screenshot_20230130_100030" src="https://user-images.githubusercontent.com/116226080/215921369-b51ea6a0-edc8-4f8b-ba4c-59bd3ffb3892.png">

EXAMPLE OF ONE DATA FRAME CREATED
<img width="1015" alt="Screenshot_20230130_085613" src="https://user-images.githubusercontent.com/116226080/215922213-5777a3eb-c6be-4bf5-8502-716abcd00ca9.png">
