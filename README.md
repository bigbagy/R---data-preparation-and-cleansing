# R---data-preprocessing-and-cleansing

### About the raw data   

The data was collected by querying IMDb’s API (see [www.omdbapi.com](http://www.omdbapi.com/)) and joining it with a separate dataset of movie budgets and gross earnings. The join key was the movie title.  The raw data is obtained from file [`movies_merged`](https://s3.amazonaws.com/content.udacity-data.com/courses/gt-cs6242/project/movies_merged). The raw data contains a dataframe that has 40K rows and 39 columns. Each row represents a movie title and each column represents a descriptor such as `Title`, `Actors`, `Release`, `Budget` , `Genre` etc.

There are lots of missing data, un-standardized data formats, duplicate/inconsistent data entries and outliers that needs to be processed and cleaned before data modeling.
