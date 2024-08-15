# eda-projects

A collection of all my data analysis projects. To run, ensure you have a Kaggle api token. Please see my [Kaggle Notebooks](https://www.kaggle.com/lizzywhite1/code)
# Ultra Marathon Large Dataset
**Late July**: Ultramarathon Dataset: A dataset with over 7 million entries of UM competitors over the past two centuries. This project involved cleaning, formatting and standardising data as well as engineering new features all using Pandas. It also involved using Matplotlib and Seaborn to visualise data.
### What I Learned: 
As this was my first EDA project I learnt a lot. The dataset was very large and it required a lot of cleaning. The dataset required me to be creative in the ways I solved some of the data cleaning issues I was having. I became better at picking up errors in my results and trouble shooting bugs in my code. More specifically some things I learnt were: 
  1. How to find, count and delete missing and duplicate values
  2. How do use string methods to extract necessary data from columns and to clean columns
  3. Using `pd.cut` to create bins/categories for numeric data
  4. How to use string formatting and regular expression and how apply to rows of data
  5. The importance of standardising entries; learnt how to create functions to return a standardised result
  6. `df.groupby` and aggregate functions to quickly obtain and visualise information about subsets of data
### What I could improve upon: 
  1. The effciency of my code: in hindsight, some methods about how I went about cleaning data were not effcient
  2. Ensuring I use categorical data types when possible to save memory
  3. Improving the presentation and motive behind certain visualisations: next time I want to have clear questions in mind and a clear and sensible idea on how is best to visualise certain data. I also want to become more comfortable taking advantage of Pandas built in `df.plot` method.
# Zomato Restaurant Dataset
- **Mid August** : Zomato Dataset: A dataset with nearly 10,000 entries of restaurants on Zomato. Unlike the first project, this one didn't involve much data cleaning so it allowed me to spend more time focusing on how I visualised the dataset.  
### What I Learned: 
This short project allowed me to solidify and futher build upon what I had learnt in my first EDA. I chose a dataset that didn't require a large amount of clearning in order to challenge myself to focus 
- The importance of creating functions: Whenever I had to do some task involving for loops and/or if-else statements to extract certain pieces of data or to manipulate data I always reverted to creating a function for this task. This made my code a lot neater and allowed me to not repeat reptitive tasks.
- Using categorical datatypes: At the start of this project I made sure to convert certain columns into the `pd.categorical` datatype to ensure I maximised memory. I then used `df.memory_useage` to calculate the percentage reduction in memory. Converting to categorical data type saved a lot of memory. I will defintely be using this data type when I have larger datasets
- Type hinting: When creating the functions I realised the data type of my inputs/outputs was ambiguous, this was where I learnt about type hint and subsquently made use of it in my code.
- The power of Plotly for creating interactive plots: While seaborn worked very well for many of my plots, I found at time when I had a large amount of different categories (e.g. 'cuisines') and I wanted to color code my graph, the coloring became ambiguous. This was when I discovered the power of Plotly to create interactive scatter plots. I also used Plotly to create heat maps on a world map!
- Using APIs to acess current information: It is sily to compare the average cost for two between countries when the currency has not been standardised. I realised I needed a way to read in current exchange rates with USD as the base currency. This was when I first used an API to obtain the up to date foreign exchange rates.
- Correlation matrices and Seaborn Heatmaps: I utilised `pd.corr()` for the first time annd used Seaborn heatmaps to investigate the correlation coeffcients (both Pearson and Spearman's) of various numeric features of the dataset
