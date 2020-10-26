# Here are the building blocks below for starting an Altair plot. 

#### The Data
- Data in Altair is built around the Pandas Dataframe, you can load data either by normal methods or use Altairs stock datasets from the vega_datasets package within it.
```python
data = pd.read_(specify the file you are reading)(data source)
```
#### The Chart object
- With the data defined, you can instantiate Altair's fundamental object, the Chart:
```python 
chart = alt.Chart(data)
```
- Fundamentally, a Chart is an object which knows how to emit a JSON dictionary representing the data and visualization encodings, which can be sent to the notebook and rendered by the Vega-Lite JavaScript library. Let's take a look at what this JSON representation looks like, using only the first row of the data:

#### The Mark
- Next we can decide what sort of mark we would like to use to represent our data. For example, we can choose the point mark to represent each data as a point on the plot:
