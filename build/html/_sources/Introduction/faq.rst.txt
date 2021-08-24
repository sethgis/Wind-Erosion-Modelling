Frequently asked questions
====================================================

This page lists some Frequently Asked Questions (FAQs) for the TrofMIS web service.

Installation and use of TrofMIS Service
___________________________________________

The TroFMIS service will be a hosted service where all users will access via the internet.
There is no special needs to install the service, a user with internet access and the address will be able to use the service.
However, for the user to access other types of analysis, the user will need to have a working email address, to receive
alerts on the monitoring aspect of the forest of interest.

Will I be able to download the outputs from the system? How will I visualize the outputs?
------------------------------------------------------------------------------------------------------------------------------------

The system will allow download of the visualised products in different formats inluding .png or .tiff files as well as statistics in form of 
.csv format for use.
These downloaded datasets could be visualised usig different formats inluding for .csv using microsoft excel file, for .tiff files, the 
output can be visualised through any GIS based software (ArcGIS or Quantum- GIS) with the latter being open source that can be downloded 
`HERE <https://qgis.org/en/site/forusers/download.html>`_

Do I need to download a 32-bit or 64 bit version of QGIS?
------------------------------------------------------------------

Any version of the software download is capable of handling and visualising the .tiff files downloaded from the system. 


System Usage
___________________________________________
Will I be able to use the system if I am not registred?
------------------------------------------------------------------
The system is accessible to anyone, in moreso visualising the various Forest products
such as Forest Canopy and Forest change, but you will not be able to use additional services such as forest 
alerts subscription to receive alerts. We reccomend that the end users register as users in order to 
access the full functionality of the system.


Datasets
___________________________________________
When will you update datasets for the current year?
------------------------------------------------------------------
TrofMIS system products are annual products and will be updated annually for the end users to 
access the output. However, the Forest alerts are automatically uupdated upon generation of new datasets
by the source providers.

Is there an option to download the original data?
------------------------------------------------------------------

Users can download the original data using the Download option within the 
toolbox.

Will the toolbox support higher resolution datasets?
------------------------------------------------------------------

The toolbox currently supports LANDSAT 7 (30m) and Sentinel 2 (10m) data for primary 
forest products computations. However, based on the later versions, the system is capable of handling any course or finer 
resolution data, based on the products generated in future.

Methods
___________________________________________

How was the default time period for the analysis determined?
------------------------------------------------------------------

The default time period of analysis is from years 2000 to Current year(2020). These were also based on reccomendation generated from 
the `Good Practice Guidelines REDD+ Reporting
<https://unfccc.int/topics/land-use/resources/redd-documents>`_

The moniroing period was fixed at one year interval in the precomputed layers such as the forest canopy and forest change. While the forest degradation is 
in 2 levels:
	- Annual Change
	- Change from Reference year 2016 
The forest alerts is computed using short terms monitoring timeline i.e Fortnight monitoring to inform on the short term degradation
and progressive loss of forest quality in the forest of ineterest.

Forest Canopy
------------------------------------------------------------------
What is considered a forest?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
The system considers areas that lie between the Dense, Moderate and the Open Canopy as forest.

How are the Forest Canopy Results Interpreted?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
The forest canopy with the four classes, outlines the regions with most canopy
progressively reducing to open canopy, where we have very few trees.
The rest of the Non Forest Class are considered areas with no Forest cover and may include 
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

How will the user receive the outputs?
---------------------------------------------------------------------------
The user, after subscription to the watchlist, will recieve output notification in their respective emails thus the need to have 
a working email and register for alerts.
Based on the user slected variables, the results will compute using those input variable and provide notification to the user via
an email.



.. toctree::
   :maxdepth: 3