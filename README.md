# Data_Preprocessing_Systematic_Approach
The purpose is just like snippet, you can reffer to it or use as a framework . Source link is attached to each title.

## 1. First and Foremost
  ### 1.1) Descriptive Approach
            https://medium.com/analytics-vidhya/how-to-summarize-data-with-pandas-2c9edffafbaf#3677
   #### · info()


   #### · describe()-       can include non numeric cols by df.describe(include="all" or [dtyp1,dtype2]), similarly we can use exclude.


   ####  · value_counts():  returns counts of unique values for the specified series. NaN values are excluded by default. df.col.value_counts().
                             You can get the frequency (instead of count) for each value by setting the normalize = True


   #### · nunique() : :     Count distinct observations. Can be used for a dataframe or a series. By default, it exclude the NaN values.
                             If you need to include the NaN values, use the parameter dropna= False


   ####  · sum():           Return the sum of the values for the requested axis. You can use it for both dataframe and series.
                            You can specify to apply the function only to numeric types by using the parameter: numeric_only = True

   ####  · count():         Return number of non-NA/null observations, Can be applied to both dataframe and series

   ####  · min(), max(), mean(), and median() -    df.min()

   ####  · agg():            Apply more than one aggregation operations to the same dataset over the specified axis.
                              df[[cols]].agg(["mean"  ,"median"})   


 ####    · groupby()         Allows you to group data (by applying aggregate functions like sum, max, min…) with the same values into summary rows:
                               df[["col or s"]].groupby("col or s").sum("col")


 ### 1.2) Culprit Investigation

  #### .Duplicates:         
