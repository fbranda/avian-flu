# WWSCAN Data Dictionary 

This data dictionary is for data downloaded via the data.wastewaterscan.org website.



## Data schema

**Filename:** summary-h5.csv


| Field                 | Format                       |Description                      
|-----------------------------|-----------------------------------|-------------------------------|
| **Sample_collected**      | YYYY-MM-DD  | Date sample was collected    
| **State**      | String       | Full name of the State in which the collection site resides
  **County**      | String       | Full name of the County in which the collection site resides  |
  **City**      | String       | Full name of the City in which the collection site resides  | 
  **Facility_name**      | String       | Full name of the collection site  | 
  **lat_facility**      | WGS84       | Latitude of the collection site  |
| **long_facility**      | WGS84       | Longitude of the collection site |
| **Quantity_nucleic_acids**      | Numeric       | Quantity of nucleic acids normalized to Pepper Mild Mottle Virus (PPMoV) concentration (x1 million) |



## License and attribution

This repository and data exports are published under the CC BY 4.0 license.

