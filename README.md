# Data visualization - <img src="https://cdn.worldvectorlogo.com/logos/netflix-3.svg" alt="netflix" width="100" style="fmargin:0 10px 10px 0"/> </a> Movies and TV Shows




The goal of this notebook is to share data visualization tools and techniques along to communicate practiques and methods to an efficient and interesting data storytelling.
Join me on this fun journey :coffee:

## Tools
<p align="left"> <a href="https://www.python.org/" target="_blank"> <img src="https://cdn.worldvectorlogo.com/logos/python-5.svg" alt="Python" width="40" height="40"/> </a>
<a href="https://matplotlib.org/stable/" target="_blank"> <img src="https://cdn.worldvectorlogo.com/logos/matplotlib-1.svg" alt="Matplotlib" width="40" height="40"/> </a>
 <a href="https://plotly.com/python/" target="_blank"> <img src="https://plotly.com/all_static/images/icon-dash.png" alt="Plotly" width="40" height="40"/> </a>
<a href="https://numpy.org/" target="_blank"> <img src="https://cdn.worldvectorlogo.com/logos/numpy-1.svg" alt="Numpy" width="40" height="40"/> </a>
<a href="https://pandas.pydata.org/" target="_blank"> <img src="https://cdn.worldvectorlogo.com/logos/pandas.svg" alt="Pandas" width="40" height="40"/> </a>
<a href="https://www.jetbrains.com/pycharm/?var=1" target="_blank"> <img src="https://upload.wikimedia.org/wikipedia/commons/1/1d/PyCharm_Icon.svg" alt="PyCharm" width="40" height="40"/> </a>



## Dataset
The [Netflix Movies and TV Shows Dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows) from Bansal, S. (2021), is a tabular dataset consists of listings of all the movies and tv shows available on Netflix, along with details such as - cast, directors, ratings, release year, duration, etc.

Netflix is one of the most popular media and video streaming platforms. They have over 8000 movies or tv shows available on their platform, as of mid-2021, they have over 200M Subscribers globally. [1]


## Attributes
 * Type (movie or TV show)
 * Title
 * Director
 * Cast
 * Country
 * Date added
 * Release year
 * Rating (TV-MA, TV-14, TV-PG, etc)
 * Duration (in minutes if it's movie or seasons if it's TV show)
 * Listed in (category)
 * Description

## Type of content distributtion
As we can observe, the Netflix catalog has approximately 70% movies over 30% TV shows. Also we can see that the catalog contains 6131 movies and 2676 TV shows, that's 8807 elements of content!!
<p align="center">
  <img src="https://github.com/Edgar-La/Data_visualization_MoviesTVshows/blob/main/plots/content_distribution.png" alt="netflix" width="700" />
</p>
Now, we have interest in see how is the distribution of content in different countries, so we choose 8 arbitrary countries. Notice how every country keeps the relation between movies and TV shows, except for India and Japan. India has almost 92% of movies, in the other hand Japan has almost 63% for TV shows (maybe cause its affinity to anime <a href="" target="blank"> <img src="https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/e395d8b4-53c0-4af8-a76a-004679f72b57/ddyqpbe-e2e4dec8-0f3e-47d5-b1c6-200412bd7619.png/v1/fit/w_537,h_632/shinobu_kocho_render_6_by_animerendersss_ddyqpbe-375w-2x.png?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOjdlMGQxODg5ODIyNjQzNzNhNWYwZDQxNWVhMGQyNmUwIiwiaXNzIjoidXJuOmFwcDo3ZTBkMTg4OTgyMjY0MzczYTVmMGQ0MTVlYTBkMjZlMCIsIm9iaiI6W1t7ImhlaWdodCI6Ijw9NjMyIiwicGF0aCI6IlwvZlwvZTM5NWQ4YjQtNTNjMC00YWY4LWE3NmEtMDA0Njc5ZjcyYjU3XC9kZHlxcGJlLWUyZTRkZWM4LTBmM2UtNDdkNS1iMWM2LTIwMDQxMmJkNzYxOS5wbmciLCJ3aWR0aCI6Ijw9NTM3In1dXSwiYXVkIjpbInVybjpzZXJ2aWNlOmltYWdlLm9wZXJhdGlvbnMiXX0.Bvd28XVo9C6Q7Nj--i9lsJSeEZb9nlMcCf_7ItURB_c" alt="anime" width="20" height="20"/> )
<img src="https://github.com/Edgar-La/Data_visualization_MoviesTVshows/blob/main/plots/content_distribution_per_country.png" alt="netflix" width="1000" /> </a>

 ## Director
 The attriburte Director is the one with most missing data, but as a exercise with wanted to show the top 15 directors who appear the most.
