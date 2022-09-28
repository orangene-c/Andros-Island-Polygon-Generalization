# Andros-Island-Polygon-Generalization
The primary task for this exercise is generalizing the polygons used to represent a set of islands. The secondary tasks include importing and exporting using ESRI’s proprietary exchange format, converting to geodatabase feature classes, and exploring ArcGIS generalization facilities within ArcGIS Pro. 

This exercise uses ArcGIS generalization tools in both ArcGIS Pro and Jupyter Notebooks. And it consists of discovering the range of generalization utilities available, discerning their differences and evaluating different approaches to line simplification. 

## Part One: Generalization in ArcGIS Pro
1. Obtain the data **andros.e00**
2. Transfer the data from **E00** to a **geodatabase** or **shapefile** by creating a new `Spatial ETL tool`, selecting E00 as the import data format, ESRI shapefile or File Geodatabase as the output format.
3. Simplify the coastline so that it appropriately represents the Andros Islands at a scale of `1:1,500,000`. This operation will probably include some combination of **line simplification**, **polygon removal**, **polygon aggregation**, and it might even include **collapsing polygons into lines**.
4. Export the final generalization products as a file geodatabase in ArcGIS Pro.


## Part Two: Generalization in Jupyter Notebook
Esri provides amazing functionality through their two libraries, `arcpy` and `arcgis`. The `[arcpy](http://pro.arcgis.com/en/pro-app/arcpy/get-started/what-is-arcpy-.htm)` library is proprietary and provides the full suite of functions that exist within ArcPro (or if it doesn't, I haven't found that yet). The `[arcgis](https://developers.arcgis.com/python/)` library provides a subset of that functionality, but is completely free. In this notebook, we will only focus on `arcpy`.

**Objectives in the Jupyter Notebook:**
1. Be able to call functions from arcpy through Jupyter notebook
    - be able to set environment workspace
    - understand arcpy is a library that needs to be imported
    - be able to use help documentation to understand function syntax
2. Reflect on Jupyter; compare and contrast with accessing GIS through Pro