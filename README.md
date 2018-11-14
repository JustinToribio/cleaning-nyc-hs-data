# Is the SAT unfair?  
### Cleaning NYC high school data to start finding the answer
==============================  

## Goal of this project
The goal of this project is to clean and consolidate several datasets relating to the SAT (Scholastic Aptitude Test) and New York City (NYC) high schools. The final cleaned dataset will be used in separate projects to explore if the SAT is unfair to particular groups of students. The annual SAT is used by U.S. colleges and universities to determine which students to admit into their programs.  

## Approach
We will start by exploring each of the datasets to understand the information they contain and how they can be consolidated. Based on what we learn we will then clean the datasets to make them ready for further analysis and modeling (i.e. correcting data types and errors, removing unnecessary characters and columns, filling in missing values etc...). Finally, we will consolidate all of the data into a single cleaned dataset and export it to a csv file that is ready to use for further exploratory data analysis, visualization and predictive modeling.  

## Installing and running the project  

### Download the data  
* Clone this repo to your computer.  
* Do not alter the folder/file structure or the file references in the Jupyter Notebook will break.

### Make sure you have the "conda" package manager installed  
* If you don't, follow the instructions [here](https://conda.io/docs/user-guide/install/index.html).

### Reproduce the analysis environment and launch the Jupyter Notebook
* From the command line:
* Reproduce the analysis environment: `conda create --name env --file requirements.txt`.  
* Activate the environment: `source activate env`.  
* Launch the Jupyter Notebook: `jupyter notebook notebooks/1.0-jt-clean-nyc-hs-data.ipynb`.

### Run the Jupyter Notebook
* From the Jupyter Notebook:  
* To run each cell one at a time: click `Run` in the top control panel or press `Shift + Enter`.
* To run all of the cells: click `Kernel` in the menu bar and then `Restart & Run All`.
* After the last code cell is run, the final cleaned dataset will be exported to a csv file named "nyc_hs_data_clean.csv" in the `data/processed` folder of this project.

## Project Organization
------------

    ├── data
    │   ├── processed      <- The final cleaned data set produced by running this project.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jt-clean-nyc-hs-data`.
    │
    ├── references         <- Data dictionaries.
    │
    ├── .gitignore         <- Files and folders for Git to ignore tracking.
    ├── LICENSE
    ├── README.md          <- The top-level README for users of this project.    
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment.
                              Generated with `conda list -e > requirements.txt`.


--------