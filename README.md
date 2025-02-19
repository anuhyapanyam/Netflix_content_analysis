# Netflix-Content-Analysis
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
This project analyzes Netflix content trends, focusing on movies, TV shows, regional distributions, ratings, and financial performance. It aims to uncover insights into content preferences and Netflix’s market strategies.
<br>

---The detailed notebook of the project is [here](Analyzing%20Netflix%20Data.ipynb).

<hr>

## __About the dataset__ ##
This project's dataset is an open-source data from __Kaggle__.
<br>

---> [You can find it here.](https://www.kaggle.com/datasets/shivamb/netflix-shows)

<u>
The dataset contains one "csv" file which has 7787 entries with the following information:
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
*__Scikit-learn__: Machine learning models
*__Statsmodels__: Time series forecasting

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
    * date_added standardized to datetime format.

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
  
  ---![image](https://user-images.githubusercontent.com/70551007/222007443-a711f14f-7d65-4149-97bf-0f33afc9ae99.png)

  > Majority of Netflix content consists of movies (~70%).
  > TV show releases have increased in recent years.
  
  </ul>


2. The growth of content creations over the years

  <ul>
  
  ---![image](https://user-images.githubusercontent.com/70551007/222007386-455595d6-92fa-4f07-bf9b-733f9f85434a.png)

  > Content additions peaked in 2020, aligning with pandemic-driven demand.
  > The U.S. leads in content production.
  
  </ul>

3. Geographical Distribution of Content
  <ul>
  
  ---![image](https://user-images.githubusercontent.com/70551007/222007273-1352b673-4c90-4e8d-a07c-445333d3be0d.png)

  > Top contributors: United States, India, UK, Japan, South Korea.
  > South Korea heavily favors TV shows, while India leans toward movies.
  
  </ul>

4. Top Genres and Ratings
  <ul>
  
  ---![image](https://user-images.githubusercontent.com/70551007/222007153-a06c604d-2f47-44e7-acbb-9c53a5869854.png)

  > Drama, Comedy, and Action are the most popular genres.
  > High-rated content (IMDb 7+) dominates Netflix’s library.
  
  </ul>

5. Netflix Stock Performance vs. Content Releases
  <ul>
  
  ---![image](https://user-images.githubusercontent.com/70551007/222006781-0a5e77a2-6564-41c1-9d86-eba8100c9341.png)
  
  > Increased content production aligns with stock price growth (2015-2020).
  > Post-2020 stock decline suggests external market influences.
  
  </ul>
  
6. Monthly Release Patterns
  <ul>
  
  ---![image](https://user-images.githubusercontent.com/70551007/222006721-3aaac1cc-3851-4a1a-b752-9ff7ce5ddd09.png)

  > Most content is added in July and December.
  > Holiday releases constitute a small percentage of total additions.

  </ul>

</ul>

<hr>