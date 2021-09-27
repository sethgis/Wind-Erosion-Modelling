
***************************************************
Forest Carbon Flux (Carbon Emission)
***************************************************
The FCD products are reclassified into majorly 2 classes. The classified products (Forest and Non Forest areas) are then used to compute the difference, and highlight areas that deforestation or regrowth has taken place, this product is what is reffered to as carbon flux product in TroFMIS. 
Carbon flux product provides information on estimated carbon transferred from the above ground pool to the atmosphere, or the vice versa (sequestration) when afforestation/reforestation occurs.
The above ground biomass (AGB) stocks in the Tropical Forests of the IGAD region, are estimated based on the 2006 IPCC guidelines. For Tropical rain forests, the AGB is estimated at 310 Mg Biomass/ha. 
Using the methodological guidelines from IPCC, this is converted to 145.7 Mg Carbon/ha (A carbon factor of 0.47 is used) and translated to 534 Mg CO2eq/ha 
(the molecular formula of CO2 is used). 
Based on the above Emission Factor, and the deforested forest areas (Activity Data), between two time intervals, Emission estimates (E) are computed as shown in the formula below.

.. math::
 E = AD*EF	 
 :label: Carbon Emission Equation

With AD being the change of forest cover in hectares (Deforestation - AD) and the reference value of 
carbon stock density per hectare in tropical forests (EF – Reference Value (Integer)).

The carbon flux was computed from the binary class of forest and non-forest class, where the difference between the Analysis period, and the reference year 2016 was generated, as is shown in the table below.

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

To compute the carbon flux, please consider the method below
Class	Pixel Count

  - Stable	11143909						
  - Loss	391764						
  - Gain	173370						
							
Surpose you get the pixel count as above, go ahead and calculate the net changes							
							
Net Changes	Gain - Loss						
Net Change	173370					
																		
After Getting the Net Change, some conditions have to be met							
							
   - Condition 1	If the change is positive (+), then there was carbon enhancement						
   - If the change is negative (-), then there is carbon loss						
   - Get the carbon flux (emmission) by first transforming the Net Change to heactares, and then multiply by 145.7							
							
Net Change (Ha)	1722.7					
							
   - Carbon Emmission	250997.39	C\Mg\ha		year = 2019 	

The figure below summarises the steps of computing the carbon flux in TroFMIS.


.. figure:: ../_static/Images/Canopy_Disturbance.png
    :width: 351
    :align: center
    :height: 300
    :alt: service schema
    :figclass: align-center

    Summary of Carbon flux computation.
    
.. figure:: ../_static/Images/trofmis3.png  
    
.. toctree::
   :maxdepth: 3
   
