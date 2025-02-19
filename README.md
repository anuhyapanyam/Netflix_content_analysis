# Netflix-Content-Analysis

<ul>

![image](C:\Users\panya\OneDrive\Desktop\Netflix_images\netflix.jpg)

<ul>

## __Table of Contents__ ##
<ul>

[1. About the project](#about-the-project)

[2. About the dataset](#about-the-dataset)

[3. Tools and libraries](#tools-and-libraries)

[4. Phases of the project](#phases-of-the-project)

<ul>

  [4.1. Data Exploration](#1-data-exploration)

  [4.2. Data Cleaning](#2-data-cleaning)

  [4.3. Data Analysis and Visualization](#3-data-analysis-and-visualization)

</ul>

</ul>

<hr>

## __About the project__ ##
Netflix has grown to be a dominant player in the streaming industry, offering a vast collection of movies and TV shows. The platform has expanded globally, producing and acquiring content that caters to diverse audience preferences. This project aims to analyze Netflix's content trends, focusing on:

1. The distribution of movies and TV shows across different regions.
2. Trends in content additions over time and their relationship to user demand.
3. The most popular genres and their impact on content success.
4. The effect of audience ratings and regional variations in content preferences.
5. The financial performance of Netflix and how it correlates with content releases.

By leveraging data analysis, visualization, and machine learning, the project provides insights into how Netflix strategizes its content offerings and maintains its position as a leading streaming service.
<br>

<hr>

## __About the dataset__ ##
This project's dataset is an open-source data from __Kaggle__.
<br>

> [You can access it through this link.](https://medium.com/@linhvu.nt/data-analysis-and-recommendations-on-netflix-content-28707163553a)

<u>
The dataset contains one "csv" file which has 8,807 entries with the following information:
</u>

* __Type__: Movie or TV Show
* __Title__: The name of the movie/tv show
* __Country__: The country(s) which this movie/tv show was filmed
* __Date added__: The date when the movie/tv show was added on Netflix
* __Release year__
* __Rating__: Age-based media reviews
* __Duration__: The number of minutes for movies or number of seasons for tv shows
* __Description__: A sentence which describes this movie/tv show on Netflix

<hr>

## __Tools and libraries__ ##
This project was done in Python using Jupyter Notebooks.

The libraries used are:
* __Pandas and Numpy__: Data handling and transformation
* __Matplotlib and Seaborn__: Visualization
* __Scikit-learn__: Machine learning models
* __Statsmodels__: Time series forecasting

<hr>

## __Phases of the project__ ##
### 1. Data Exploration ###

<ul>

After analyzing the data I explored its columns, and the info it contains.

1. Understanding dataset size and structure.
2. The datatypes of the columns
3. Identifying key trends in content distribution.
4. Analyzing content categories, country contributions, and rating distributions.

</ul>

<hr>

### 2. Data Cleaning ###

<ul>

After exploring the data, checked it if there are any issues.

1. Handling missing values:
  
    * Missing ratings were replaced with "Unrated."
    * __date_added__ standardized to datetime format.

2. Removing duplicates and invalid data.

3. Adding computed columns:

   * __content_age__: Difference between 2024 and __release_year__.

</ul>

<hr>

### 3. Data Analysis and Visualization ###

<ul>

<u>
Insights into content trends, country distributions, ratings, and stock performance.
</u>

1. The percentage of Movies vs. TV Shows Trend

  <ul>
  
  ![image](https://github.com/anuhyapanyam/Netflix_content_analysis/blob/main/Images/Movies%20vs.%20TV%20Shows.png)

  > Majority of Netflix content consists of movies (~70%).
  > TV show releases have increased in recent years.
  
  </ul>


2. The content age variation by country over the years

  <ul>
  
  ![image](https://github.com/anuhyapanyam/Netflix_content_analysis/blob/main/Images/content%20age%20variation%20by%20country.png)

  > Content additions peaked in 2020, aligning with pandemic-driven demand.
  > The U.S. leads in content production.
  
  </ul>

3. Geographical Distribution of Content
  <ul>
  
  ![image](https://github.com/anuhyapanyam/Netflix_content_analysis/blob/main/Images/content%20age%20variation%20by%20country.png)

  > Top contributors: United States, India, UK, Japan, South Korea.
  > South Korea heavily favors TV shows, while India leans toward movies.
  
  </ul>

4. Top Genres and Ratings
  <ul>
  
  ![image](https://github.com/anuhyapanyam/Netflix_content_analysis/blob/main/Images/Top%20Genres.png)

  ![image](https://github.com/anuhyapanyam/Netflix_content_analysis/blob/main/Images/ratings.png)
  
  > Drama, Comedy, and Action are the most popular genres.
  > High-rated content (IMDb 7+) dominates Netflix’s library.
  
  </ul>

5. Netflix Stock Performance vs. Content Releases
  <ul>
  
  ![image](https://github.com/anuhyapanyam/Netflix_content_analysis/blob/main/Images/Stock%20Price%20vs%20Content%20Releases%20(Yearly).png)
  
  > Increased content production aligns with stock price growth (2015-2020).
  > Post-2020 stock decline suggests external market influences.
  
  </ul>
  
6. Monthly Release Patterns
  <ul>
  
  ![image](https://github.com/anuhyapanyam/Netflix_content_analysis/blob/main/Images/Content%20release%20patterns%20by%20month.png)

  > Most content is added in July and December.
  > Holiday releases constitute a small percentage of total additions.

  </ul>

</ul>

<hr>