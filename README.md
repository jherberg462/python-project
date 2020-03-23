# Trends about Trending YouTube Videos

This goal of this project was to look for trends and anomalies among trending videos on YouTube. After choosing our dataset, we removed data that we decided would not be useful to provide insights, cleaned the data, and combined the data into a single CSV file. Once the data was combed into a CSV file, each group member could look for interesting and useful insights from the data.   

### Datasets 
https://www.kaggle.com/datasnaek/youtube-new

https://github.com/jherberg462/python-project/blob/master/data/cleaned_data.csv (cleaned data)

### Questions:

1. How many times have people located in selected major countries viewed trending videos in total? On a per capita basis? 

2. What percentage of likes do trending videos tend to receive among likes/dislikes in selected major countries?

3. How many comments do trending videos tend to receive? 

4. Does the ratio of likes to dislikes affect how many views a treding video gets? 

### Tasks:

1. Download files from kaggle and put them in a folder titled 'source_csv_files' in the root folder.

2. Collaberate with the group and decide which columns we agree will not look at. 

3. Load CSV files into Pandas DataFrames, combine DataFrames into a single DataFrame, and save as a single CSV file.

4. Collabertae with the group and decide which rows we want to exclude from our analysis

5. Clean data to conform with the agreed upon criteria in step 4 above.

6. Reformat dates in our dataset into datetime objects that are uniform format. 

7. Collaberate with group to decide what questions we want to answer, and assign roles. 

8. Each group member performs individual analysis depending on their assigned role. 

#### To reproduce the analysis results:

Run the code in the following order: get_data_into_single_csv.ipynb, cleanup2.ipynb, cleandata_dateissue.ipynb, the rest of the files. The various plots and charts are in the Jupyter Notebooks. 

### Results:

- Per Capita Views: Great Britain has the highest number, 1241, and Japan has the lowest one at  views per person.
![Views Per Capita](/images/ViewsPerCapitaCountry.png)

![Views by country](/images/TotalViewsPerCountry.png)

- Top Categories and trend duration: Entertainment is the category with more views and Movies has almost no views. The mayority of views are trending in the first 2.5 days they are published.

- Likes and Dislikes: If a viewer say if they like the video, there is a 95% probability that the person likes the video, compared to a 5% of saying that does not like the video.

- Number of Views vs likes and dislikes: We did not find a relatinship between number of views and likes or dislikes.
![views per interaction vs likes ratio](/images/perlikevsratio.png)


- Number of videos trending in each country: the videos got a similar number on each of the countries we use for our analysis, except for South Korea and Japan.
