# NG Consumption Clustering

Developed POC for a client that required prediction of natural gas consumption in a city based on the dataset provided. The dataset included the attributes:

1) KOD- ID of City
2) LG- PPL using natural gas
3) LO- PPL in City

DSK- length of the sewage network

DSRW- lenght od water network

ZWNM- Water used per person

LBM- Noumber of building

GZAL- Density of population

LNKM- Ppl per km2

POW- Area of city

CPO- number of connection to buildings generall

CPDB- Number of connection to living builnings

OG- Number of natural gas consumer

OOM- customers using NG to heating flats

OwM- custemers in cities( if 0 its a village)

GAZ- Natural Gas used in MWh

Using the given attributes, we were attempting to predict the value of GAZ through implementation  of a DNN. However, due to the discrete nature of the values present, correlation between all the attributes is in the same level of positivity and hence yields no insight. So we first cluster the data into different ranges of GAZ and then attempt to predict consumption via DNN.
