# Using the 3D BAG in Python

In this workshop we are going to walk you through the details of the 3D BAG data set, which is a collection of 3D building models at multiple levels of detail for the Netherlands. See https://3dbag.nl. We will introduce the data set, discussing the data model, available formats, data quality and some of the peculiarities. In the hands-on part of the session, we will show how you can make the most out of the data by using Python, whether you integrate with other services or use it directly for analysis. In this part we will focus on CityJSON (http://www.cityjson.org) and cjio (https://github.com/cityjson/cjio), but we will also show other tools that can be helpful for working with the data.

## Installing the dependencies

**Python version:** 3.6 or above. We used Python 3.8 for developing these materials.

### With conda

Probably the easiest if you install the dependencies with `conda`. See how to [install conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/)

Create a new conda environment and set install the dependencies from the `environment.yml` file.

`conda env create --name foss4gnl_3dbag --file environment.yml`

### Not using conda

You can also set up everything if you cannot or don't want to use conda. In this case, install the dependencies manually with `pip`. The dependencies are listed in the `environment.yml` file.

## Workshop outline

1. Introductions
2. 3D BAG schema ([intro.ipynb](intro.ipynb))
   1. Data layers
   2. Identifiers
3. CityJSON introduction ([intro.ipynb](intro.ipynb))
   1. General schema
   2. Geometry representations, depth of arrays
   3. Semantic Objects
   4. Transformation
4. Get 2D layers for your AOI through WFS
   1. Draw your Area Of Interest in QGIS
   2. In QGIS
   3. In Python ([wfs.ipynb](wfs.ipynb))
5. Basics of CityJSON in Python ([basics.ipynb](basics.ipynb))
   1. cjio CLI
   2. CityJSON with standard libraries
   3. cjio API intro
6. Get a citymodel for your area of interest ([download.ipynb](download.ipynb))
   1. Get the tile ID-s within a WKT polygon
   2. Download the tiles
   3. Merge the tiles
   4. Subset with the AOI
   5. Write result
7. Assign addresses to CityObjects ([addresses.ipynb](addresses.ipynb))
   1. Access the BAG API
   2. Get addresses for each CityObject
   3. Write addresses to attributes
8. Create new semantic surfaces ([semantics.ipynb](semantics.ipynb))
   1. Explain the semantic surface access and indexing works in the API
   2. Create new semantic surfaces per surface orentation
   3. Assign semantics to the geometry and the citymodel
9. Wrap up and summarise the learnings
10. Individual work
