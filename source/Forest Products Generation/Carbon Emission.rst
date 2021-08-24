
***************************************************
Forest Carbon Flux (Carbon Emmission)
***************************************************
Carbon flux estimates the amount 
of carbon transferred from one 
carbon pool(forest) to another 
(atmosphere) in 
density per unit area per year. 
Ideally, Tropical forests acts as carbon sinks with forest cover reduction/emissions 
potentially contributing to exponential global warming. Based on the changes in forest cover (above biomass), there is 
a significant amount of carbon released in the atmosphere.
 
The above ground biomass is estimated at 310 Mg Biomass/ha. This is about 145.7 Mg Carbon/ha and translates to
about 534 Mg CO2eq/ha. This is based on 2006 IPCC guidelines. 

Based on the above estimations, the deforested forest areas are computed per hectare annually, and then multiplied ny the 
estmated carbon density value as shown in the fomular below.

.. math::
 E=AD*EF	 
 :label: eq_d

With AD being the change of forest caover in hectares (Deforestation - AD) and the reference value of 
carbon stock density per hectare in tropical forests (EF – Reference Value (Integer)).

The FCD products are reclassified into majorly 2 classes annually.
The classified product (Forest and Non Forest areas) are then computed for difference between the 2.
The difference is tranlated into loss per hectare per year, to generate the amount of carbon flux in a specific years.
The figure below shows the classification table for the FCD products.

+------------------+-----------+---------+---------------+
| Sensor/Dataset   | Min       | Max     |               |  
+==================+===========+=========+===============+
| Non Forest       | 0         | 30      |  Non Forest   |  
+------------------+-----------+---------+---------------+
| Open Canopy      | 30        | 45      |               |  
+------------------+-----------+---------+   Forest      +
| Moderate Canopy  | 45        | 65      |               |  
+------------------+-----------+---------+               +
| Dense Canopy     | 65        | 100     |               |  
+------------------+-----------+---------+---------------+



.. figure:: ../_static/Images/Canopy_Disturbance.png
    :width: 351
    :align: center
    :height: 341
    :alt: service schema
    :figclass: align-center

    Summary of computating Difference between 2 Forest Canopy Products


.. toctree::
   :maxdepth: 3
   
