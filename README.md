# Advanced Census data with Python

A workshop/tutorial developed for [NICAR 2020](https://ire.org/nicar2020).

The goal is to walk people with some experience with Python and Census data through specific tasks.



## Python Census libraries you can use:

### Getting data

* [census](https://github.com/datamade/census): A simple wrapper for the United States Census Bureau's API. Provides access to ACS, SF1, and SF3 data sets.
* [census-area](https://github.com/datamade/census_area): This Python library extends the the above Census API Wrapper to allow querying Census tracts, block groups, and blocks by Census place, as well as by arbitrary geographies. **Extremely slow** -- N+1 query problem
* [cenpy](https://cenpy-devs.github.io/cenpy/): 
* [CensusData](https://jtleider.github.io/censusdata/index.html): A Python wrapper to the Census API
* [census-data-downloader](https://github.com/datadesk/census-data-downloader): From the LA Times Datadesk,  designed mostly as a command line tool to download data sets (but can be used as a Python library)
* [autocensus](https://github.com/socrata/autocensus): Python package for collecting American Community Survey (ACS) data from the Census API, along with associated geospatial points and boundaries, in a pandas dataframe. Uses asyncio/aiohttp to request data concurrently. From the maintainers, "This package is under active development and breaking changes to its API are expected."

### Working with data

* [census-data-aggregator](https://github.com/datadesk/census-data-aggregator): Another LAT Datadesk joint, "Combine U.S. census data responsibly"
* [census-error-analyzer](https://github.com/datadesk/census-error-analyzer): yet another from LAT, this one helps test to see if values are statistically different when taking the margin of error into account.
* [censusgeocode](https://pypi.org/project/censusgeocode/): wraps the Census geocoder API. Can geocode single addresses or in batch, both in Python code and as a command line tool. 
