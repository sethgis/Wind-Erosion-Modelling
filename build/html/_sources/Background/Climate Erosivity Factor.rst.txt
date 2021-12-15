.. figure:: ../_static/Images/wind.png



***************************************************
Climate Erosivity Factor (CE)
***************************************************
The FCD product in specified forests are generated using the Forest Canopy Density Model (FCD algorithm), as applied by (Rikimaru, et al, 2002). 
TroFMIS approach made slight modification to the original FCD technique, by excluding Principal Component Analysis (PCA),
which is computational intensive over large areas, or when computed using high resolution data. 
The modified FCD approach can be expressed as:

.. figure:: ../_static/Images/CE.png

Where: 
  - U is mean wind speed (m/s) at 2-10 m height in 
  - PETi is mean potential evapotranspiration 
  - Pi	is precipitation (mm) 
  - di	is the total number of days’ observation was made

Wind speed U and soil moisture (PET and P) 
are directly proportional to climatic erosivity while 
(PET) is inversely proportional to the climatic erosivity. 
When the PET is greater than the precipitation the moisture is 
removed from the soil, the adhesive force reduces, as a result 
the weight reduces making the particle susceptible to detachment 
and transportation by wind. 
When the Precipitation is higher than the evapotranspiration, 
the water is absorbed by soil particles, the particles 
increases in weight due to mutual adherence to surrounding particles, 
as a result the soil particles are less susceptible to detachment  and 
transportation by wind.

  Note: 

The value ranges of the above parameters should be meaningful; 
it is recommended the values are rescaled to fit in 
within the meteorological known values for each 
particular datasets; because the remotely acquired 
datasets may not necessarily come with the expected value ranges. 
However, for generating a 
sensitivity map, the final CE will be fuzzified by a linear function to yield 
values that are between 0 and 1 scale. Fuzzification saves a user 
the complexities of rescaling their values to laboratory 
tested ranges as applied by (Fryrear et al., 1998). 


    


  
.. figure:: ../_static/Images/wind.png  
  


.. toctree::
   :maxdepth: 3



