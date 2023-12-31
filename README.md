**Purpose:**
The purpose of this project is to explore the alternative fuel stations in the US using geospatial analysis in R.

**Questions:** 
Where in the US (lower 48 states only) are the most common types of alternative fuel stations concentrated? Which states have the most alternative fuel stations, which have the most stations per unit area, and which have the most stations per person? 

**Introduction:** 
The main dataset we will be using to answer these questions is the 'Alternative Fuel' data set. This dataset comes from the US Department of Energy and it provides information on the alternative fuel stations within the United States. The columns we will use include FUEL_TYPE_CODE (the type of fuel station, coded with an abbreviation), STATE (the US state in which fuel station is located), X (the latitude coordinate of the fuel station), and Y (the longitude coordinate of the fuel station). We will also use R's built in dataset "state.x77" to get the populations and areas for the states as well as "state.center" for coordinates of the center of each state and "state.abb" for abbreviations of the state names. 

**Approach:** 
We will start by wrangling all the data necessary for analysis by creating, filtering, summarizing, and joining all necessary data frames, computing the relevant density statistics, and combining data frame with sf object for use in all plots. Next, we will create a Cloropleth map and add a fill aesthetic that corresponds to the count of charging stations for each state. We will also make cloropleth maps for station density per unit area and station density per person. These plots will allow us to see which states have more total alternative charging stations, which states have more per person, and which have more per unit area. We will then create geospatial plots of the 5 most common alternative fuel stations in the lower 48 states and color by type. These plots will allow us to see which alternative fuel technologies are used in the different regions of the US.
