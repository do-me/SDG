# Sustainable Development Goals, Targets, Indicators
![E_SDG_logo_without_UN_emblem_horizontal_RGB-1200x219](https://github.com/do-me/SDG/assets/47481567/51f39727-b565-428e-8620-faceaf219ab3)

2023 updated list of SDGs, targets &amp; indicators ready for data processing with data sources

![image](https://github.com/do-me/SDG/assets/47481567/234e4c1b-1a0e-4901-a660-a60cc9b75a27)


## Intro
SDG targets & indicator get yearly updates and are hence quickly outdated.
This repo holds data sources, a processing script and the final table you can freely use for any purpose: **SDG.xlsx** or **SDG.csv**.

You can load the csv in pandas with:

```python
import pandas as pd
df = pd.read_csv("SDG_Target_Indicator_UNSD_2023.csv",delimiter=";")
df
```

Or load the table directly in your script with pandas without cloning this repo or downloading any file manually:

```python
import pandas as pd
df = pd.read_csv("https://raw.githubusercontent.com/do-me/SDG/main/SDG_Target_Indicator_UNSD_2023.csv",delimiter=";")
df
```

## Data sources 
- Main indicator table homepage: https://unstats.un.org/sdgs/indicators/indicators-list/ ([xlsx](https://unstats.un.org/sdgs/indicators/Global%20Indicator%20Framework%20after%202023%20refinement.English.xlsx))
- Logos: https://www.un.org/sustainabledevelopment/news/communications-material/
- SGD Names from 2023 report: https://unstats.un.org/sdgs/report/2023/ ([pdf](https://unstats.un.org/sdgs/report/2023/The-Sustainable-Development-Goals-Report-2023.pdf))

## Collaboration 
PR's very welcome. Please indicate what you corrected and why, possibly with the right data source. Else, feel free to file an issue.
