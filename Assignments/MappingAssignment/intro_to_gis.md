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

## Thematic shading

## Assignment

[Some help here](http://www.qgistutorials.com/en/docs/performing_table_joins.html). 