
***************************************************
Forest Canopy Density (FCD)
***************************************************
The FCD mapping applied the Forest Canopy Density Model (FCD), to compute and generate the various 
forest canopy densities within the selected forest of interest.
The FCD computation considered the fusion of Advanced Vegetation Index (AVI) and the Scaled Shadow Index (SSI) as hsown in the 
equation below.

.. math::
 FCD=√(AVI×SSI+1)-1 
 :label: eq_a


The Advanced Vegetation Index (AVI), like many vegetation index, gives precendence to the areas with healthier vegetation, with
canopy covered areas geeting high values as compraed to the low vegetation or bare areas. The AVI was computed as shown in teh equation below.

.. math::
 AVI=  ((NIR+1)*(65536 -Red))*1/3
 :label: eq_b



The AVI was directly fused with Scaled Shadow Index (SSI), to yield the ultimate delineation of forested areas
i.e. areas with canopy cover while segregating areas with very little or no vegetation. 
SSI applied the numerical intergration of Blue and Green bands to identify shadow covered areas as shown below before combined to 
the FCD equation Refer to :eq:`eq_a`.


.. math::
 SSI=(256-Blue)*(256-Green)*(256-Red)/3
 :label: eq_c	
	



FCD Data Encoding
=============================
The ultimate output of the FCD as a product was rescaled tp percentage using a linear regression modell.
The values after being transformned into percentage, were reclassified into various Forest Canopy classes.
The percentage output values of this equation geovisualised areas of Dense Canopy, Moderate Canopy 
and Open Canopy between 100 to 65, 65 to 45, 45 to 30 respectively, while 
the non forest areas were capped at below 30 percent as shown in the table below.

+------------------+-----------+---------+
| Sensor/Dataset   | Min       | Max     | 
+==================+===========+=========+
| Non Forest       | 0         | 30      | 
+------------------+-----------+---------+
| Open Canopy      | 30        | 45      | 
+------------------+-----------+---------+
| Moderate Canopy  | 45        | 65      | 
+------------------+-----------+---------+
| Dense Canopy     | 65        | 100     | 
+------------------+-----------+---------+


To compute the FCD output, the figure below summarises the steps applied in the computation.

.. figure:: ../_static/Images/fcd_flowchart.png
    :width: 351
    :align: center
    :height: 341
    :alt: service schema
    :figclass: align-center

    Summary of computation of Forest Canopy Density (FCD)

.. toctree::
   :maxdepth: 3



