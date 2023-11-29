# Creating A Subset for A Specific Analysis-State and Homicide Rate
## Overview
The instructions below would guide you through compiling a subset from a larger public dataset and filtering out undesired NaN values for better analysis. All procedures would be done within a Google Colab notebook with pandas and Python.

- The instructions are designed for people with little experience in data processing or coding. They could go very detailed sometimes. Please feel free to skip around depending on your experience level.

The overall process would be
1. Import the public dataset.
2. Read and define basic elements.
3. Filter out the undesired parts of the data.
4. Export the outcome as a csv. file.

- This repository filters out NaN data for homicide rate from the dataset County Health Data 2014-2015 for better analysis. The final dataset with NaN data filtered out is in the file *CKe Feeder 3.1 csv*. The process would be demonstrated with the County Health Data and result in the final dataset in the repository. 

## Import the public dataset
1. Open a new Google Colab file.
2. Upload the original data set to *content* folder.
   
   The content folder can be found by clicking the folder icon on the left-side toolbar in Google Colab. If it does not show up, click on the folder icon with a little arrow above the sample data folder.
   
   Upon seeing the *content* folder, click on the three dots right beside it. Do *not* upload the file to the subfolders.
   
   In this case, upload the csv. file *County Health data*.

## Read and define basic elements
1. Input code: *import pandas as pd* to make sure every step below can be performed successfully with pandas.
2. Define the data frame with code:* df=pd.read_csv("CountyHealthData_2014-2015.csv") *to perform the following steps based on our original dataset.

## Filter out the undesired parts of the data
4. To filter out the NaN data, that does not contain wanted numerical information, use the code df.dropna. As a result, we will create a new dataframe called df_filtered. This can be done by inputting: *df_filtered = df.dropna(subset=['Interest_set'])*. The interest_set can be any column that we are interested in. In this case, it would be *Homicide rate*.
5. The further actions performed on df_filtered would bring results without any NaN value in the interested column. In the resulting dataset here, "NaN" homicide rate would not show up any more.

## Export the outcome as a csv. file
