# System Description

The benchmarks described in this repo are obtained on a MacBook with: 

| Hardware Overview||
| ------------- |-------------|
|Model Name:|MacBook Pro|
|Model Identifier:|MacBookPro14,3|
|Processor Name:|	Intel Core i7|
|Processor Speed:|2.9 GHz|
|Number of Processors:|1|
|Total Number of Cores:|4|
|L2 Cache (per Core):|256 KB|
|L3 Cache:|	8 MB|
|Memory:|16 GB|

| Storage||
| ------------- |-------------|
|Device Name:|APPLE SSD SM0512L|
|Media Name:|AppleAPFSMedia|
|Medium Type:|SSD|
|Protocol:|PCI-Express|
|Internal:|Yes|
|Partition Map Type:|Unknown|

  
# Intallations

Setup a conda environment

```
conda create --name po_pandas
source activate po_pandas
```

Get jupyterlab up and running

```
conda install -c conda-forge jupyterlab
```

Launch jupyter lab

```
jupyter lab
```

## Pandas

```
conda install pandas scipy
```

## datatable

[Git](https://github.com/h2oai/datatable)

[Docs](https://datatable.readthedocs.io/en/latest/api/frame.html)

```
pip install datatable
```


## Vaex

Need vaex jupyter for plot_widget in vaex

```
conda install vaex
pip install vaex-jupyter
```

## Dask
Do a powered with dask thing. 

```
conda install dask
#For some visuals. 
conda install -c conda-forge ipywidgets
```

## Modin 

Modin will work with Dask as engine but aslo install Ray. 

```
pip install ray
pip install modin
```

## ARROW 

pyarrow

```
conda install -c conda-forge pyarrow
conda install -c conda-forge fastparquet 

The current version of pyarrow=0.13 does not work with Dask 2.5.0
```


# Data Soucres

[New York Taxi Trips(2015) - 146 million rows - 23GB](https://drive.google.com/file/d/0B8gjQokMGa4nTXc0Z3QyYjZBMWc/view)

[New York Taxi Trips (2009 Year 2009 - 2015 - 1 billion rows - 135GB](https://drive.google.com/file/d/0B8gjQokMGa4nTXc0Z3QyYjZBMWc/view)

[Washington DC taxi trips 2017](https://www.kaggle.com/bvc5283/dc-taxi-trips - )



## Double a csv file from bash 

```
# Remove header row 
sed 1d iris.csv > iris_noheader.csv

# Add newline to end of first file for combining if not already there
sed -i '' -e '$a\' iris.csv

# Combine files
cat iris.csv iris_noheader.csv > iris_double.csv
```

# Links

### Video 

[Data.table for R and Python](https://www.youtube.com/watch?v=Ddr8N9STSuI)


### Articles

### Github

[Data.table](https://github.com/Rdatatable/data.table)
