# NG Consumption Clustering

Developed POC for a client that required prediction of natural gas consumption in a city based on the dataset provided. The dataset included the attributes:

1) KOD- ID of City
2) LG- PPL using natural gas
3) LO- PPL in City
4) DSK- length of the sewage network
5) DSRW- lenght of water network
6) ZWNM- Water used per person
7) LBM- Number of buildings
8) GZAL- Density of population
9) LNKM- Ppl per km2
10) POW- Area of city
11) CPO- Number of connection to buildings general
12) CPDB- Number of connection to living buildings
13) OG- Number of natural gas consumer
14) OOM- customers using NG to heating flats
15) OwM- customers in cities (if 0, it's a village)
16) GAZ- Natural Gas used in MWh

Using the given attributes, we were attempting to predict the value of GAZ through implementation  of a DNN. However, due to the discrete nature of the values present, correlation between all the attributes is in the same level of positivity and hence yields no insight. So we first cluster the data into different ranges of GAZ and then attempt to predict consumption via DNN.

The project makes use of Python and its libraries, Pandas, Numpy, Matplotlib and Seaborn for analytics and visulaization of data along with Scikit for implementation of KMeans Clustering.
