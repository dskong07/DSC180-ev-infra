# DSC180-ev-infra

## Note: all datasets are not included for the following code. Acquisition/description of the datasets will either be included or available upon request via email. 

Dataset requirements and instructions for the vehicle data used are also contained within the notebook.
The following notebooks are included, along with the required datasets, sources, and instructions:

-  AFDC_EDA.ipynb, containing AFDC dataset EDA and exploration <br>

    Dataset info:

        AFDC dataset source: https://developer.nrel.gov/docs/transportation/alt-fuel-stations-v1/all/
        Accessing this data requires an API key, which can be acquired at this link:
        https://developer.nrel.gov/docs/
        Additional instructions can be found in notebook.

        The US state geojson data referenced is from the open source mapping api by PublicaMundi. GitHub repo at https://github.com/PublicaMundi/MappingAPI/, with specific data from: https://raw.githubusercontent.com/PublicaMundi/MappingAPI/refs/heads/master/data/geojson/us-states.json

        California State Geoportal Govt Data:
    
        Transmission line data source is: https://gis.data.ca.gov/datasets/CAEnergy::california-electric-transmission-lines-1/about. 
        Zip Code data source is: https://gis.data.ca.gov/datasets/CDEGIS::california-zip-codes/about



-  vehicle_fuel_types_eda.ipynb, vehicle registrations dataset EDA

    Dataset info:

        The vehicle datasets required can be found at the link https://data.ca.gov/dataset/vehicle-fuel-type-count-by-zip-code via the api, or direct download for each individual year. 
        These datasets can be downloaded via API call or direct download. 
    

-  datamerge and distributions.ipynb, containing investigation of dmv dataset joined with census data and AFDC data, as well as distribution analysis of ev registrations per year
    
    Dataset info:
  
        The vehicle datasets required can be found at the link https://data.ca.gov/dataset/vehicle-fuel-type-count-by-zip-code via the api, or direct download for each individual year. For guidance, refer to in-code instructions within "vehicle_fuel_types_eda.ipynb".
            
        California State Geoportal Govt Data:
        
        Zip Code data source is: https://gis.data.ca.gov/datasets/CDEGIS::california-zip-codes/about

-    osmnx.ipynb, containing exploration and usage of geospatial plotting and graph network based calculations
-    cenpy.ipynb, containing exploration and continued usage of government census data

other potential data sources:

        https://www.energy.ca.gov/files/zev-and-infrastructure-stats-data

all the datasets gathered, either through an API or direct download should have code in the notebooks regarding their usage.

the required packages to run the notebooks locally have been included in the form of an environment <environment.yml>
