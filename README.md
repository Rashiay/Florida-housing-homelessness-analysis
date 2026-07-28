#  Florida Housing, Population Trends & Homelessness Analysis (2010–2028)

A Power BI business intelligence report analyzing the relationship between population growth, housing supply, affordability, and homelessness rates across Florida[cite: 1].

---

## Project Goal

The primary objective of this report is to examine Florida's housing market dynamics from 2010 to 2023 (with projections through 2028) to determine how supply shortages and rising costs impact homelessness[cite: 1]. By synthesizing data from the **U.S. Census Bureau** and the **Annual U.S. Homeless Statistics Reports Database**, this project evaluates whether existing vacant housing assets can be strategically leveraged to mitigate housing instability[cite: 1].

---

##  Key Findings & Conclusions

1. **Supply Shortage vs. Population Spikes:** Florida added over 3.5 million residents between 2010 and 2023[cite: 1]. Year-over-year population growth consistently outpaces housing unit development—most severely in 2015 and 2021—creating a systemic supply bottleneck[cite: 1].
2. **The Affordability Squeeze:** Entry-level home supply has collapsed[cite: 1]. New home sales under **$300,000** decreased sharply after 2020, concentrating the market in the **$300,000–$399,999** price range[cite: 1]. Coupled with dips in median household income (e.g., 2022 post-COVID recovery), lower-income families face severe financial strain[cite: 1].
3. **Unlocking Vacant Housing Potential:** While total homeless counts fluctuated (peaking at 37,584 in 2011, dropping to 12,502 in 2021, and rising back to 22,925 in 2023), home vacancy rates have steadily declined[cite: 1]. The **Vacant Housing-to-Homeless Ratio (`Average xRate`)** proves that available vacant housing units remain an underutilized, immediate solution for addressing homelessness.

---

##  Dashboard Pages & Visualizations

> *Place your page screenshots inside the `assets/` folder to preview your dashboard below.*

| Page 1: Title Screen | Page 2: Population vs. Supply |
| :---: | :---: |
| ![Title Screen](assets/title_screen.png) | ![Population Growth vs Housing Supply](assets/population_vs_supply.png) |

| Page 3: Affordability & Home Sales | Page 4: Homelessness & Vacancy Rates |
| :---: | :---: |
| ![Affordability and Home Sales Trends](assets/affordability_and_sales.png) | ![Homelessness and Vacancy Rates](assets/homelessness_and_vacancy.png) |

---

##  Key Report Metrics & DAX Calculations

### 1. Homes Per 1,000 People
Measures regional housing density relative to the state population benchmark:
$$\text{Homes Per 1,000 People} = \frac{\text{[Housing Units]}}{\text{[Population]}} \times 1000$$

### 2. Year-over-Year (YoY) Growth Metrics
Tracks annual rate of change to highlight supply gap years:
```dax
Population YoY Change (%) = ([Population] - PREVIOUSYEAR([Population])) / PREVIOUSYEAR([Population])
Housing YoY Change (%) = ([Housing Units] - PREVIOUSYEAR([Housing Units])) / PREVIOUSYEAR([Housing Units])