<p align="center">
  <img src="https://github.com/Edgar-La/Data_visualization_MoviesTVshows/blob/main/plots/directors_in_netflix_database.png" alt="netflix" width="500" />
</p>

 ## Cast
 The attriburte Cast is the third with most missing data, but also, the attribute with the mst number of elements, it contains almost 40000 actors, so as a exercise with wanted to show the top 40 actors who appear the most.

 <p align="center">
  <img src="https://github.com/Edgar-La/Data_visualization_MoviesTVshows/blob/main/plots/top_cast_in_netflix_database.png" alt="netflix" width="640"/> </a>
</p>

 ## Country
 In the following chart, we can see the elements that every country has, as expected, the US has the most ammount of elements, followed by India and UK, the following countries has a simillar proportion with each other.
 <p align="center">
  <img src="https://github.com/Edgar-La/Data_visualization_MoviesTVshows/blob/main/plots/content_elements_per_country_in_netflix_database.png" alt="netflix" width="800"/> </a>
 </p>


 ## Date added
 Ih the following plot, we can observe the ammount of elements that were added to the Netflix catalog, notice that in gray color are the movies and in red color are the TV shows, also the black vertical bars indicate a different year.
 From this plot we can notice several thigs:
  * the ammount of items per movie and per TV shows has increase over the years
  * the months where the elements are added tend to be in the beginning and ending of the year
  * the porportion movies/TV shows remains over the years
 <img src="https://github.com/Edgar-La/Data_visualization_MoviesTVshows/blob/main/plots/date_added_per_content_in_netflix_database.png" alt="netflix" width="1000" /> </a>

 ## Release year
 In this plot we can infer several things:
 * in the 2000 decade the amount of movies/TV shows increased considerably
 * after 2018 the amount decrease, maybe because un updated data or maybe because pandemic
 * the plot follows an exponential distributtion
 <img src="https://github.com/Edgar-La/Data_visualization_MoviesTVshows/blob/main/plots/release_year_content_in_netflix_database.png" alt="netflix" width="1000" /> </a>

 ## Rating
 In this pie chart, we can observe the rating distributtion taht the Betflix database has, as we can notice, almost 40% is for TV-MA audidence, follow by TV-14 and TV-PG, as we expected, because the goal of Netflix is to capture the attention of a global audience. Of course, it has content restricted for adults and in counterpart, content dedicated for kids, bith in less proportions.
 <p align="center">
 <img src="https://github.com/Edgar-La/Data_visualization_MoviesTVshows/blob/main/plots/content_classification_in_netflix_database.png" alt="netflix" width="600" /> </a>
 </p>

 ## Duration
 In ths chart of TV shows seasons we can see the almost all the TV shows has 1 seasons, followed by 2, 3, and so on.
 <p align="center">
  <img src="https://github.com/Edgar-La/Data_visualization_MoviesTVshows/blob/main/plots/seasons_tv_shows.png" alt="netflix" width="700" /> </a>
 </p>
 
  In the case of Movies, the average tend to be 100 minutes which is approximately 1 hour 40 minutes.
  <p align="center">
  <img src="https://github.com/Edgar-La/Data_visualization_MoviesTVshows/blob/main/plots/movies_duration.png" alt="netflix" width="600" /> </a>
 </p>

 ## Listed in
 For the category, we can observe the top categories in a _wordcloud_, the bigger the word the most appear in the catalog.
 <p align="center">
  <img src="https://github.com/Edgar-La/Data_visualization_MoviesTVshows/blob/main/plots/top_categories_in_Netflix_database.png" alt="netflix" width="900" /> </a>
 <p align="center">
  In addition, we wanted to know the top 4 categories in 8 arbitrary countries. As we can expect, every country have different tastes for each category.
  <img src="https://github.com/Edgar-La/Data_visualization_MoviesTVshows/blob/main/plots/top_categories_per_country.png" alt="netflix" width="1000" /> </a>


 ## Description
 Finally, we made an interes wordclud:
 We take the synopsis of all the 8807 elements ad extract the 150 most repeated words, those words where placed over the Netflix logo and the result was the following wordcloud!! 
 <img src="https://github.com/Edgar-La/Data_visualization_MoviesTVshows/blob/main/plots/descriptions_in_Netflix_wordcloud.png" alt="netflix" width="1000" /> </a>






## References
[1] Bansal, S. (2021). Netflix Movies and TV Shows. Kaggle. https://www.kaggle.com/datasets/shivamb/netflix-shows
[https://www.holisticseo.digital/python-seo/word-cloud/]: <> 
