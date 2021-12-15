.. figure:: ../_static/Images/RC2.png


========================
Data Source
========================

This is the process of acquiring and structuring the raw datasets in a spatial 
format mode in order to take advantage of the visualization and analytical abilities 
of the GIS environment. The raw data sets acquired matched the parameters 
previously as shown in the mathematical algorithms of soil datasets, 
climatic datasets, land cover classes and the vegetation cover factors.
The acquired datasets covered the wind erosion modelling area of 
interest including soil datasets, climatic datasets, 
vegetation cover and land use land cover datasets.

Soil datasets and their source included:
- Sand Sa : `Harmonized World Soil Database <https://data.isric.org/geonetwork/srv/eng/catalog.search#/home/>`_,
- Clay Cl : `Harmonized World Soil Database <https://data.isric.org/geonetwork/srv/eng/catalog.search#/home/>`_,
- Organic content OM : `Harmonized World Soil Database <https://data.isric.org/geonetwork/srv/eng/catalog.search#/home/>`_,
- Calcium carbonate CaCO3 : `Harmonized World Soil Database <https://data.isric.org/geonetwork/srv/eng/catalog.search#/home/>`_,

Climatic factor datasets included:
- Wind speed U between 2 -10-meter height : `Global Wind Atlas <https://globalwindatlas.info/>`_,
- Precipitation, P in mm : `Terra Climatology <https://www.climatologylab.org/terraclimate.html/>`_,
- Potential Evapotranspiration PET : `Terra Climate <https://www.climatologylab.org/terraclimate.html/>`_,

Fractional cover datasets acquired from `Copenicus Proba NDVI data <https://earth.esa.int/eogateway/missions/proba-v>`_,
, for soil roughness, Land cover classes’ from corpenicus data was reclassified and applied in the modelling. 


-------------------------------------------------------
Other Data Sources
-------------------------------------------------------

+------------------+-----------+---------+--------+------------------+
| Sensor/Dataset   | Temporal  | Spatial | Extent | License          |
+==================+===========+=========+========+==================+
| Landsat 4,5,7,8  | 1990-2020 | 30 m    | Global | `Public Domain`_ |
+------------------+-----------+---------+--------+------------------+
| Sentinel 2       | 1990-2020 | 10 m    | Global | `Public Domain`_ |
+------------------+-----------+---------+--------+------------------+
| Sentinel 1       | 1990-2020 | 10 m    | Global | `Public Domain`_ |
+------------------+-----------+---------+--------+------------------+


.. note::
    The `Natural Earth Administrative Boundaries`_ provided in LaSWE  
    are in the `public domain`_. The boundaries and names used, and the 
    designations used, in LaSSWE - do not imply official endorsement or 
    acceptance by RCMRD or its implemeting patners, organisation and contributors.

    If using LaSWE for official purposes, it is recommended that users 
    choose an official boundary provided by the designated office of their 
    country.

.. _Natural Earth Administrative Boundaries: http://www.naturalearthdata.com

.. _Public Domain: https://creativecommons.org/publicdomain/zero/1.0



