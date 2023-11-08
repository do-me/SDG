# Sustainable Development Goals, Targets, Indicators
**tl;dr**: download either the csv or xlsx **[SDG_Target_Indicator_UNSD_2023.csv](SDG_Target_Indicator_UNSD_2023.csv)** or **[SDG_Target_Indicator_UNSD_2023.xlsx](SDG_Target_Indicator_UNSD_2023.xlsx)**

![E_SDG_logo_without_UN_emblem_horizontal_RGB-1200x219](https://github.com/do-me/SDG/assets/47481567/51f39727-b565-428e-8620-faceaf219ab3)

2023 updated list of SDGs, targets &amp; indicators with target search keywords from the [JRC SDG Mapper](https://knowsdgs.jrc.ec.europa.eu/sdgmapper#api) ready for data processing. Data sources below.

![image](https://github.com/do-me/SDG/assets/47481567/a915ec54-b5b3-4de0-a64c-28f2053149bf)


## Intro
SDG targets & indicator get yearly updates and are hence quickly outdated.
This repo holds data sources, a processing script and the final table you can freely use for any purpose: **[SDG_Target_Indicator_UNSD_2023.csv](SDG_Target_Indicator_UNSD_2023.csv)** or **[SDG_Target_Indicator_UNSD_2023.xlsx](SDG_Target_Indicator_UNSD_2023.xlsx)**. You can either download the final files (watch out for the "last modified" date) or rerun the scripts yourself to make sure to get the latest version from the UN.

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

## Info
**Attention**: as of 2023 be aware that target 11.c does not have an indicator/UNSD code yet. Check [here](https://sdgs.un.org/goals/goal11#targets_and_indicators) too. Be careful when processing.
```
11.c Support least developed countries, including through financial and technical assistance, in building sustainable and resilient buildings utilizing local materials

No suitable replacement indicator was proposed. The global statistical community is encouraged to work to develop an indicator that could be proposed for the 2025 comprehensive review. See E/CN.3/2020/2, paragraph 23.
```

## Collaboration 
PR's very welcome. Please indicate what you corrected and why, possibly with the right data source. Else, feel free to file an issue.
