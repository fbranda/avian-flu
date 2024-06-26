# Avian Flu 

This repository contains the most updated information on HPAI outbreaks in domestic poultry and captive birds and HPAI positive cases in wild birds in 
1) Europe, according to official reporting sources ([ADIS – Animal Disease Information System](https://eurlaidata.izsvenezie.it/))
2) USA, according to official reporting sources ([USDA - United States Department of Agriculture](https://www.aphis.usda.gov/aphis/home/))
3) Italy, according to official reporting sources ([IZSVe - Istituto Zooprofilattico Sperimentale delle Venezie](https://www.izsvenezie.com/))
4) Argentina, according to official reporting sources ([SENASA - DIRECCIÓN NACIONAL DE SANIDAD ANIMAL](https://www.argentina.gob.ar/senasa/influenza-aviar))
5) England, according to official reporting sources ([GOV.UK](https://www.gov.uk/government/publications/avian-influenza-influenza-a-h5n1-technical-briefings/investigation-into-the-risk-to-human-health-of-avian-influenza-influenza-a-h5n1-in-england-technical-briefing-2#part-2-epidemiology-update))

## Repository structure
```
avian-flu/
│
├── */
│   ├── Africa/
│   │   ├── africa-outbreaks.csv
│   ├── Americas/
│   │   ├── Argentina/
│   │   │   ├── argentina-aves-de-corral-cases.csv
│   │   │   ├── argentina-aves-no-corral-cases.csv
│   │   ├── USA/
│   │   │   ├── commercial-backyard-flocks.csv
│   │   │   ├── hpai-mammals.csv
│   │   │   ├── hpai-wild-birds.csv
│   │   ├── americas-outbreaks.csv
│   ├── Asia/
│   │   ├── asia-outbreaks.csv
│   ├── Europe/
│   │   ├── Italy/
│   │   │   ├── HPAI/
│   │   │   │   ├── 2021-2022/
│   │   │   │   │   ├── hpai-domestic-poultry-2021-2022.csv
│   │   │   │   │   ├── hpai-wild-birds-2021-2022.csv
│   │   │   │   ├── 2022-2023/
│   │   │   │   │   ├── hpai-domestic-poultry-2022-2023.csv
│   │   │   │   │   ├── hpai-wild-birds-2022-2023.csv
│   │   ├── United Kingdom/
│   │   │   ├── human-potential-exposures.csv
│   │   │   ├── poultry-wildbirds-england.csv
│   │   │   ├── wild-mammals-england.csv
│   │   │   ├── wild-mammals-international.csv
│   ├── Line-lists/
│   │   ├── H3N8/
│   │   │   ├── 2023-03-27-avian-flu-linelist.csv
│   │   ├── H5/
│   │   │   ├── H5N1/
│   │   │   │   ├── 2022-01-14-avian-flu-linelist.csv
│   │   │   │   ├── 2022-05-06-avian-flu-linelist.csv
│   │   │   │   ├── ...
│   │   │   ├── 2022-10-21-avian-flu-linelist.csv
│   │   │   ├── 2023-01-09-avian-flu-linelist.csv
│   │   │   ├── ...
│   ├── PDFs/
│   ├── images/
│   ├── human-cases.csv
│   ├── summary-outbreaks-mammals.csv

```


## Information on data files
1) The **Argentina** folder was added on March 12
2) The **Americas**, **Asia**, **Africa** folders was added on March 15
3) The **United Kingdom** folder was added on March 16

## Visualization
1) Italy Map <br><br>
<a href="https://lnkd.in/dbT2T3WG"><img src="https://github.com/fbranda/avian-flu/blob/main/images/Fr6xLWsXoAA_gpj.jpeg" alt="Italy" data-canonical-src="https://github.com/fbranda/avian-flu/blob/main/images/Fr6xLWsXoAA_gpj.jpeg" width="700"/></a>

## Data dictionary

The [data dictionary](https://github.com/fbranda/avian-flu/blob/main/data_dictionary.yml) contains information about columns/fields in the list files.


## Data schema

**Filename:** europe-cases.csv


| Field                 | Format                       |Description                      
|-----------------------------|-----------------------------------|-------------------------------|
| **Confirmed date**      | YYYY-MM-DD  | Date of notification	 
| **Country**      | String       | Name of the country	 |
| **Lat**      | WGS84       | Latitude of the country  |
| **Long**      | WGS84       | Longitude of the country  |
| **HPAI strain**      | String       | Name of the HPAI strain  |
| **WOAH Classification**      | String       | Name of the species  |
| **Outbreaks**      | Integer       | Number of outbreaks  |


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

## Contributions
1) [Branda F, Mazzoli S. The importance of rapid and robust availability of epidemiological data for real-time mapping of the risk of avian influenza a (H5N1) spread. Pathogens and Global Health. 2023 Jun 22:1-4.](https://www.tandfonline.com/eprint/FS9IJRRHTYGF44KPJEQX/full?target=10.1080/20477724.2023.2228055)


2) [Branda, F.; Mazzoli, S.; Pierini, M.; Ciccozzi, M. Trends and Spatiotemporal Patterns of Avian Influenza Outbreaks in Italy: A Data-Driven Approach. Infect. Dis. Rep. 2024, 16, 1-12.](https://www.mdpi.com/2036-7449/16/1/1)



## License and attribution

This repository and data exports are published under the CC BY 4.0 license.

Please cite as: Francesco Branda. (2023). Open Avian Flu Dataset [Data set]. Zenodo. https://doi.org/10.5281/zenodo.8246456
