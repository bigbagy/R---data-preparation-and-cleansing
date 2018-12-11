# R---data-preprocessing-and-cleansing

### About the raw data   

The data was collected by querying IMDb’s API (see [www.omdbapi.com](http://www.omdbapi.com/)) and joining it with a separate dataset of movie budgets and gross earnings. The join key was the movie title. There are many missing data, un-standardized data format, and duplicate/inconsistent data entries that needs to be cleaned before training model can be applied.  The raw data is obtained from file [`movies_merged`](https://s3.amazonaws.com/content.udacity-data.com/courses/gt-cs6242/project/movies_merged). The raw data contains a dataframe that has 40K rows and 39 columns. Each row represents a movie title and each column represents a descriptor such as `Title`, `Actors`, `Release`, `Budget` etc.
