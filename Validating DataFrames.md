[[Data Validation]] in [[Pandas DataFrame|DataFrames]] is necessary after merging operations. Fore each kind of merge (horizontal and vertical), we have mehods which avoids the merge if some conditions are not true.

## [[Merging  DataFrames]]

For the *merge* method, we have the **validate** argument, which throws an error if the resultant DataFrame doesn't sastisfy the condition. 

```
dataFrame.merge(dataFrame, on='key', validate='one_to_one', 'one_to_many', 'many_to_one', 'many_to_many)
```
## [[Concatenating DataFrames]]

Concatenating DataFames could reuslt in a index overlapping situation. To avoid this, we have the boolean argument **validate_integrity**. The method throws an error if one, or more indexes are overlapped.

```
pd.concat([d1,...,dn], validate_integrity = True)
```