Project Title

- Data wrangling practice with New York OpenStreetMap data.

Prerequisites

- Jupyter notebook and sqlite3 already need to be installed. If not, you can download from below sites : 

https://sqlite.org/download.html

http://jupyter.readthedocs.io/en/latest/install.html

- If you already installed the programs, you need to know how to use them.

Running the tests

- First, download OSM XML file from the site : https://mapzen.com/data/metro-extracts/metro/new-york_new-york/

- Second, change the paths in 'clean and shape datas.ipynb' according to the computer and OSM XML file.

- Third, run the 'clean and shape datas.ipynb'. It can take about an hour to make all csv files.

- Fourth, make two sqlite databases. One is for small_sample_*.csv files and the other is for sample_*.csv files.

- Fifth, create 10 tables in each databases. You can get schema from here : https://gist.github.com/swwelch/f1144229848b407e0a5d13fcb7fbbd6f
Using the schema, you can make 5 tables. You need to make 5 more tables with same schema only adding the 'uncleaned_' prefix to table names.

- Sixth, in csv mode, import each csv files to each tables in databases.

- Seventh, change the paths in 'Audit sample datas.ipynb' according to the computer and OSM XML file.

- Eighth, run the 'Audit sample datas.ipynb'. You can connect to the databases and query to them.

Built With

1) readme.txt
 - Introduce about this project.

2) clean and shape datas.ipynb
 - It is written by the python code for making the sample OSM file, cleaning the data, and making csv files from OSM file.

3) Audit sample datas.ipynb
 - It is written by the python code for connecting and querying to the database to audit and find the problems in the data.

3) New_York_sample.osm
 - It is about 95MB sample of New York OSM XML file.

Author

- JehyeonHeo

Acknowledgments

- I got overall help from this case study example : https://gist.github.com/carlward/54ec1c91b62a5f911c42#file-sample_project-md

- I got New York OSM XML file from this site : https://mapzen.com/data/metro-extracts/metro/new-york_new-york/

- To understand the contents of OSM XML file, I watched videos from this site : https://www.youtube.com/watch?v=DJ2TARmvTao&list=PLCE6296A33CF47955

- To know the rules of writing the OSM data, I got help from this wiki : http://wiki.openstreetmap.org/wiki/Map_Features

- In most part of codes, I got basic parts from Udacity's Data Wrangling course.

- To write readme, I refered this site : https://gist.github.com/PurpleBooth/109311bb0361f32d87a2

- To create tables in SQL, I used the schema in this site : https://gist.github.com/swwelch/f1144229848b407e0a5d13fcb7fbbd6f
