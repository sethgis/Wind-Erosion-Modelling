
***************************************************
Forest Carbon Flux (Carbon Emmission)
***************************************************
The FCD products are reclassified into majorly 2 classes annually. The classified product (Forest and Non Forest areas) are then computed for difference (Deforestation or afforestation) between the two time periods. 
Carbon fluxes provide information on estimates of carbon transferred from the above ground pool to the atmosphere or the reverse (sequestration) when afforestation/reforestation occurs
The above ground biomass (AGB) stocks in the Tropical Forests of the IGAD region are estimated based on the 2006 IPCC guidelines (Table 4.7 of Chapter 4 Forestland) for Tropical rainforests which estimates AGB at 310 Mg Biomass/ha. Using the methodological guidelines from IPCC, this is converted to 145.7 Mg Carbon/ha (A carbon factor of 0.47 is used) and translates to 534 Mg CO2eq/ha (the molecular formula of CO2 is used). Based on the above Emission Factor, and the deforested forest areas (Activity Data) between two time intervals, Emission estimates (E) are computed as shown in the formula below.

.. math::
 E=AD*EF	 
 :label: eq_d

With AD being the change of forest caover in hectares (Deforestation - AD) and the reference value of 
carbon stock density per hectare in tropical forests (EF – Reference Value (Integer)).

The forest change was computed from the binary class of forest and non-forest zones, where the system computed the difference between the Analysis period, which and the reference year 2016. The reference year was constant as compared to the forest change where the reference year was changing from year to year as shown in the figure below.

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

    Carbon Emission computation procedure


.. toctree::
   :maxdepth: 3
   
