# 2020 US Census SQL Experiments

Just playing around with PostgreSQL, csvkit and census data. See install (OSX primarily) and query notes in notes/ 

The source census csv file is here in the data/ directory.

Overview of the tools and data:
* [PostgreSQL](https://www.postgresql.org/)
* [Csvkit](https://csvkit.readthedocs.io/en/latest/)
* [US Census Data: Cities and Towns, "United States" csv file](https://www.census.gov/data/datasets/time-series/demo/popest/2010s-total-cities-and-towns.html#ds)


## CsvKit

Csvkit is an amazing set of tools for working with csv files. It relies on Python and I used virtual_env to install csvkit. See the notes/210829_install_notes.txt and the ./setup_venv.sh script on how to setup and use virtual_env with Python.

My primary use of csvkit was to feed it the census csv file and have it suggest the SQL table create command in this case. I just added an index and renamed the table. A seriously handy utility.

## PostgreSQL

I opted to install PostgreSQL via [Homebrew](https://brew.sh/). Install it however you'd like. I tend to use the psql client that installs with directly with PostgreSQL for running queries. 

## SqlLite and Jupyter Notebooks

I came back to this project much later to attempt some basic demo queries using Python/SqlLite/Jupyter Notebooks. My python environment is installed via [Anaconda](https://docs.anaconda.com/anaconda/install/index.html). I run Jupyter Notebooks in VSCode via the JupyterLab Plugin. 