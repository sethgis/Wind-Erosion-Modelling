.. figure:: ../_static/Images/wind.PNG



***************************************************
Climate Erosivity Factor (CE)
***************************************************
Climate Erosivity is the ability of climatic condition in a particular area to yield an environment conducive for wind erosion. For wind erosion to occur: Threshold velocity of the wind must be attained to initiate particle movement. Soil particle size, shape, weight and mutual adherence of the particles, must be favorable. Soil surface must have minimal surface barrier that can stop movement of soil particles

Normally, the variables that are inplay, varies from climatic variables such as wind speed, potential evapotranspiration, rainfal amount, all being a fctor of time.  

Climate Erosivity is computed with the variables as represented in the equation below. The variables are described in the following sections below.

.. figure:: ../_static/Images/CE.PNG

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
the complexities of rescaling their values to meteorological
tested ranges as applied by (Fryrear et al., 1998). 


    


  
.. figure:: ../_static/Images/wind.PNG
  


.. toctree::
   :maxdepth: 3



