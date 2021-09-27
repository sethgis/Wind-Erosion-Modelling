Frequently Asked Questions (FAQ)
====================================================

This page lists some Frequently Asked Questions (FAQs) for TroFMIS .

Installation and use of TroFMIS Service
___________________________________________

TroFMIS service is a hosted service where all users can access via the internet.
There is no special need to install the service, a user with internet access and the address will be able to use the service.
However, for the user to access other types of analysis such as forest surveillance, the user will need to have a working email address, to receive
alerts on the monitoring aspect of the forest of interest. however, the user can also detect forest disturbance based on their defined dates.

Will I be able to download the outputs from the system? How will I visualize the outputs?
------------------------------------------------------------------------------------------------------------------------------------

The system will allow download of the visualised products in different formats inluding .png & .tiff files as well as statistics in form of 
.csv format for further use.
The downloaded products can be visualised using different formats including microsoft excel software, and .tiff files, the 
output can be visualised in any GIS based software (ArcGIS or Quantum- GIS) with the latter being open source  
`HERE <https://qgis.org/en/site/forusers/download.html>`_.

Do I need to download a 32-bit or 64 bit version of QGIS?
------------------------------------------------------------------

Any version of the software downloaded is capable of handling and visualising the .tiff files downloaded from the system. 


System Usage
___________________________________________
Will I be able to use the system if I am not registred?
------------------------------------------------------------------
The system is accessible to anyone to visualise the Forest products, however, to get the full system functionalities such as forest surveilance using Sentinel 1 - Radar imageries, 
a user will be required to register and log in to the system. For user alerts on forest disturbances, a user will be required to subscribe for such services in the system. 

.. note::
   We reccomend that users register and log in on the TroFMIS system before performing and form of analysis in order to access the full functionality of the system.  
  
Datasets
___________________________________________
When will you update datasets for the current year?
------------------------------------------------------------------
TroFMIS system products are annual products and will be updated annually for the end users to 
access them. However, the Forest surveilance can be done on the fly, monthly or fortnightly.

Is there an option to download the original data?
------------------------------------------------------------------

Users can download the original data using the Download option within the TroFMIS
toolboxes.

Will the toolbox support higher resolution datasets?
------------------------------------------------------------------

The toolbox currently supports LANDSAT datasets with a resolution of 30 meter and Sentinel 2 images with 10 meter resolution, data for primary 
forest products generation. 
However, based on the later versions, the system is capable of handling any type of higher resolution raster dataset.

Methods
___________________________________________

How was the default time period for the analysis determined?
------------------------------------------------------------------

The default time period of analysis is from years 1990 to Current year (2020). This was based on reccomendation generated from 
the `Good Practice Guidelines for REDD+ Reporting
<https://unfccc.int/topics/land-use/resources/redd-documents>`_

The moniroing period was fixed at one year interval in the forest product layers such as the forest canopy densities and forest canopy changes. 

Forest Canopy
------------------------------------------------------------------
What is considered a forest?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
The system considers areas that lie between the Dense, Moderate and the Open Canopies as forest,
while the Non - Forest are the areas that exist outside the three classes.

How are the Forest Canopy Results Interpreted?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
The forest canopy densities with the four classes, outlines the regions with most canopy
progressively reducing to open canopy, where we have fewer trees.
The rest, i.e Non Forest Class are considered areas with no forest cover and may include 
shrublands, grassland, mooreland, rocks and bareland.
 

Canopy Disturbance
------------------------------------------------------------------

What is the Canopy Disturbance product?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
The canopy disturbance products highlights the areas that have remained stable, or gained in terms of quality of canopy.
The loss highlights areas that have lost quality in terms of canopy cover, dropping from Dense to the next class.
The disturbed areas may also inlude the forested zones that have changed to non forest areas.


Carbon Emmission
------------------------------------------------------------------

What is the product Carbon Emmission?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
This product is generated form layers that is classified into 2, showing the areas that are Forest and Non forest.
The products highlights areas that were previously a different class that have either gained to be forest, or have completely lost
tree cover to become non forested areas.
The non forested areas signifies the deforestation that has occurred within the analysis period.

Forest Alerts
________________________

How will the user receive the alerts?
---------------------------------------------------------------------------
The user, after subscription to the watchlist, will receive notification in their respective emails thus the need to have 
a working email and register as a user in TroFMIS.



.. toctree::
   :maxdepth: 3
