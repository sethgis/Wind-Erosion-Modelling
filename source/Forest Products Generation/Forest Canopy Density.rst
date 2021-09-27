.. figure:: ../_static/Images/trofmis.png
    :width: 300
    :align: center
    :height: 400
    :alt: service schema
    :figclass: align-center


***************************************************
Forest Canopy Density (FCD)
***************************************************
The FCD products in specified forests were generated using the Forest Canopy Density Model (FCD algorithm), as applied by (Rikimaru, et al, 2002). 
Our approach made slight modification to the original FCD technique by excluding Principal Component Analysis (PCA),
which is computational intensive over large areas, or when done using high resolution data. 
The modified FCD approach can be expressed as:

.. math::

 FCD=√(AVI×SSI+1)-1 
 :label: eq_a


Where, the Advanced Vegetation Index (AVI), like many vegetation index, gives precedence to the areas with healthier vegetation as
compraed to the areas with scarce or novegetation. The AVI was computed as shown in the equation below.

.. math::

 AVI =  ((NIR+1)*(65536 -Red))*1/3
 :label: AVI model



The AVI was directly fused with Scaled Shadow Index (SSI), to yield the ultimate forest canopy densities.
i.e. areas with canopy cover while segregating areas with very little or no vegetation. 
SSI applied the numerical intergration of Blue and Green bands to identify shadow covered areas as shown in the equation below.

.. math::
 SSI=(256-Blue)*(256-Green)*(256-Red)/3
 :label: SSI model	
	
The image summarises the steps of generating FCD prodct uisng earth observation methods.

.. figure:: ../_static/Images/fcd_image.png
    :width: 300
    :align: center
    :height: 400
    :alt: service schema
    :figclass: align-center

    FCD computation summary.



FCD Data Encoding
=============================
The ultimate output of the FCD product was rescaled to percentage, using a linear regression modell.
The values were later reclassified into various Forest Canopy classes.
The percentage output values of this equation geovisualised areas of Dense Canopy, Moderate Canopy 
and Open Canopy between 100 to 65, 65 to 45, 45 to 30 respectively, while 
the Non- Forest areas were capped at below 30 percent as shown in the table below.

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
    :width: 350
    :align: center
    :height: 250
    :alt: service schema
    :figclass: align-center

    FCD computation summary.

.. toctree::
   :maxdepth: 3



