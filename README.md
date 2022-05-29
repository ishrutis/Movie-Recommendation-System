# Movie-Recommendation-System

Content Based Recommender System recommends movies similar to the movie user likes and analyses the sentiments on the reviews given by the user for that movie.

The details of the movies(title, genre, runtime, rating, poster, etc) are fetched using an API by TMDB, https://www.themoviedb.org/documentation/api, and using the IMDB id of the movie in the API, I did web scraping to get the reviews given by the user in the IMDB site using `beautifulsoup4` and performed sentiment analysis on those reviews.

## Technologies Used
- Python 3.8
- Framework: Flask
- Frontend: HTML/CSS/JS
- API: TMDB

## Architecture

![Recommendation App](https://github.com/ishrutis/Movie-Recommendation-System/blob/datascience-projects/images/architecture.png)


## Similarity Score

It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.

## Cosine Similarity Algorithm

Cosine similarity measures the similarity between two vectors of an inner product space. It is measured by the cosine of the angle between two vectors and determines whether two vectors are pointing in roughly the same direction. It is often used to measure document similarity in text analysis. It is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.

![image](https://github.com/ishrutis/Movie-Recommendation-System/blob/datascience-projects/images/cosine%20similarity.png)

More about Cosine Similarity : [Understanding the Math behind Cosine Similarity](https://www.machinelearningplus.com/nlp/cosine-similarity/)

## Screenshots

![img1](https://github.com/ishrutis/Movie-Recommendation-System/blob/datascience-projects/images/ss1.png)

![img2](https://github.com/ishrutis/Movie-Recommendation-System/blob/datascience-projects/images/ss2.png)

![img3](https://github.com/ishrutis/Movie-Recommendation-System/blob/datascience-projects/images/ss3.png)

![img4](https://github.com/ishrutis/Movie-Recommendation-System/blob/datascience-projects/images/ss4.png)

![img5](https://github.com/ishrutis/Movie-Recommendation-System/blob/datascience-projects/images/ss5.png)

![img6](https://github.com/ishrutis/Movie-Recommendation-System/blob/datascience-projects/images/ss6.png)


### Sources of the datasets 

1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
2. [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
3. [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
4. [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
5. [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)
