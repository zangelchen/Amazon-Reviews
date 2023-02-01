# Amazon Review Analysis
## Digital vs Vinyl/CD sales & top ranked branked brands in the industtry!

Collaborators: Angel Chen, Amr Ismail, Roger Zatarain, Drew Barnhart, & Cesar Ruiz

# Background

We developed a code to using JSON files extracted from Amazon Reviews API. Our aspirration was to examine categories within the Music Genre and create analysis based on the reviews provided. Our Data gave multiple categories to choose from and allowed us to compare and contrast manageable and easily accessible data source for example: CD & Vinyls and Digital music.Our goals was to provide better understanding of customer opinions, preferences, and top genres to help our audience: Music customers, producers, & musicians. 

Software Used: Python

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


# Part I - 
1. initially we Extracted JSON Digital Music, Meta Digital Music, CD, & Meta CD
2. Created a For Loop to Read JSON
3. Merged Digital Muisc and Meta Digital Music 
4. Merged CD and MetaCD
5. Finally, we created a DataFrame groupby ASIN

# Part 2- 
We begin a two pronged strategy for anlyzing 2 seperate categories:

##A. Comparative analyis of digital music vs that of CD/Vinyl 

##B. Compared the total sales vs average ranking and found top 20 ranked/selling artists/bands
  
# A: Digital Music vs CD/Vinyl 

We created a graph from our merged DataFrame to establish a count of total count of ratings compared to actual rating (1-5)
Within this graph we integrated the distribution to show the spread independent to each rating as well. 

![image](https://user-images.githubusercontent.com/116226080/215923525-25d6abf5-c233-4287-8375-39970359c116.png)

We then counted the cummulative ratings of Digital Music and Vinyl/CDs and depicted them via Pie Charts 

#### Digital Music Overall
![image](https://user-images.githubusercontent.com/116226080/215924754-e16b139d-ce5c-4a5a-bfcf-22ba9151f7c9.png)

#### CD/Vinyl Overall
![image](https://user-images.githubusercontent.com/116226080/215924855-0b4312d0-3a12-466b-a4cb-da4cee7747ed.png)

It was interesting to not that CD/Vinyl had 64% ranked at a perfect 5, whhile digital music's overall % of 5's was only 55%



# B: Total Sales, Highest Ranking, Top 20 & Comparative Analysis

Ascending Total sales by average rating

Worked off of Digital Music Only (



<img width="384" alt="Screenshot_20230130_083524" src="https://user-images.githubusercontent.com/116226080/215922333-02a45caa-df60-45f1-869e-b7fc8345fc95.png">


<img width="483" alt="Screenshot_20230130_080802" src="https://user-images.githubusercontent.com/116226080/215922541-dca94816-028b-40b9-b78c-c772dd063644.png">


<img width="515" alt="Screenshot_20230130_083228" src="https://user-images.githubusercontent.com/116226080/215922364-e9c8c131-b932-4546-83e2-4012f04c0371.png">


<img width="459" alt="Screenshot_20230130_080306" src="https://user-images.githubusercontent.com/116226080/215922577-324cdd31-299e-45e3-affc-7585a1734381.png">













findings 





contributers 

Part I: Roger

Part II: CD/Vinyl vs Digital Mussic comparative analysis of overall rating 



Part III: Sales vs Rating Analysis

Objective: Determine the total sale and average rating for each artist to derive potential correlations between the two data points to inform future stakeholders whether the higher rating guarentees higher sales. 

Functions used: 
- Groupby
- Creating dataframe
- Sort_Value
- Ascending
- Plt.Scatter
- Plt.Bar
- Plt.Pie



Findings: There is a very week positive correlation between Total Sales and Average Ratings. While the highest sales did have high ratings, there are also artists that had high ratings but few reviews. 
