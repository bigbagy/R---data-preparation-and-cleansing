# R---data-preprocessing-and-cleansing-for-linear-model-training

### About the raw data   

The raw data is obtained from file [`movies_merged`](https://s3.amazonaws.com/content.udacity-data.com/courses/gt-cs6242/project/movies_merged). The raw data contains a dataframe that has 40K rows and 39 columns. Each row represents a movie title and each column represents a descriptor such as `Title`, `Actors`, and `Budget`. The data was collected by querying IMDb’s API (see [www.omdbapi.com](http://www.omdbapi.com/)) and joining it with a separate dataset of movie budgets and gross earnings. The join key was the movie title. There are many missing data, un-standardized data format, and inconsistent data entries that needs to be cleaned before training model can be applied.

### Objective

The end goal is to investigate the relationship between the movie descriptors and the box office success of movies, as represented by the target variable `Gross`. 

THe data is precessed as follows: Tcleaned missing values, either as 0, (logical) NA or (string) "N.A."; cleanup data inconsistencies, for example in movie release/debut/first premier may have different values; cleanup non-standard formats, for example string format values in numeric columns; change features, there are features that are encoded as list of possible categories (such as movie genere), these categorical features can not fit into linear models and needs to be converted to series of numerical features (binaries), each binary feature will encode a movie genre (eg comedy column will be 1 if that movie belongs to comedy, thriller column will be 0 if movie is not thriller), the binary values can then be fit into linear models
