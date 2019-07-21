# Forest Fire Analysis
Data on Forest Fires was explored and visualized using the R program to understand what variables contributed to the likelihood of a Forest Fire, so as to be able to better predict them. Variables that increased the severity of a Forest Fire were also explored. The [dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/forest-fires/) we used in this is associated with a scientific research paper on predicting the occurrence of forest fires in Portugal using modeling techniques. 

A preview of the dataframe is here:

![dataframe](https://i.gyazo.com/e04e44bfdf98710deec7b2abbea3ac5c.png)

The columns seen are the following:

- X: X-axis spatial coordinate within the Montesinho park map: 1 to 9
- Y: Y-axis spatial coordinate within the Montesinho park map: 2 to 9
- month: Month of the year: 'jan' to 'dec'
- day: Day of the week: 'mon' to 'sun'
- FFMC: Fine Fuel Moisture Code index from the FWI system: 18.7 to 96.20
- DMC: Duff Moisture Code index from the FWI system: 1.1 to 291.3
- DC: Drought Code index from the FWI system: 7.9 to 860.6
- ISI: Initial Spread Index from the FWI system: 0.0 to 56.10
- temp: Temperature in Celsius degrees: 2.2 to 33.30
- RH: Relative humidity in percentage: 15.0 to 100
- wind: Wind speed in km/h: 0.40 to 9.40
- rain: Outside rain in mm/m2 : 0.0 to 6.4
- area: The burned area of the forest (in ha): 0.00 to 1090.84


## Visualizing Forest Fire occurrences by Month and Day

The frequency of forest fires during each Month and Day of the week were visualized.

The trend of forest fires occuring during the summer months in the Northern Hemisphere, August and September, remarkably stuck out:

![forest fires months](https://i.gyazo.com/d08832c8c12c6c461676bcb23c910888.png)

Various Boxplots were also made analyzing variables other than forest fire count, such as area of the forest fire, wind speed, rainfall, FWI (fire weather index) were drawn up. Unsurprisingly, it was mostly seen that lower rainfall and higher FWI were factors that contributed to forest fire frequencies. 

## Visualizing the correlation of Forest Fire severity with other factors.

We measured the severity of Forest Fires by the area (in hectares) that was burnt during a forest fire.

Upon analysis of some variables compared against area using scatter plots, it was seen that factors like temperature, and drought code index (a measure of dryness, or period without rain, derived as a component of the FWI), noticeably correlated with the area of a fire. 

We noticed that some of the largest forest fires that occurred, particularly the ones with an area burnt of above 150 Hectares, happened during conditions of notably high Temperature and Drought Index.
