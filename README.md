# Module 6 Challenge

Real-Estate Rental Analysis for San Francisco

[![Screen-Shot-2022-02-13-at-4-43-38-PM.png](https://i.postimg.cc/wxCyVLLr/Screen-Shot-2022-02-13-at-4-43-38-PM.png)](https://postimg.cc/dD9VQ7WR)

# Background

Proptech, the application of technology to real-estate markets, is an innovative domain in the fintech industry. Assume that I'm an analyst at a proptech company that wants to offer an instant, one-click service for people to buy properties and then rent them. 

The company wants to have a trial of this offering in the San Francisco real-estate market. If the service proves popular, they can then expand to other markets.

My job is to use my data visualization skills, including aggregation, interactive visualizations, and geospatial analysis, to find properties in the San Francisco market that are viable investment opportunities.

---

## Technologies

The data we're analyzing comes from a jupyter notebook that we've created and imported files to. We'll be using Python to run and read our data. 

* [jupyter] - (https://github.com/jupyter/notebook) - Helps us run our code and get the information we need from the data listed in csv files.


---

## Installation Guide

In order for us to get the data we need we must import pandas, plots and the csv files we want to observe.

```python
import pandas as pd
import numpy as np
import geoviews
import hvplot.pandas
from pathlib import Path
```

---

## Usage

To find the information needed we build a jupyter notebook and run various functions to pull the data from csv files.

```python
# Creating a plot to analyze neighborhood info

all_neighborhoods_df.hvplot.points(
    'Lon', 
    'Lat', 
    geo=True, 
    color='gross_rent',
    size='sale_price_sqr_foot',
    tiles='OSM',
    frame_width=700,
    frame_height=500,
    title='Average Price per Sq. Foot and Gross Rents by Neighborhood (San Francisco)'
    )

```

[![bokeh-plot.png](https://i.postimg.cc/65zK3NWh/bokeh-plot.png)](https://postimg.cc/ykJtQtSJ)
---

## Contributors

Brought to you by Elgin Braggs Jr.

---

## License

MIT