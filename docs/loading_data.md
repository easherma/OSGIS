# Loading Data Overview

## File Formats

### Open Source Flexibility

QGIS is very flexible with file formats, which is a wonderful thing given the wide variety of spatial data formats you'll come across.

Most, if not all, of QGIS's functionality regarding file formats is thanks to [GDAL/OGR](http://www.gdal.org/). Thanks, [OSGeo](http://www.osgeo.org/)!

## Crusin' for Files (Before Ye Fetch, Ye Must Find)

Clearly, the first thing you need to do before loading data is find it. As we talk about in customizing the UI, there are often multiple ways to do similar things in QGIS. You can browser for data using the browser panel inside QGIS, or you can use your operating system to find a file (which you are probably already comfortable with) and drag it into the Layers panel. There are some slight differences between the two, which aren't worth getting into here. For the vast majority of the cases, either way will work.

### To use the file browser panel or not to use the file browser panel...
Do this whichever way you'd like. Personally, I'd disable the Browser Panel to free up that space inside the QGIS GUI becuase I like seeing every inch of the beautiful maps I make. ;-)

![Browser](.\images\browser.png)
*You can find and add data using the browser panel in QGIS or by dragging files from your operating system*


## Adding Layers

You can also add layers using the 'Manage Toolbar Layers' toolbar or under the Layer menu.

![Browser](.\images\AddLayer.png)

### These all do the same thing

![Browser](.\images\AddVector.png) **=** ![Browser](.\images\AddVector2.png) **=**

![Browser](.\video\vectorAdd.gif)


## Connect to DB

Special case, either talk about it here or just link to seperate section.

## Spatial Indexing
Clicking on "Use spatial index" allows for faster referencing of layer
contents




## Specify Your CRS ASAP
After adding CSV, need to specify a Coordinate Reference System (or
"CRS") in the "Coordinate Reference System Selector"

We picked "WGS 84/4326" which is the most commonly used Geographic
Coordinate SystemGeographic

This window tracks recent reference systems (and there are only so many
that you'll typically use if you're focused on a specific geography)

Can see the definition of the CRS in the very bottom field to compare different
