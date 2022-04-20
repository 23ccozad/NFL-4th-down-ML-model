# NFL 4th Down Decision Machine Learning Model
This repo contains the data and Jupyter notebooks used to create a machine learning model that can decide whether an NFL team should punt, kick a field goal, or "go for it" on 4th down. This served as the final project in CSCI 334: Data Mining for Dr. Navid Hashemi, Department of Computer Science, College of Charleston.

## Project Overview

<b>Data Sources</b>: Every NFL play run between the 2003 and 2021 seasons was scraped using BeautifulSoup4 in Python. Scraped data was saved into the CSV files found in `/data`. Code is provied in `data_scraping.ipynb`.

<b>ML Models</b>: Seven different machine learning algorithms were considered, shown in `data_processing_and_ml_models.ipynb`. We found the highest accuracy when using XGBoost, an algorithm based on a gradient boosted ensemble of decision trees.

<b>87% Accuracy</b>: Our final XGBoost model chooses the best play to run on 4th down 87% of the time.

## Install and Run the Project
The steps will allow you to run `data_processing_and_ml_models.ipynb`, which processes, trains, and tests a machine learning model on the data found in the `data` directory.

1. Download the `data` directory and `data_processing_and_ml_models.ipynb` into the same location on your computer.
2. Create a Python environment that has pandas, numpy, seaborn, matplotlib, sklearn, xgboost, and jupyter installed.
3. Use jupyter in this Python environment to open `data_processing_and_ml_models.ipynb`.
4. Run all cells in the notebook, and watch as the data is processed and machine models are trained and tested.

You may have noticed that these instructions don't include `data_scraping.ipynb`. This Juypter notebook was used retrieve and store the data found in the `data` directory in this repo. Feel free to use this notebook if you're interested in scraping data yourself.
