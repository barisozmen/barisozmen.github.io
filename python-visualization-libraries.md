## Python data visualization libraries


Here is a list of popular high level visualization libraries in Python, and blogs that compares them.

* [altair](https://altair-viz.github.io/)
   * Has a nice logic of plotting. Each part of the figure is treated as an object. A figure can be created by summing up those object. 
   * [Interactive plots](https://altair-viz.github.io/gallery/index.html#interactive-charts) are easy to create.
   * Implemented by Pthon, outputs JSON, rendered by Javascript
  

* [bokeh](https://bokeh.pydata.org/en/latest/) 
   * possible to create detailed impressive graphs.
   * relatively more difficult to understand than **altair**
   * Sponsored by [NumFocus](https://numfocus.org/)
   * Easy to use example: [selection_histogram](https://bokeh.pydata.org/en/latest/docs/gallery.html)
   * [interactive heatmap](https://bokeh.pydata.org/en/latest/docs/gallery/les_mis.html)
   * Implemented by Pthon, outputs JSON, rendered by Javascript


* [plotly](https://plot.ly/python/)
   * more professional compare to previous two
   * [3D plots](https://plot.ly/python/3d-scatter-plots/) are impressive
   * [heatmap transcription profiling of brain samples](https://plot.ly/ipython-notebooks/bioinformatics/)
   * [DNA sequence slider](https://moderndata.plot.ly/bioinformatics-plots-made-in-python-and-r/)
   * compatible with R as well

* [seaborn](https://seaborn.pydata.org/)
   * I was using this frequently before, but gave up. Not very flexible.
   

### Comparisons

* https://twitter.com/jakevdp/status/975105808861032448?lang=en
* http://pbpython.com/python-vis-flowchart.html

<img src="fig1.png" height="500" width="400">

* http://vid.ssdi.di.fct.unl.pt/ressources/lectures/files/IDV-09-Python%20Plotting.pdf
    * explains plotly and bokeh well
 

  


### Other
* [Clustered Heat Maps (Double Dendrograms)](https://ncss-wpengine.netdna-ssl.com/wp-content/themes/ncss/pdf/Procedures/NCSS/Clustered_Heat_Maps-Double_Dendrograms.pdf)

A seaborn clustered heatmap example
```
import pandas as pd
import seaborn as sns
sns.set()

# Load the brain networks example dataset
df = sns.load_dataset("brain_networks", header=[0, 1, 2], index_col=0)

# Select a subset of the networks
used_networks = [1, 5, 6, 7, 8, 12, 13, 17]
used_columns = (df.columns.get_level_values("network")
                          .astype(int)
                          .isin(used_networks))
df = df.loc[:, used_columns]

# Create a categorical palette to identify the networks
network_pal = sns.husl_palette(8, s=.45)
network_lut = dict(zip(map(str, used_networks), network_pal))

# Convert the palette to vectors that will be drawn on the side of the matrix
networks = df.columns.get_level_values("network")
network_colors = pd.Series(networks, index=df.columns).map(network_lut)

# Draw the full plot
sns.clustermap(df.corr(), center=0, cmap="vlag",
               row_colors=network_colors, col_colors=network_colors,
               linewidths=.75, figsize=(13, 13))
 ```
 
 <img src="seaborn-heatmap-example.png" height="500" width="500">




