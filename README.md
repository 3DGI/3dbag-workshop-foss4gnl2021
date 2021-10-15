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