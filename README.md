# MIT-Seds-2022
Materials for TAing Sedimentology in the Field, Spring 2022

## Macrostrat burial history instructions
*The goal of this project is to construct a time-Temperature path for the Manlius Formation that we measured at sections CV and J during the field trip. We will then use this t-T path to predict the clumped isotope (<img src="https://render.githubusercontent.com/render/math?math= \Delta_{47}">) temperatures we should measure if these rocks were affected only by solid state reordering.*  

First, **determine the spatial extents of the Helderberg Group and Manlius Formation**. (*How does the lithology of the Helderberg Group change across its geographic extent? Why is the spatial extent of the Manlius Formation < the spatial extent of the Helderberg Group?"*) 

To see spatial extents, navigate to [macrostrat.org](url) and search "Helderberg" or "Manlius" in either the "Map" or "Search" functions. (Example: https://macrostrat.org/sift/#/strat_name_concept/2030)

A note about Macrostrat terminology: the "Manlius Formation" in Macrostrat is best represented as a set of 'units,' which are the expression of the Manlius Formation in one 'column' (the columns are the polygons you see in map view). To see all of the units included in the Manlius Formation in the API, you'd use these search terms: https://macrostrat.org/api/units?strat_name=Manlius. To access lithological data about just *one* of the Manlius units in Macrostrat, you can zoom-in on a unit by searching by unit_id: https://macrostrat.org/api/units?unit_id=8448&response=long. (Adding "response=long" makes sure you're retreiving all information possible!)

Next, you'll need to **determine what rocks were deposited on top of the Manlius Formation, when**. You can see this schematically on each column's webpage (e.g., https://macrostrat.org/sift/#/column/313), but you will need the detail provided via the Macrostrat API to construct a time-temperature path. Access more information about each column's units via searches like: https://macrostrat.org/api/units?col_id=313. (You can then follow up on each unit via the 'units' route. For example, the youngest unit in column 313 is the Slide Mountain Formation (unit_id = 8514), which you can see in more detail here: https://macrostrat.org/api/units?unit_id=8514&response=long.)

Now, **construct a table** containing data about all units overlying the Helderberg Group, which will be necessary for plotting the Helderberg Group's burial history. (You can work whichever direction in time feels right to you.)

| age (top) | age (bottom) | (Overyling) formation name | Formation thickness (NY) | [optional: Fm. thick. elsewhere] |
|-----------|--------------|----------------------------|--------------------------|----------------------------------|
| 325 Ma    | 333 Ma       | EXAMPLE FORMATION          | 125 m                    | 350m (PA, WV)                    |
| ...       | ...          | ......                     | ...                      | ...                              |


**TIPS**
- To complete your table, you will need to explore multiple columns that contain the Helderberg Group.  
- You can export a .csv file from the Macrostrat API by adding "&format=csv" to the end of any of the web addresses linked above.    
- Go wild on the Macrostrat API! Reading the links I've provided above will give you some clues about how the API commands work. 


Finally, use the data from your completed table to fill in the Helderberg Group's burial history^ as best you can (with the information you have). We will turn to the literature to help fill in the blanks during class in a few weeks.

^Plot time [Myr] on the horizontal axis with 419 Ma on the far left, and plot the depth of the Manlius Fm./thickness of overlying units [m] on the y-axis.



## Blimp processing instructions
*coming soon*
