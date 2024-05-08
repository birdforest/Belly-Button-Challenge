# Belly-Button-Challenge
Challenge 14
## Build the MetaData Panel
- The function fetches metadata from a JSON file and builds the metadata panel
- Load the JSON file containing the metadata using d3.json (following class activities)
- Filters the metadata based on the sample ID provided (arrow function)
- Selects the HTML element with the ID #sample-metadata
- Clears any existing metadata inside the element (per instruction)
- Appends paragraph (p) elements to the panel for each key-value pair in the filtered metadata
- Capitalize the elements using  var capitalizedKey = key.toUpperCase(). Reference: Stack Overflow: How to uppercase Javascript object keys? https://stackoverflow.com/questions/7408638/how-to-uppercase-javascript-object-keys
## Build the Two Charts
- The function builds the bubble chart and the bar chart
- Filters the sample data based on the sample ID provided
- Extracts the necessary data for plotting the charts (OTU IDs, OTU labels, and sample values)
- Builds a bubble chart using Plotly, represetnting bacteria cultures found
- Slices and reverses the data appropriately for plotting (horizontal bar chart)
## Function to run on page load
- The function initializes the dashboard when the page loads
- Loads the JSON file containing the sample data
- Extracts the sample names from the data
- Populates the dropdown menus (select) with the sample names as options
- Get the first sample from the list and builds charts and metadata panel for it
## Function for event listener
- The function is triggered when a new sample is selected from the dropdown menu
- Rebuilds both the charts and the metadata panel for the selected sample
## Event Listeners and Dashboard Initialization
- Set up an event listener for changes in the dropdown menu
- When a new sample is selected, it triggers the optionChanged function to update the dashboard accordingly
- init() function is called to initialize the dashboard when page (re)loads
