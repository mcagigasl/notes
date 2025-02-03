Explicit indexing is a way to set an arbitrary number of columns of a  [[Pandas DataFrame]] as an [[Vault Index]]

``dataFrame.set_index([])
``dataFrame.reset_index(drop=bool) // by default reset_index transform the index into a column

The advantages of explicit indexing is that subsetting is simpler in this way. For example: 

``dogs[dogs["name"].isin(["Bella", "Stella"])] 

with explicit index, is transformed into: 

``dogs_ind.loc[["Bella", "Stella"]]

However, explicit indexing avoid a data frame to have [[Tidy Data]]: *each row contains a single observation, and each variable it's store in its own column*. Indexes violate the last rule because index are not columns in a DataFrame

DataFrames Series inherits the indexing of the DataFrame.
## Slicing

Explicit index, in combination with [[Pandas loc|LOC]] allow to slice Data