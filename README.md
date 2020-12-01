# GrassCast_DB
Github account for GrassCast DB. Data also found at https://data.nal.usda.gov/dataset/grasscast-database. 
Temporary info also found at https://globalviz-chrisdorich.shinyapps.io/grasscast_shiny/ where updates on the data and methods can be found. This website will be brought down in the future though. 


GrassCast_Global_prep.Rmd is the final preparation script. It utilizes the below scripts to combine the data into a working environment. 
  * GrassCast_cattleweight.Rmd - for procesing cattle weight gain data (and NPP data for those sites).       
  * GrassCast_NDVI_climate.Rmd - for processing NDVI and climate data for sites.     
  * GrassCast_NPP.Rmd - for processing Annual aboveground net primary productivity (ANPP) data. There are subscripts for the site level within this, below:     
    * Jornada.Rmd
    * ReynoldsCreek.Rmd 
    * Konza.Rmd 
    * sevilleta.Rmd
    * Navajo.Rmd 
    * Torell.Rmd 
    * Nebraksa_sandhills.Rmd  
    
Output excel files: 
These are the files that can be downloaded as part of the database. Also found at data.nal.usda.gov/dataset/grasscast-database. 
The database can also be directly loaded into R as the data is processed and saved in RData files. More info on those access R scripts and the R shiny app will come later.        
  * GrassCast_Database_v1.xls - excel sheet that outlines basic sites level information and provies a list of availables sites in version 1 of the database.   
  
 The resulting/processed datasets themselves are: 
 (format is the first tab being 'readme' that gives metadata, second tab reflecting the data)
  * ANPP_metadata.xls - annual aboveground net primary productivity (ANPP) data
  * ANPP_raw.xls - Temporal biomass measurements that are part of ANPP data sets 
  * Functional.xls - Species or plant functional group level datasets that comprise NPP. 
  * WeightGain.xls - Cattle weight gain data from grazing experiments. 
  * NDVI.xls - MODIS and AVHRR cumulative growing season NDVI value for sites in the database. 
  * NDVI_raw.xls - MODIS AND AVHRR temporal NDVI values for sites in the database. 
           
           
-Chris Dorich       
chris.dorich@colostate.edu 

