# Intallations

Setup a conda environment

```
conda create --name po-pandas
source activate po-pandas
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

```
conda install vaex
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

## Data Soucres

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

## Links

### Video 

[Data.table for R and Python](https://www.youtube.com/watch?v=Ddr8N9STSuI)


### Articles

### Github

[Data.table](https://github.com/Rdatatable/data.table)
