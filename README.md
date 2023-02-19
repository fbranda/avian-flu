# Avian Flu 

This repository contains the most updated information on HPAI outbreaks in domestic poultry and captive birds and HPAI positive cases in wild birds in (i) Europe, according to official reporting sources ([ADIS – Animal Disease Information System](https://eurlaidata.izsvenezie.it/)); (ii)ì USA, according to official reporting sources ([USDA - United States Department of Agriculture])(https://www.aphis.usda.gov/aphis/home/) . 

Currently, the United Kingdom is not included. For further information on this country, please refer to the website for [Avian Influenza (bird flu)](https://www.gov.uk/guidance/avian-influenza-bird-flu).

## NEXT UPDATE
1) Data from the United Kingdom will be added
2) European data by species will be added



## Getting the data

**Direct download (CSV)**: https://raw.githubusercontent.com/fbranda/avian-flu/main/general-situation.csv


**Python** (requires `pandas`):
```python
import pandas as pd
df = pd.read_csv("https://raw.githubusercontent.com/fbranda/avian-flu/main/general-situation.csv")
```

**R** (requires `httr`):
```r
library(httr)
df <- read.csv(text=content(GET("https://raw.githubusercontent.com/fbranda/avian-flu/main/general-situation.csv")))
```

## License and attribution

This repository and data exports are published under the CC BY 4.0 license.
