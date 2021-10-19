This is a HighCharts column chart demo, with drop-down lists to manipulate data shown.

# Data
- the key used is the season identifier.
- *categories* is an array of player names
- *appearances* is an array of the corresponding player's appearances
- *goals* is an array of the corresponding player's goals

# HTML
- a div with id *container* is required. This is where Highcharts will render the column chart.
- two drop-down lists for selection of season and statistics.

# JavaScript
- on page load, the *data* object is declared and populated, then *renderBarChart()* is run.
- *renderBarChart()* function retrieves a subset of *data* based on the selection of season and statistic, then renders the chart.

# Rendering the chart
This uses a Highcharts configuration. We pass this into the *chart()* method of the *Highcharts* object, along with the string "container".

# Adding an average line
This requires adding a spline to the chart, after calculating the average for the dataset required. An array of all the same values is generated, then the data is added as a spline to the *series* property.
