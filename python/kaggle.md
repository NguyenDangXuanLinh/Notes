# Pandas
axis=0 -- rows
axis=1 -- cols
## Selection
### Indexing in pandas
row-first, col-second (python opposite)
`loc` -- use labels; ALL INCLUSIVE 

  - `df.loc[0:100]` returns 101
  - `reviews.loc[:, ['taster_name','time']]`

`iloc` -- ignore indices (i stands for integer); LAST ONE EXCLUDED  

  - `df.iloc[0:100]` returns 100
  - `reviews.iloc[[0, 1, 2], 0]`

### with condition
`&` , `==`, `|`, `>=` -- and, eual, or, greater or equal

`isnull` , `notnull`, `isin`-- self-explain

## Summary Functions
`describe()`
`value_counts()` -- a list of unique values and how often they occur
`unique()` -- a list of unique values

## Create new repre of existing data
- `map(function, iterable))` -- applies a function to all items in an iterable.
    
      review_points_mean = reviews.points.mean()
      reviews.points.map(lambda p: p - review_points_mean)


- `apply()` -- apply a func to each element (S) or axis (DF)
      
      Series.apply(function)
      DataFrame.apply(function, axis=0)

       def remean_points(row):
        row.points = row.points - review_points_mean
        return row
    
      reviews.apply(remean_points, axis='columns')
