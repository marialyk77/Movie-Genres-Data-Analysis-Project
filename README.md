❤️ I am supper supper HAPPY having completed my first Full Project with Python. 

📣 This project is sourced from the course of Alex Freberg: Pandas for Data analysis:   

           https://www.analystbuilder.com/courses/pandas-for-data-analysis 


🎁 The focus of the project is: 
  
    Exploring Movie Genres: Analyzing Trends in Budget, Revenue, Profit, Popularity, and Viewer Ratings.


🎨 As a student, I primarily followed the coding guidance provided by my trainer, whose expertise and instruction were invaluable in my learning journey. 

🧩 However, in certain instances throughout the project, I encountered unique challenges that required me to adapt and explore alternative approaches.

🦉 In these cases, I exercised my problem-solving skills to find solutions that addressed the specific requirements of the analysis.

  1. For determining which genres have high average budget and revenue, I encountered a KeyError and NotImplementedError with the trainer's suggested code. 
    Consequently, I opted to aggregate the data using the agg function to calculate the mean budget and revenue for each genre, followed by sorting the genres based on these metrics.

  2. Similarly, when investigating the relationship between movie ratings (vote average) and profit/revenue, I encountered issues with the correlation analysis.
     So, I deviated from the trainer's code: movies_counted.corr(method = 'spearman'). 
     I specifically selected only the numerical columns from the dataset. Imported NumPy and utilized 'np.number' to filter the numerical columns in the DataFrame.

     
           import numpy as np
     
           numerical_columns = movies_counted.select_dtypes(include=np.number)
     
           correlation = numerical_columns.corr(method='spearman')
