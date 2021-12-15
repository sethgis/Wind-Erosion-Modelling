.. figure:: ../_static/Images/wind.PNG



*****************************************************************
Computing Index of Land Susceptibility to Wind Erosion (ILSWE) 
*****************************************************************
To com




ry class of forest and non-forest class, where the difference between the Analysis period, and the reference year 2016 was generated, as is shown in the table below.

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

To compute the carbon flux, please consider the steps as illsutrated below.

* Surpose you get the pixel count as above, go ahead and calculate the net changes

+------------------+-----------+
| Class            |Pixel Count|  
+==================+===========+
| Stable           | 11143909  | 
+------------------+-----------+
| Loss             |391764     |
+------------------+-----------+
| Gain             | 173370    |
+------------------+-----------+					
							
Compte the net change.							
							
Net Changes	Gain - Loss

(173370 subtract 391764)

Net Change	173370					
																		
After Getting the net change, some conditions have to be met							
							
   * If the change is positive (+), then there was carbon enhancement						
   * If the change is negative (-), then there is carbon loss						
   * Get the carbon flux (emmission) by first transforming the Net Change to hectares, and then multiply by 145.7 Mg C/ha							
							
Net Change (Ha)	1722.7					
							
   - Carbon Emmission	250997.39	Mg C/ha	per year	

The figure below summarises the steps of computing the carbon flux in TroFMIS.


.. figure:: ../_static/Images/Canopy_Disturbance.png
    :width: 351
    :align: center
    :height: 300
    :alt: service schema
    :figclass: align-center

    Summary of Carbon flux computation.
    
.. figure:: ../_static/Images/wind.png  
    
.. toctree::
   :maxdepth: 3
   
