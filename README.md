# Electric Vehicle Population

📍 README in Ukrainian language: [README-UA](README-UA.md)

📍 Initial Dataset: [dataset](initial-dataset.csv)

📍 Excel Workbook: [workbook](ElectricVehiclePopulationData_workbook.xlsx)

📍 Cleaned Dataset: [cleaned dataset](ElectricVehiclePopulationClearData.csv)

📍 Tableau Dashboard: [dashboard](ElectricVehicle.twb)

---

## Table of contents

- [1. Data Understanding](#1-data-understanding)
- [2. Data Cleaning](#2-data-cleaning)
- [3. Exploratory Data Analysis](#3-exploratory-data-analysis)
- [4. Spatial Analysis](#4-spatial-analysis)
- [5. Hypotheses and Conclusions](#5-hypotheses-and-conclusions)
- [6. Additional Findings and Interesting Details](#6-additional-findings-and-interesting-details)

---

## 1. Data Understanding

The dataset Electric Vehicle Population Data contains information about registered electric vehicles in Washington State, USA. The dataset represents real-world vehicle registration records and includes technical and geographical information.

Each row represents one registered electric vehicle.

The dataset contains information about:

| Column | Description |
|---|---|
| VIN (1-10) | First 10 characters of the Vehicle Identification Number
County | County where the vehicle is registered
City | Registration city
State | State code
Postal Code | ZIP code of registration location
Model Year | Vehicle manufacturing year
Make  | Vehicle manufacturer
Model | Vehicle model
Electric Vehicle Type | BEV or PHEV classification
CAFV Eligibility  | Clean Alternative Fuel Vehicle eligibility status
Electric Range | Maximum electric driving range (miles)
Base MSRP | Manufacturer suggested retail price
Legislative District | Legislative district number
DOL Vehicle ID | Unique vehicle identifier
Vehicle Location | Geographic coordinates
Electric Utility | Electricity provider
2020 Census Tract | Census area identifier

---

## 2. Data Cleaning

Before performing analysis, the dataset was inspected for:

* missing values;
* duplicated records;
* incorrect values;
* inconsistent naming;
* outliers

---

## 3. Exploratory Data Analysis

You can see dashboard online: [Tableau Public Dashboard](https://public.tableau.com/views/ElectricVehicle_17856090722630/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

![Tableau dashboard 1](./images/tableau-1.png)

![Excel dashboard 1](./images/excel-1.png)

![Excel dashboard 2](./images/excel-2.png)

![Excel dashboard 3](./images/excel-3.png)

## 4. Spatial Analysis

The dataset contains geographic information, allowing analysis of EV distribution.

You can see dashboard online: [Tableau Public Dashboard](https://public.tableau.com/shared/3M95M4PH6?:display_count=n&:origin=viz_share_link)

![Tableau dashboard 2](./images/tableau-2.png)

## 5. Hypotheses and Conclusions

#### Hypothesis 1

Electric vehicle adoption has increased over time.

The number of newer model-year vehicles is significantly higher than older vehicles.

---

#### Hypothesis 2

`BEV` vehicles are definetly more popular than `PHEV` vehicles.

The dataset shows a higher proportion of fully electric vehicles.

---

#### Hypothesis 3

TESLA takes the first place in BEV vehicles.

TESLA vehicles registered `104,728` times, while the second place belongs to CHEVROLET with `18,124` vehicles.

---

#### Hypothesis 4

Newer vehicles have better electric range.

Modern EV models demonstrate significantly higher range compared with older vehicles.

---

## 6. Additional Findings and Interesting Details

During the analysis, several unusual patterns were investigated.

#### BrightDrop naming issue, some vehicles appear as:
```
Make = Chevrolet
Model = BrightDrop
```

and others as:

```
Make = BrightDrop
Model = ZEVO
```

This was identified as a manufacturer branding transition rather than a data error.

---

#### Zero MSRP Values, many vehicles contain:

Base MSRP = 0

This was identified as missing price information rather than a real price.

---

## Final Conclusion

The analysis demonstrates that the electric vehicle market in Washington State is rapidly developing.

The main conclusions are:

1. Battery Electric Vehicles dominate the market compared with Plug-in Hybrid vehicles.
2. Tesla, Nissan, and Chevrolet are among the most represented manufacturers.
3. Electric vehicle adoption is strongly concentrated in urban regions.
4. Newer EV models provide significantly better electric range, but we can see a huge drop in 2011 for some reason.
5. Data quality issues were mostly related to naming inconsistencies and missing values rather than incorrect records.
