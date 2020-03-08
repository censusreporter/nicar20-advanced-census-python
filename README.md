# Advanced Census data with Python

A workshop/tutorial developed for [NICAR 2020](https://www.ire.org/events-and-training/conferences/nicar-2020).

In this workshop, we'll work through the multi-step process of aggregating data from the US Census American Community Survey (ACS) to locally important geographies: specifically, [Chicago community areas](https://en.wikipedia.org/wiki/Community_areas_in_Chicago).

The workshop is designed as a Jupyter Notebook to support self-paced learning and future reference. To begin, you'll need to set up a Python environment using either [Poetry](https://python-poetry.org/) or `pip install -r requirements.txt`. If you really don't know what any of that means, you may not be ready for this workshop, because it's more about showing how to do things without a lot of explaining.



## Python Census libraries you can use:

In preparing this, I gathered a list of Python libraries designed to help with Census data. Not all of them are covered in theis repository, but I figured I'd keep the list anyway, in case it's useful.  Feel free to send pull requests if I missed any!

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
