# Final Report ---- [Yelp Maps](https://cs61a.org/proj/maps/#phase-2-unsupervised-learning)
The [pdf file](https://github.com/XiaoqianZhu1997/HSG_exchange_courses/blob/master/Skills_Programming_Introduction_Level/report.pdf) for the report is alread uploaded on Github.
## 1  Background 
Our report is based on an online project called “[Yelp maps](https://cs61a.org/proj/maps/#phase-2-unsupervised-learning)” available in Berkley online platform, therefore we used data sets from their website.\
We download the dataset [maps.zip](https://cs61a.org/proj/maps/maps.zip), including all the starter codes we need and we coded on three files: [utils.py](https://github.com/XiaoqianZhu1997/HSG_exchange_courses/blob/master/Skills_Programming_Introduction_Level/utils.py);
[abstractions.py](https://github.com/XiaoqianZhu1997/HSG_exchange_courses/blob/master/Skills_Programming_Introduction_Level/abstractions.py) ; [recommend.py](https://github.com/XiaoqianZhu1997/HSG_exchange_courses/blob/master/Skills_Programming_Introduction_Level/recommend.py). 
The first two files are more related to the helper functions and preparation works, while the last one is the main file for execution and visualization.\
In this project, we create a visualization of restaurant clustering and rates prediction round the city of Berkley, depending on certain criteria such as the given user and the type of restaurant we are searching. 
We choose this project because we found it’s very interesting and easily applicable to our daily lives, if we have the data of the restaurants in St.Gallen, we can do the same thing. 
Besides, not just in what respects to restaurants but also to facilities from other fields such as hospitals or libraries for example.

## 2	Introudction
### 2.1	 Explain the Voronoi Diagram:
Our visualization we will be based on a [Voronoi diagram](https://en.wikipedia.org/wiki/Voronoi_diagram) which represents the division of a plane (in this case a map) into regions. 
And this partition will be based on the distance of points in a specific subset of the plane. These set of points will be specified beforehand and will be responsible for generating our parted map given that for each point (or seed) there will be a corresponding region containing all the points that are closer to that seed than to any other.  \
In our representation the seeds will be dots representing the location of the restaurants in the map and we use a Voronoi diagram to divide the map because we often find useful to find nearest restaurant within a given area at which we (as a user) might be at.

