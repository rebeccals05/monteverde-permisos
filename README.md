# Monteverde Institute Internship Project on Construction Permits

## Presentation
https://docs.google.com/presentation/d/1Y-3-nKwjy6MHvegyO0mpbgjmRMYCx1WP5VWA1yjIl2k/edit?usp=sharing

## Interactive Report
https://rebeccals05.github.io/monteverde-permisos/#Spatial_Distribution_of_Permits

# Project Overview
This project analyzes the rate of construction in the Monteverde Cantón in Costa Rica (2019-2022) to understand how construction activity varies depending on the year, season, area, and type of construction permit filed.

## Research Questions
- How does the rate of construction vary depending on the season?
- What areas of Monteverde are seeing the most construction, depending on the year
- What types of construction are occurring the most, and how are they spatially distributed?

## Data
The dataset contains 403 construction permits from 2019-2022 with key variables, such as: 
- Payment date
- Permit type
- Address
- Spatial coordinates (UTM converted to latitude/longitude)
- Type of construction work

## Tools used
This project was built in R using:
- tidyverse
- ggplot
- sf
- leaflet/ggmap

## Results
### Permit Date
- The number of construction permits declined throughout the COVID-19 Pandemic, but has shown signs of recovery, as of 2022.
- Construction has is a moderately strong seasonal pattern with higher permit frequencies from November to February (dry season) and lower frequencies in other months.
- Seasonality strength: 0.54
- Trend strength: 0.44
- Construction activity is influenced by both seasonal weather patterns and external factors (COVID-19 pandemic).
### Permit Type
- The majority of permits are residential, as seen throughout the canton.
- Commercial and tourist permits are concentrated in Santa Elena and Cerro Plano.
- The most vacant permits are in Santa Elena, San Luis, and Los Llanos.
- Categories were grouped to simplify spatial visualization (and due to time constraints).

Visualizations were created with time series analyses of monthly permits, heatmaps of seasonal activity, spatial point mapping of coordinates, and interactive maps using leaflet.

## Limitations
- Limited recent data (post-2022 not included)
- Limited data prior to the COVID-19 pandemic to properly model trends and predictions
- Incomplete address and coordinate data

## Future Work
- Incorporate additional variables
- Improve classification
- Develop predictive models to estimate monthly construction permit volume and the likelihood of permit types by municipality, exploring linear regression or generalized linear models and machine learning-based approaches (random forests).
