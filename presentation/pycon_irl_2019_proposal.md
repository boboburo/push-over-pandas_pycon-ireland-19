[pandas](https://github.com/pandas-dev/pandas) has been the default library of choice for data analysis / manipulation in the Python ML ecosystem. 

Recently there has a raft of new libraries/frameworks that are similar in design intent as pandas (easy & fast analysis and manipulation of mixed data types in a tabular structure) but take different implementation pathways, incorporating newer compute paradigms. Some of these include

- [Dask](https://docs.dask.org/en/latest/why.html) allowing you to scale from single computer to run on 1000+ clusters of machines using familiar pandas APIs. 

- [data.table](https://github.com/h2oai/datatable) from h20.ai focusing on single machines, that can process moderately large amounts of data (100GB) - taking advantage of column-orientated data storage and native-c implementation of all datatypes (including strings unlike pandas)

- [modin](https://github.com/modin-project/modin) from the [RiseLab, Berkely](https://rise.cs.berkeley.edu/) taking advantage of [ray](https://github.com/ray-project/ray/) to seamlessly speed up existing pandas based notebooks, scripts, and libraries.

- [vaex](https://github.com/vaexio/vaex) a python library for lazy out-of-core data-frames that can calculate statistics on an N-dimensional grid for more than a billion (10^9) objects/rows per second and has incredibly fast and memory efficient support for all common string manipulations.

- [rapids](https://rapids.ai/) from [Nivida](https://developer.nvidia.com/rapids) a suite of software libraries, built on CUDA-X AI, allowing you build ML pipelines entirely on GPUs. 

In this talk myself and my colleague Barry will give an overview of some of emerging data-frame technologies and guide the listener to advantages, pitfalls and also considerations as to where some of these new libraries may be worthwhile considering as part of the ML practitioners toolkit. 
