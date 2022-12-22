
Exploratory Data Analysis ( EDA ) of Amazon Prime's Dataset

This is a pipeline of Prime's dataset where we read the data from a source, do some data analysis and load the data to a target source.
This repo has 2 folders and 1 CSV file. One folder is the notebook folder where the ipynb notebooks is sitting and the other folder has 3 CSV files filtered from the main CSV file.

I had stored the data in my S3 bucket on AWS.

Step 1 - We extract the data from there using boto3 - the Python package.

Step 2 - We read the dataframe using pandas and start the process of transformation

Step 3 - Transformations such as Null Handling, Data Analytics that is answering some questions and bringing value out of the data.

Step 4 - I have split the dataset into 2 - One for Movies and the other one for TV shows. Since it is an OTT platform's data, splitting the dataset here makes things simpler, more interesting and clear.

Step 5 - Final part where we load the dataframes to the target source. My target source here is the Postgres DB. I load the 3 dataframes to my newly created db using SQLAlchemy.
