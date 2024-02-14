## Project Overview 

The main notebook in this project is EDA.ipynb. Column_names file has explanation of the varous columns. 

### Exploratory Data Analysis

This project is centered around exploratory data analysis techniques and presentation of results to a client.

### The client Overview: 
                                                                                                               
Charles Christensen is a seller who invests with big returns, he is wondering about renovation?, which Neighborhood? Timing?                                                                                
### The data

- I will use the King County Housing Data: This dataset contains information about home sales in King County (USA).
- I will find the data in the eda schema of our database. 
- I have used DBeaver to explore the data and do the necessary querrying and joining the table

### The Tasks

1. Through EDA/statistical analysis above please come up with **AT LEAST 3 insights** regarding the overall data. One should be geographical.

2. In addition also come up with **AT LEAST 3 recommendations** for your client.

_Note, I took the perspective of a property investor. 


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Instalation Setup

### Requirements

- pyenv
- python==3.11.3

### Setup

One of the first steps when starting any data science project is to create a virtual environment. For this project you have to create this environment from scratch yourself. However, you should be already familiar with the commands you will need to do so. The general workflow consists of... 

* setting the python version locally to 3.11.3
* creating a virtual environment using the `venv` module
* activating your newly created environment 
* upgrading `pip` (This step is not absolutely necessary, but will save you trouble when installing some packages.)
* installing the required packages via `pip`

At the end, you want to make sure that people who are interested in your project can create an identical environment on their own computer in order to be able to run your code without running into errors. Therefore you can create a `requirements file` and add it to your repository. You can create such a file by running the following command: 

```bash
pip freeze > requirements.txt
```

*Note: In rare case such a requirements file created with `pip freeze` might not ensure that another (especially M1 chip) user can install and execute it properly. This can happen if libraries need to be compiled (e.g. SciPy). Then it also depends on environment variables and the actual system libraries.*

### Unit testing (Optional)

If you write python scripts for your data processing methods, you can also write unit tests. In order to run the tests execute in terminal:

```bash
pytest
```

This command will execute all the functions in your project that start with the word **test**.


### Environment

This repo contains a requirements.txt file with a list of all the packages and dependencies you will need. Before you install the virtual environment, make sure to install postgresql if you haven't done it before.

```bash
brew update
brew install postgresql@14
```

In order to install the environment you can use the following commands:

```
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```