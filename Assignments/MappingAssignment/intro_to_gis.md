# Intro to GIS


## The general idea

The way to think about GIS is that it's data that understands space. I understands where it is, what it's next to, and how far it's away from things. And you can query that data. And you can make it visual. 

## Data types

There are several data types in GIS. The major ones that you will work with are:

1. Vector layers. These are the most common. They are maps, like roads or county boundaries or state boundaries. 
2. Raster layers. These are things like satellite images, or data inferred from remotely sensed images, like land cover maps. 
3. Geodatabase layers. More common now, they are geographic data stored in a special database that understands space. 
4. Non-geographic data layers. These are things like CSVs that you import and join to a spatial layer.

## Selecting by attributes

1. Download a national county boundary file. [Counties of the U.S.](ftp://ftp2.census.gov/geo/tiger/TIGER2015/COUNTY/)
2. Open it. Let's explore it. 
3. Layer > Open Attribute Table
4. Select features by using an expression (STATEFP=31)
5. Save As and be sure to only save selected features. 

## Joining data to a map 

1. Open your Nebraska Map. (Add Vector Layer)
2. Download a data file I have created of [population change in Nebraska counties from 2010-2014](https://www.dropbox.com/s/o771pbmpzvt18ra/countymap.csv?dl=0). 
3. Open a text editor to create a CSVT file. You *MUST* name that file *EXACTLY* the same thing as the csv file, just with a .csvt extension. And you *MUST* save it in the same place as the csv file. 
4. Add the CSV to the map (Add Delimited Text Layer) and remember to click No Geometry.
5. Right click or control click or go to Layer > Properties
6. Click on Joins.
7. Add a join. 
8. Set the Join Field and the Target Field to GEOID and click OK. 
9. Go to Style. Change Single Symbol to Graduated and the field to countymap_change1014.

## Thematic shading

Questions about thematic shading?

1. What are we trying to accomplish with a thematic shading?
2. What concerns should we have?
3. What colors should we use?
4. How do we decide where to set break points?

## Assignment

Create a map of population change in Nebraska using this data. Thematically shade it in a manner you think is appropriate. Write a paragraph discussing what the map shows, as if this paragraph were going to be published in a story about population change in Nebraska after a Census data release. 

To get the points for the assignment, you must submit to Blackboard:

1. An image of your map (Project > Save as Image). 
2. The paragraph of discussion.

[Some help here](http://www.qgistutorials.com/en/docs/performing_table_joins.html). 