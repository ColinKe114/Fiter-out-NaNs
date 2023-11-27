# Fiter-out-NaNs
Filter out undesired NaN data using Pandas
Procedural instructions:
1. Input code: *import pandas as pd* to make sure every step below can be performed successfully with pandas.
2. Upload the original data set to *content* folder, which can be found by clicking the folder icon on the left-side toolbar in Google Colab. In this case, upload the csv. file *County Health data*.
3. Define the data frame with code:* df=pd.read_csv("CountyHealthData_2014-2015.csv") *to perform the following steps based on our original dataset.
4. To filter out the NaN data, that does not contain wanted numerical information, use the code df.dropna. As a result, we will create a new dataframe called df_filtered. This can be done by inputting: *df_filtered = df.dropna(subset=['Interest_set'])*. The interest_set can be any column that we are interested in. In this case, it would be *Homicide rate*.
5. The further actions performed on df_filtered would bring results without any NaN value in the interested column. In the resulting dataset here, "NaN" homicide rate would not show up any more.
