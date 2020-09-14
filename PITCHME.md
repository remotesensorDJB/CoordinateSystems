@title[Coordinate Systems in GIS]
Coordinate Systems in GIS
-------------------------------
### @fa[globe fa-5x]

###### Use the space bar to advance the slides
---
### The Plan

- Review of Coordinate Systems, Datums, and Projections
- Projections: Distortion and Compromise
- Projection Selection: Guiding Principles
- Working with Coordinate Systems in ArcGIS Projection
---
#### Coordinate Systems, Datums, and Projections: A Review
Coordinate systems define how locations are referenced by their *x*, *y*, and sometimes *z* values in a GIS dataset

![coordsys1](images/coordsys1.jpg)

+++
#### Coordinate Space

The specific *x*, *y* values and their units are known as the **coordinate space**. Could be *arbitrary*, and locally defined, or standardized for cross referencing with other data. 

![arbitrary](images/coordspace.jpg)
![std coords](images/std_coords.jpg)
+++
#### Coordinate Systems: Two Types

Coordinate Systems in GIS can be either **unprojected/geographic**, or **projected**...

- Unprojected |
    - Based on spherical coordinates |
	- Units: Degrees of Lat/Long |
- Projected |
    - Mathematical Transformation from sphere > flat surface/plane |
	- 3 dimensional surface > 2D surface |
+++
Projected vs Unprojected...

![proj/unproj](images/proj_unproj.jpg)
+++
#### Geographic Coordinate Systems
A **GCS** uses latitude and longitude to store feature locations in *Decimal Degrees*. Location data in *Degrees, Minutes, and Seconds* must be converted, keeping	 at least 5-6 decimal places. 
	
![geog coord](images/geog_coord.jpg)	
+++
#### Datums

A **datum** defines a **spheroid** that is aligned with Earth's shape (the **geoid**). A **local datum** prioritizes best fit for a particular location, while a **geocentric datum** seeks the best fit for all locations. 

![datum](images/datum.jpg)
+++
#### Datums for North America
- Several datums may be used for spatial data in North America...
    - NAD27: North American Datum 1927 - Clarke 1866 spheroid
    - NAD83: North American Datum 1983 - GRS80 spheroid. **Current most popular/default datum**
    - WGS84: World Geodetic Survey 1984 - Geocentric datum. Default for many GPS units.

More: https://desktop.arcgis.com/en/arcmap/latest/map/projections/datums.htm
+++
#### Projections
**Map projections** are complex mathematical models that translate the Earth's curved surface to the flat 2D surface of a paper map. 

Each projection is based on a **datum** and **GCS** that define the shape of the Earth. Different datums/GCSes could result in coordinate shifts
+++
#### Types of projections
Map projections project Earth's surface onto a shape, like a **cylinder**, **cone**, or **plane**. Each shape yields different properties. 

![proj type](images/proj_types.jpg)
+++
#### Tradeoffs...
*All* map projections confer some distortion of one or more of the following properties...

- Direction
- Distance
- Shape
- Area
+++
#### Tradeoffs
*Some* projections preserve certain properties at the expense of others...

- Cylindrical: usually preserve **direction** and **shape** (navigational maps)
- Conic: usually preserve **area** and **distance** (small scale maps)
- Planar: usually preserve **area** and **distance**
+++
![Why All World Maps Are Wrong](https://www.youtube.com/embed/kIID5FDi2JQ)
+++





