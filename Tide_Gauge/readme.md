#Tide guage stuff
- Contains Get_HC_allstations.m and a .csv template for doing the harmonic decomposition of tide guage time series data (setup to perform on the data from UHSLC) 

- Contains kml2csv_tides.m to convert a .kml file of the tide gauge names and locations into a table that you can readily copy into the fort.15 for ADCIRC. The script is is also capable of getting the boundaries of the mesh (both external and internal, need to use the extdom .m files from the Distmesh folder) and only extracting the stations which lie within the bounds of the mesh. The kml can been exported from a Google map. The database created by William Pringle can be found at: https://www.google.com/maps/d/u/0/edit?hl=en&authuser=0&mid=1yvnYoLUFS9kcB5LnJEdyxk2qz6g&ll=-8.356587969923837%2C89.57681401715104&z=4

- Contains Station_harmonic_compare.m to get the timeseries of the output fort.61.nc from ADCIRC at station locations, perform the harmonic decomposition and compare with the observed harmonic constituents producing a scatter plots of errors and the total complex RMS. Very gappy fort.61.nc data is automatically ignored and somewhat gappy data can be processed by Utide OK. 
