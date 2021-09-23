========================
Data Source
========================

The data needs assessment outlined all the data needed for generation of the forest products,
which entailed the proposed REDD+ models to achieve the envisioned forest products and statistical information.
The models specifications are outlined in the objectives section. 
For their successive computation and analysis, the data needs assessed were as shown in the table below.

-------------------------------------------------------
Data Source
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
    The `Natural Earth Administrative Boundaries`_ provided in TrofMIS  
    are in the `public domain`_. The boundaries and names used, and the 
    designations used, in TrofMIS - IGAD Region do not imply official endorsement or 
    acceptance ICPAC or its implemeting patners, organisation and contributors.

    If using TrofMIS for official purposes, it is recommended that users 
    choose an official boundary provided by the designated office of their 
    country.

.. _Natural Earth Administrative Boundaries: http://www.naturalearthdata.com

.. _Public Domain: https://creativecommons.org/publicdomain/zero/1.0

-------------------------------------------------------
Forest Product Coding
-------------------------------------------------------
The generated forest products included:
	- Forest Canopy Map
	- Forest Change Map
	- Forest Disturbance Map
	- Forest Carbon Flux Map

Were generated automatically in Google earth engine as highlighted in the methodology section.
These products are in GeoTiff format, and have a range of values for classification. 
These range of values were considered as the data coding values used to classify the outputs for visualisation
as shown in the table below.


Forest Canopy
-------------------------------------------------------
+------------------+-----------+---------+
| Sensor/Dataset   | Min (%)   | Max (%) | 
+==================+===========+=========+
| Non Forest       | 0         | 30      | 
+------------------+-----------+---------+
| Open Canopy      | 30        | 45      | 
+------------------+-----------+---------+
| Moderate Canopy  | 45        | 65      | 
+------------------+-----------+---------+
| Dense Canopy     | 65        | 100     | 
+------------------+-----------+---------+


Forest Change
-------------------------------------------------------
+------------------+-----------+---------+
| Sensor/Dataset   | Min       | Max     | 
+==================+===========+=========+
| Stable           | 1         | 1       | 
+------------------+-----------+---------+
| Gain             | 2         | 2       | 
+------------------+-----------+---------+
| Loss             | 3         | 3       | 
+------------------+-----------+---------+



Carbon Flux
-----------------------------------------
A multi band raster form 2016 - 2020, coded as:
+------------------+-----------+---------+
| Sensor/Dataset   | Min       | Max     | 
+==================+===========+=========+
| Stable           | 1         | 1       | 
+------------------+-----------+---------+
| Gain             | 2         | 2       | 
+------------------+-----------+---------+
| Loss             | 3         | 3       | 
+------------------+-----------+---------+



Forest Alerts
-------------------------------------------------------
+------------------+-----------+---------+
| Sensor/Dataset   | Min       | Max     | 
+==================+===========+=========+
| Loss             | 0.5 ha    | Inf     | 
+------------------+-----------+---------+
| Gain             | - 0.5 ha  | Inf     | 
+------------------+-----------+---------+

