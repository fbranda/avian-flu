# Avian Flu 

This repository contains the most updated information on HPAI outbreaks in domestic poultry and captive birds and HPAI positive cases in wild birds in (i) Europe, according to official reporting sources ([ADIS – Animal Disease Information System](https://eurlaidata.izsvenezie.it/)); (ii) USA, according to official reporting sources ([USDA - United States Department of Agriculture](https://www.aphis.usda.gov/aphis/home/)); (iii) Italy, according to official reporting sources ([IZSVe - Istituto Zooprofilattico Sperimentale delle Venezie](https://www.izsvenezie.com/)).

Currently, the United Kingdom is not included. For further information on this country, please refer to the website for [Avian Influenza (bird flu)](https://www.gov.uk/guidance/avian-influenza-bird-flu).

## NEXT UPDATE
1) Data from the United Kingdom will be added
2) European data by species will be added

## Data dictionary

The [data dictionary](https://github.com/fbranda/avian-flu/blob/main/data_dictionary.yml) contains information about columns/fields in the list files.


## Data schema

**Filename:** europe-cases.csv


| Field                 | Format                       |Description                      
|-----------------------------|-----------------------------------|-------------------------------|
| **Confirmed date**      | YYYY-MM-DD Date of notification	  |
| **Country date**      | String       | Name of the country	 |
| **Lat**      | WGS84       | Latitude of the country  |
| **Long**      | WGS84       | Longitude of the country  |
| **HPAI strain**      | String       | Name of the HPAI strain  |
| **WOAH Classification**      | String       | Name of the species  |
| **Cases**      | Integer       | Number of cases  |


**Directory:**  Italy<br>
**Filename:** hpai-wild-birds-#.csv (example: hpai-wild-birds-2021-2022.csv)<br>


| Field                 | Format                       |Description                      
|-----------------------------|-----------------------------------|-------------------------------|
| **n**      | Integer | Number of the row	  |
| **ID ADIS**      | String       | ADIS Reference is a unique identification code authomatically created by the EU Animal Disease Information System (Regolations (EU) 2016/429 e 2020/2002) when Competent Autority of each Member State notifies an animal disease outbreak. The actual number of outbreaks is the one indicated in the first column of the table.	 |
| **Region**     |  String       | Name of the region   |
| **Province**     |  String       | Name of the province   |
| **Latitude**      | WGS84       | Latitude of the province  |
| **Longitude**      | WGS84       | Longitude of the province  |
| **No. animals**      | Integer       | Number of cases  |
| **Species**      | String       | Name of the species  |
| **HPAI strain**      | String       | Name of the HPAI strain  |
| **Confirmation date**      | YYYY-MM-DD| Date of notification	  |

**Directory:**  Italy<br>
**Filename:** hpai-domestic-poultry-#.csv (example: hpai-domestic-poultry-2021-2022)<br>


| Field                 | Format                       |Description                      
|-----------------------------|-----------------------------------|-------------------------------|
| **n**      | Integer | Number of the row	  |
| **ID ADIS**      | String       | ADIS Reference is a unique identification code authomatically created by the EU Animal Disease Information System (Regolations (EU) 2016/429 e 2020/2002) when Competent Autority of each Member State notifies an animal disease outbreak. The actual number of outbreaks is the one indicated in the first column of the table.	 |
| **Region**     |  String       | Name of the region   |
| **Province**     |  String       | Name of the province   |
| **Latitude**      | WGS84       | Latitude of the province  |
| **Longitude**      | WGS84       | Longitude of the province  |
| **No. animals**      | Integer       | Number of cases  |
| **Species**      | String       | Name of the species  |
| **HPAI strain**      | String       | Name of the HPAI strain  |
| **Confirmation date**      | YYYY-MM-DD| Date of notification	  |
| **Extinction date**      | YYYY-MM-DD| Termination date surveillance	  |
| **Measures Protection Zone in force until**      | YYYY-MM-DD| The boundaries of the protection and surveillance zones and the date on which the measures applied will be lifted, were decided according to art 21 point 2 ‘The competent authority shall adapt the boundaries of the initial restricted zone, including the boundaries of the protection, surveillance and the further restricted zones, in the case of the overlapping of two or more restricted zones due to further outbreaks of the category A disease.’, and art 39 point 1 a) and b) of the Commission Delegated Regulation (EU) 687/2020 ‘The competent authority may lift the measures provided for in Section 1 and 2 of this Chapter only if the minimum period set out in Annex X has elapsed and the following conditions are fulfilled: (a) the preliminary cleaning and disinfection and, where relevant, control of insects and rodents, has been performed in accordance with Article 15 in the affected establishment; and (b) in all establishments keeping animals of listed species in the protection zone, animals of listed species have undergone, with favourable results, clinical and when necessary laboratory examination in accordance with Article 26.’ The amendments to these zone will be published regularly with the Commission Implementing Decision (EU) 2021/641.	  |
| **Measures Surveillance Zone in force until**      | YYYY-MM-DD| The boundaries of the protection and surveillance zones and the date on which the measures applied will be lifted, were decided according to art 21 point 2 ‘The competent authority shall adapt the boundaries of the initial restricted zone, including the boundaries of the protection, surveillance and the further restricted zones, in the case of the overlapping of two or more restricted zones due to further outbreaks of the category A disease.’, and art 39 point 1 a) and b) of the Commission Delegated Regulation (EU) 687/2020 ‘The competent authority may lift the measures provided for in Section 1 and 2 of this Chapter only if the minimum period set out in Annex X has elapsed and the following conditions are fulfilled: (a) the preliminary cleaning and disinfection and, where relevant, control of insects and rodents, has been performed in accordance with Article 15 in the affected establishment; and (b) in all establishments keeping animals of listed species in the protection zone, animals of listed species have undergone, with favourable results, clinical and when necessary laboratory examination in accordance with Article 26.’ The amendments to these zone will be published regularly with the Commission Implementing Decision (EU) 2021/641.	  |






## Getting the data

**Direct download (CSV)**: https://raw.githubusercontent.com/fbranda/avian-flu/main/europe-cases.csv


**Python** (requires `pandas`):
```python
import pandas as pd
df = pd.read_csv("https://raw.githubusercontent.com/fbranda/avian-flu/main/europe-cases.csv")
```

**R**:
```r
df <- read.csv("https://raw.githubusercontent.com/fbranda/avian-flu/main/europe-cases.csv")
```

## License and attribution

This repository and data exports are published under the CC BY 4.0 license.

Please cite as: "Francesco Branda Avian Flu (accessed on YYYY-MM-DD)"
