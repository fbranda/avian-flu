# WWSCAN Data Dictionary 

This data dictionary is for data downloaded via the data.wastewaterscan.org website.



## Data schema

**Filename:** summary-h5.csv


| Field                 | Format                       |Description                      
|-----------------------------|-----------------------------------|-------------------------------|
**sample_collected**      | YYYY-MM-DD  | Date sample was collected    | 
**state_name**      | String       | Full name of the State in which the collection site resides |
**state_id**      | String       | 2-letter from the ANSI standard INCITS 38:2009 (supersedes FIPS 5-2) |
**state_ansi**      | String       | 2-digit codes from the ANSI standard INCITS 38:2009 (supersedes FIPS 5-2) |
**county_name**      | String       | Full name of the County in which the collection site resides  |
**county_fips**      | String       | 5-digit FIPS code of the `county_name`. The first two digits correspond to the state's FIPS code.	 |
**city_name**      | String       | Full name of the City in which the collection site resides  | 
  **facility_name**      | String       | Full name of the collection site  | 
 **NPDES_ID**      | Numeric       | Unique identifier assigned to each collection site under the National Pollutant Discharge Elimination System (NPDES) program, which regulates pollutant discharges to waters of the United States |
 **FRS_ID**      | Numeric       | The Facility Registry Service (FRS) is a unique identifier assigned by the Environmental Protection Agency (EPA) system to track environmental facilities |
**facility_address**      | String       | Physical address of the collection site  | 
**watershed_HUC12**      | Numeric       | The identifier of the watershed in which the collection site is located, based on the Hydrologic Unit Code (HUC12)   | 
**lat_facility**      | Numeric       | Latitude of the collection site  |
**long_facility**      | Numeric       | Longitude of the collection site |
**major_minor_facility**      | String       | This field indicates whether the collection site is considered major (M) or minor (N) in terms of environmental importance or impact |
**facility_type**      | String       | The type of plant. For example, "POTW" (Publicly Owned Treatment Works) indicates a publicly owned wastewater treatment plant |
 **quantity_nucleic_acids**      | Numeric       | Quantity of nucleic acids normalized to Pepper Mild Mottle Virus (PPMoV) concentration (x1 million) |



## License and attribution

This repository and data exports are published under the CC BY 4.0 license.

