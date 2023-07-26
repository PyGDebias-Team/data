## Dataset Description

26 graph datasets are collected in this library, including 24 commonly used ones and two newly constructed ones (Aminer-L and Aminer-S).
We provide their descriptions as follows.

-  **Facebook**: Facebook has anonymized features for each node representative of various attributes of a person’s Facebook profile.
-  **Pokec_z & Pokec_n**:  The two datasets are sampled from Pokec by province. Pokec contains anonymized data of the whole social network in 2012, in which the profiles contain gender, age, hobbies, interest, education, working field and etc.
-    **NBA**: This dataset is an extension of a Kaggle dataset containing around 400 NBA basketball players. Features include the performance statistics of players in the 2016-2017 season and other various information e.g., nationality, age, and salary.
-   **German**: The dataset is a credit graph which has 1,000 nodes representing clients in a German bank that are connected based on the similarity of their credit accounts.
-   **Credit**: Credit contains individuals which are connected based on the similarity of their spending and payment patterns.
- **Recidivism**: Recidivism has 18,876 nodes representing defendants who got released on bail at the U.S state courts during 1990-2009, where defendants are connected based on the similarity of past criminal records and demographics.
-  **Google+**: The dataset is created by data collected from a social networking platform developed by Google.
-  **AMiner-L** & **AMiner-S**: **AMiner-L** and **AMiner-S** are co-author networks with sensitive attributes ready for algorithmic fairness study on graphs. Specifically, we construct AMiner-L (titled 'LCC' in our built-in data loader) and AMiner-S (titled 'LCC_small' in our built-in data loader) based on the AMiner network [1]. To construct the two datasets, we first filter out the nodes in the AMiner network with incomplete information. Then we adopt two different approaches to sample a connected network from the filtered dataset: AMiner-L is a subgraph sampled with random walk, while AMiner-S is the largest connected component of the filtered AMiner network. In both datasets, nodes represent the researchers in different fields, and edges denote the co-authorship between researchers. The sensitive attribute is the continent of the affiliation each researcher belongs to, and the labels of nodes represent the primary research field of each researcher. 
-    **Cora**: The Cora dataset is a collection of computer science research papers categorized into different topics.
-  **Citeseer**: The CiteSeer dataset is a digital library of scientific articles, primarily focused on computer science, featuring citation relationships and widely utilized for research in information retrieval and citation network analysis.
-   **Pubmed**: Pubmed contains citation networks that consider articles as nodes and descriptions of articles as their nodal attributes.
-   **Amazon**: The dataset constitutes a respective knowledge graph with entities and relations crawled from Amazon. The collection consists of four different domains: CDs and Vinyl, Clothing, Cell Phones, and Beauty.
-    **Yelp**: The Yelp dataset is a large collection of user-generated reviews and associated ratings for businesses, encompassing various industries and geographical locations.
-    **Ciao**: The Ciao dataset is a comprehensive collection of product reviews and ratings from the Ciao shopping website.
-    **DBLP**: The DBLP dataset is a bibliographic database containing computer science research publications, authors, and their relationships.
- **Filmtrust**: The Filmtrust dataset is a collection of movie ratings and trust relationships between users.
-   **Lastfm**: The Last.fm dataset is a music dataset that contains user listening histories, artist information, and user preferences.
-   **ML100k**: The ML-100K dataset is a widely used benchmark dataset in the field of recommender systems, containing movie ratings and user information for evaluating collaborative filtering algorithms.
-    **ML1m**: The ML-1M dataset is a movie rating dataset that contains one million ratings from users on various movies.
-   **ML20m**: The ML-20M dataset is a larger movie rating dataset consisting of 20 million ratings from users on a vast collection of movies.
- **Oklahoma**: Oklahoma is a dataset composed of social networks of the University of Oklahoma. A link represents a friendship relation in
social media, and every user has a profile for vertex features, including student/faculty status, gender, and major,
-   **UNC**: UNC is a dataset of social networks in the University of North Carolina at Chapel Hill.


## Statistics

|                |               #Nodes               |   #Edges   | #Features |
| :------------: | :--------------------------------: | :--------: | :-------: |
|  **Facebook**  |               1,045                |   53,498   |    573    |
|  **Pokec_z**   |               67,796               |  882,765   |    276    |
|  **Pokec_n**   |               66,569               |  729,129   |    265    |
|    **NBA**     |                403                 |   16,570   |    95     |
|   **German**   |               1,000                |   24,970   |    27     |
|   **Credit**   |               30,000               |  200,526   |    13     |
| **Recidivism** |               18,876               |  403,977   |    18     |
|  **Google**+   |              290,468               |   3,601    |   2,532   |
|  **AMiner-L**  |              129,726               |  591,039   |   5,694   |
|  **AMiner-S**  |               39,424               |   52,460   |   5,694   |
|    **Cora**    |               2,708                |   4,751    |   1,433   |
|  **Citeseer**  |               3,312                |   4,194    |   3,703   |
|   **Pubmed**   |               19,717               |   88,648   |    500    |
|   **Amazon**   |       2,549 (item) 2 (genre)       |   2,549    |    N/A    |
|    **Yelp**    |       2,834 (item) 2 (genre)       |   2,834    |    N/A    |
|    **Ciao**    |  7,375 (user)  106,797 (product)   |   57,544   |    N/A    |
|    **DBLP**    |  22,166 (user)  296,277 (product)  |  355,813   |    N/A    |
| **Filmtrust**  |     1,508 (user) 2,071 (item)      |   35,497   |    N/A    |
|   **Lastfm**   | 1,892 (customer) 17,632 (producer) |   92,800   |    N/A    |
|   **ML100k**   |      943 (user) 1,682 (item)       |  100,000   |     4     |
|    **ML1m**    |     6,040 (user) 3,952 (item)      | 1,000,209  |     4     |
|   **ML20m**    |    138,493 (user) 27,278 (item)    | 20,000,263 |    N/A    |
|  **Oklahoma**  |               3,111                |   73,230   |    N/A    |
|    **UNC**     |               4,018                |   65,287   |    N/A    |