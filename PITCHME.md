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
### Coordinate Systems, Datums, and Projections
##### A Review
Coordinate systems define how locations are referenced by their *x*, *y*, and sometimes *z* values in a GIS dataset

![coordsys1](images/coordsys1.jpg)

+++
#### Coordinate Space

The specific *x*, *y* values and their units are known as the **coordinate space**. Could be *arbitrary*, and locally defined, or standardized for cross referencing with other data. 

![arbitrary](images/coordspace.jpg)	![std coords](images/std_coords.jpg)
+++
### Coordinate Systems: Two Types

Coordinate Systems in GIS can be either **unprojected/geographic**, or **projected**...

- Unprojected |
    - Based on spherical coordinates |
	- Units: Degrees of Lat/Long |
- Projected |
    - Mathematical Transformation from sphere @fa[arrow-right] flat surface/plane |
	- 3 dimensional surface @fa[arrow-right] 2D surface
+++
Projected vs Unprojected...

![proj/unproj](images/proj_unproj.jpg)
+++
