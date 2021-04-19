# GeoDataSet
This repository contains the work for the GeoDataSet class I created in Python.

To create a new GeoDataSet:
```python

geods = GeoDataSet(
  frame=<string, DataFrame or GeoDataFrame representing geospatial data>
  coord_field1=<name of column containing the first coordinate>,
  coord_field2=<name of column containing the second coordinate>,
  coord_field3=<name of column containing the third coordinate>,
  value_field=<name of column containing a value>
)
```

To make a field PERSISTENT, i.e it will not be allowed to change when reassigning the 'frame' attribute one can add the field to the GeoDataSet as a Tuple.
```python
geods = GeoDataSet(
  frame=<string, DataFrame or GeoDataFrame representing geospatial data>,
  value_field = (<name of column containing a value>, True)
)
```
