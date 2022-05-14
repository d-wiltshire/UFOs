# UFOs

## Overview

The goal of this challenge was to create a "UFO Sightings" webpage (using HTML, Bootstrap, and JavaScript) that would be able to receive user input and use it to filter a large dataset of reported UFO sightings. The dataset contains reported UFO sighting information including 1) the date of the sighting, 2) the location of the sighting (city, state, and country), 3) the shape of the object seen in the sky, 4) the duration of the object's appearance, and 5) additional comments. The desired filters for the dataset include: 1) date of the sighting, 2) location city, 3) location state, 4) location country, and 5) shape of the object. 


## Results

Using the search criteria to filter is a straightforward process. The user can input information into any (or all) of the available filters in order to filter the complete dataset by those criteria. The page will update when the user presses Enter. 

For example, filtering by "ca" to find reports from California filters the dataset only by state:

![Mod 11 CA](https://user-images.githubusercontent.com/100863488/168443496-aff13e96-1138-44a0-9bd8-9ee4561d1bb0.png)

We can also add "light" to the "shape" filter to find reports from California that listed the object's shape as "light":

![Mod 11 CA and light](https://user-images.githubusercontent.com/100863488/168443497-a90ce72e-97f7-4c9d-8a44-5d84273f0d53.png)



## Summary

The webpage functions as intended to filter the dataset by the desired filters. However, its function could be improved to help the user navigate the page and understand the context of the filter results.

### Drawbacks of the current version

* The user does not know (except by browsing the complete dataset) which cities, states, shapes, etc. it is possible to filter by. If possible, it would be ideal to include a list of options under each filter (perhaps hidden until the user reveals them) so that the user can see what search options there are. Visualizations (for example, a heatmap) would also help the user understand trends.
* The current version of these filters are case-sensitive, and the user must type search criteria in all lowercase. 

### Recommendations for further development

* Since the current version of this filter is case-sensitive, and all information in the data.js file is in lowercase text, we should add code in the app.js file to convert any user input to lowercase text in order to match the lowercase data.
* It would be helpful to add groupings information or visualizations that would help the user see trends (for example, a timeline that might show clusters of reports). 
* It would be helpful to add a filter based on keywords in the reported comments.
