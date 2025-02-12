# M1P12 Capstone Project
---

**The objective of the M1P12 Capstone Project is to apply the material from Module 1.**

**The material applied from Module 1 will be the following:**
1. Web Scraping (to acquire data)
2. Seaborn and Matplotlib (for visualizations)
3. Pandas (for dataframes)
4. Data Exploration (to confirm null values, dtypes, etc.)

**M1P12 Capstone Project has the following conditions:**
1. Project must be unique.
2. The Project notebook must include visualizations (minimum of 5 visualizations).

**For this project, two data tables for Shōnen Jump Manga will be used:**
1. Data table displaying the manga with highest circulation.
2. Data table displaying the manga which have sold over 100 million copies.

**References for data collection (by Web Scraping):**

1. https://en.wikipedia.org/wiki/Weekly_Sh%C5%8Dnen_Jump <br>
   table class="wikitable sortable jquery-tablesorter" <br>
   table1 = pd.read_html('https://en.wikipedia.org/wiki/Weekly_Sh%C5%8Dnen_Jump'), table1[4] <br>
   
2. https://en.wikipedia.beta.wmflabs.org/wiki/List_of_best-selling_manga <br>
   table class="wikitable sortable jquery-tablesorter" <br>
   table2 = pd.read_html('https://en.wikipedia.beta.wmflabs.org/wiki/List_of_best-selling_manga'), table2[1] <br>

**The outline for the project will be the following:**

**The project will be split into three parts:**
1. Part 1 will be working with the data of manga with the highest circulation. One plot (visualization) will be displayed here. <br>
- *Plot 1 will display a bar plot of the top ten circulated manga.* <br>
   
2. Part 2 will be working with the data of manga which have sold over 100 million copies. Two plots (visualizations) will be displayed here. <br>
- *Plot 2 will display a bar plot of the sum of approximate sales for each demographic.* <br>
- *Plot 3 will display a horizontal bar plot of the number of volumes for each manga, with each bar colored based on the publisher.* <br> 

3. Part 3 will be combining both data frames (highest circulation data with 100 million copies sold data). Two plots (visualizations) will be displayed here. The intention is to find a relation between a column of values from one data frame with another column of values from the second data frame. <br>
- *Plot 4 will display a scatter plot of the total circulation (from highest circulation data) vs approximate sales (from 100 million copies data). Only manga series found from both data tables will be included.* <br>
- *Plot 5 will include a double bar plot for Manga Series vs number of Issues (from highest circulation data) and number of Volumes (from 100 million copies data).
  A second bar plot will be displayed next to this (Plot 5) displaying  Manga Series vs the average number of issues per volume (number of Issues/number of Volumes).* <br>

**Questions for the project:**
1. Part 1 (data of manga with the highest circulation): <br> 
   *What are the top 10 circulated manga?* 
   
2. Part 2 (data of manga which have sold over 100 million copies): <br> 
   *What are the sum of approximate sales for each demographic?* 
   
3. Part 2 (data of manga which have sold over 100 million copies): <br>
   *What are number of volumes for each manga? Use bar plot and have each bar colored based on a publisher. (Based on the plot, we could see which publisher has manga with the highest number of volumes.)*
   
4. Part 3 (both data of manga with the highest circulation and data of manga which have sold over 100 million copies): <br>
   *What is the relationship between total circulation with  approximate sales? (Based on the scatter plot, does a higher circulation usually yield higher sales?)* 
   
5. Part 3 (both data of manga with the highest circulation and data of manga which have sold over 100 million copies): <br>
   *What is the relationship between number of Issues with  number of Volumes for each manga series? What is the average number of issues per volume? (Note: For this question, to save space, I will only plot 3 manga series: One Piece, Naruto and Bleach)*

*Note for question 5: To my understanding one magazine issue contains one chapter from a volume for a manga series (a magazine usually contains a collection of one chapter from different manga series). Question 5 is to observe how many chapters on average are found in a volume.*


**Summary for each part and their subsections in the notebook:**

**Part 1 (data of manga with the highest circulation):**
- Part 1.1: Data collection by Webscraping
- Part 1.2: Data exploration and find top ten circulated manga
- Part 1.3: Plot 1, Seaborn, Data Visualization displaying top ten circulated manga <br>

**Question for Part 1:**
- *What are the top 10 circulated manga?*

**Part 2: Data of manga which have sold over 100 million copies**
- Part 2.1: Data collection by Webscraping
- Part 2.2: Data exploration
- Part 2.3: Converting Values from Object (strings) to Numerical (from two columns)
- Part 2.4: Group each demographic, and include for each the sum of approximate sales
- Part 2.5: Plot 2, Seaborn, Data Visualization displaying the sum of approximate sales for each demographic
- Part 2.6: Plot 3, Seaborn, Data Visualization displaying Number of Volumes per Manga Series, with each bar colored based on Publisher <br>

**Questions for Part 2:**
- *What are the sum of approximate sales for each demographic?* 
- *What are number of volumes for each manga? Use bar plot and have each bar colored based on a publisher. (Based on the plot, we could see which publisher has manga with the highest number of volumes.)*

**Part 3: Combining Data of Manga with Highest Circulation with Data of Manga which have Sold over 100 Million Copies**
- Part 3.1: Combining dataframes of Highest Circulation data with 100 Million Copies data, based on having the same Manga Series
- Part 3.2: Plot 4, Seaborn, Data Visualization with Scatter Plot of Total Circulation vs Approximate Sales
- Part 3.3: Plot 5, Seaborn, Data Visualization with Double Bar Plot of Manga Series vs Number of Issues and Volumes, with a second plot displaying Manga Series vs (Average) Number of Issues per Volume <br>

**Questions for Part 3:**
- *What is the relationship between total circulation with  approximate sales? (Based on the scatter plot, does a higher circulation usually yield higher sales?)*
- *What is the relationship between number of Issues with  number of Volumes for each manga series? What is the average number of issues per volume? (Note: For this question, to save space, I will only plot 3 manga series: One Piece, Naruto and Bleach)*


End
     
