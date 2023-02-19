# Avian Flu 

This repository contains data extracted from the [Italian National Institute of Health (ISS)](https://www.epicentro.iss.it/influenza/influnet) bulletins starting from the [2003-2004 seasonal flu](https://w3.iss.it/site/rmi/influnet/pagine/stagioni.aspx). The repository will be updated every Friday.

This repository contains the most updated information on HPAI outbreaks in domestic poultry and captive birds and HPAI positive cases in wild birds in Europe, according to official reporting sources ([ADIS – Animal Disease Information System](https://eurlaidata.izsvenezie.it/)).

Currently, the United Kingdom is not included. For further information on this country, please refer to the website for [Avian Influenza (bird flu)](https://www.gov.uk/guidance/avian-influenza-bird-flu).



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
