# eda-projects

A collection of all my data analysis projects. To run, ensure you have a Kaggle api token. Please see my [Kaggle Notebooks](https://www.kaggle.com/lizzywhite1/code) for improved readability.
# Ultra Marathon Large Dataset
**Late July**: Ultramarathon Dataset: A dataset with over 7 million entries of UM competitors over the past two centuries. This project involved cleaning, formatting and standardising data as well as engineering new features all using Pandas. It also involved using Matplotlib and Seaborn to visualise data.
### What I Learned: 
As this was my first EDA project I learnt a lot. The dataset was very large, and it required a **lot** of cleaning. The dataset required me to be creative in the ways I solved some of the data cleaning issues I was having. I also became better at picking up data entry errors in my results. For example, I noticed that some people apparently ran their 100km race with an average speed faster than the fastest 60m dash ever recorded, these results had to be filtered out!  More specifically some things I learnt were: 
- **Handling missing and duplicate values**: How to find, count and delete missing and duplicate values.
- **String methods to extract and clean data**: How to use string methods to clean existing columns and extract necessary data for new columns.
- **Creating bins for categorical data:** Using `pd.cut` to create bins/categories for numeric data. This was helpful when creating my own standardised age categories as many races used a different set of age categories.
- **The power of regular expressions for data cleaning/extraction:** How to use regular expressions to clean and extract data. For example, I had to use regular expression to extract content from the last parenthesis in a specific column.
- **The importance of standardising columns**: I learnt how to create functions to return a standardised result (for example, making sure all distances were recorded in km).
  6. **Power of`df.groupby` and aggregation functions:** I used `df.groupby` and aggregate functions to quickly obtain and visualise information about subsets of data.
### What I could improve upon: 
  1. The efficiency of my code: in hindsight, some methods about how I went about cleaning data were not efficient. I need to continue to learn of new string methods and methods in pandas in order to speed up the way I go about cleaning data.    
  2. Ensuring I use categorical data types when possible to save memory. The dataset I worked with was very large, it would’ve helped to use a more memory efficient data type when possible.
  3. Improving the presentation and motive behind certain visualisations: next time I want to have clear questions in mind and a clear and sensible idea on how is best to visualise certain data. I also want to become more comfortable taking advantage of Pandas built in `df.plot` method.
# Zomato Restaurant Dataset
- **Mid August** : Zomato Dataset: A dataset with nearly 10,000 entries of restaurants on Zomato. Unlike the first project, this one didn't involve much data cleaning so it allowed me to spend more time focusing on how I visualised the dataset.  
### What I Learned: 
This short project allowed me to solidify and further build upon what I had learnt in my first EDA. I chose a dataset that didn't require a large amount of clearing so that I could focus more on learning how to go about analysing the data. 
- **The importance of creating functions**: Whenever I had to do any task involving for loops or if-else statements to or manipulate data, I always tried to create a function to complete this task. This made my code a lot neater and allowed me to not repeat repetitive tasks.
- **Using categorical datatypes**: At the start of this project I made sure to convert certain columns into the `pd.categorical` datatype to ensure I maximised memory. I then used `df.memory_useage` to calculate the percentage reduction in memory. Converting to categorical data type saved a lot of memory. I will definitely be using this data type when I have larger datasets.
- **Type hinting**: When creating the functions I realised the data type of my inputs/outputs was ambiguous, this was where I learnt about type hint and subsequently made use of it in my code.
- **The power of Plotly for creating interactive plots**: While seaborn worked very well for many of my plots, I found at times when I had large amounts of categories (e.g. 'cuisines') and I wanted to colour code my graph, the colouring became ambiguous. This was when I discovered the power of Plotly to create interactive scatter plots. I also used Plotly to create heat maps on a world map!
- **Using APIs to access current information:** It is silly to compare the average cost for a meal for two between countries when the currency has not been standardised. I realised I needed a way to read in current exchange rates with USD as the base currency. I used an API to obtain the up to date foreign exchange rates.
- **Correlation matrices and Seaborn Heatmaps**: I utilised `pd.corr()` for the first time and used Seaborn heatmaps to investigate the correlation coefficients (both Pearson and Spearman's) of various numeric features of the dataset.
### What I could improve upon: 
- **Applying ML techniques to build predictive models:**  The next step in myself education is to begin learning the fundamentals of machine learning. I am excited to start digging into the maths behind popular models and learn how to use popular ML libraries to make my own models.
- **Become more confident in extracting the necessary data**: For example, It took me a lot of time to figure out how to create a function to extract the different cuisines listed for each restaurants and then create a dictionary containing each cuisine and a count of its occurrence. For my next project, I want to choose a dataset that requires substantial data cleaning and feature engineering to improve my ability to work with messier datasets. 
