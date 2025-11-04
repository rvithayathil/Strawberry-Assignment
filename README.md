# Strawberry-Assignment-HERBICIDE-Analysis

## Project Description

This project investigates the use of herbicides across U.S. states.

The goal is to identify regional patterns and differences in herbicide application practices, and to explore the relationship between farming type and agricultural land use.

We examine how herbicide-related data differ between organic and conventional programs, aiming to uncover insights into sustainable agricultural practices.

## Dataset Description

The dataset originates from the USDA National Agricultural Statistics Service (NASS).

Data Cleaning Steps:

Removed columns only containing NA or single-value.

Removed redundant text and symbols in Domain.Category and Data.Item using sub() and trimws().

Filtered observations where Domain contained "HERB".

Combined Domain and Domain.Category into one field for easier filtering.

Combined with the data set of herbicide toxicity information.

Saved cleaned data as strawberry_with_toxicity.csv.

Key Variables:

| Variable | Description |
|------------------------------|------------------------------------------|
| **Program** | The USDA data collection program (e.g., “CENSUS”, “SURVEY”). |
| **Year** | The years in which the data were collected. |
| **State** | The U.S. states where data were collected. |
| **Domain.Category** | Production type and category (e.g., “ORGANIC: HERBICIDE”, “CONVENTIONAL: HERBICIDE”). |
| **APPLICATIONS..MEASURED.IN.LB** | Total amount of herbicide applied, measured in pounds. |
| **APPLICATIONS..MEASURED.IN.LB...ACRE...APPLICATION..AVG** | Average herbicide amount per acre per application. |
| **APPLICATIONS..MEASURED.IN.LB...ACRE...YEAR..AVG** | Average herbicide amount per acre per year. |
| **APPLICATIONS..MEASURED.IN.NUMBER..AVG** | Average number of herbicide applications. |
| **TREATED..MEASURED.IN.PCT.OF.AREA.BEARING..AVG** | Average percentage of the bearing (fruiting) area treated with herbicides. |
| **Herbicide.ID** | Unique identifier for each herbicide used in the dataset. |
| **Acute.Toxic** | Indicates whether the herbicide is classified as acutely toxic. |
| **Corrosive** | Indicates whether the herbicide is classified as corrosive. |
| **Environmental.Hazard** | Indicates whether the herbicide poses environmental hazards. |
| **Flammable** | Indicates whether the herbicide is classified as flammable. |
| **Health.Hazard** | Indicates whether the herbicide poses general health hazards. |
| **Irritant** | Indicates whether the herbicide is classified as an irritant. |
| **Additional.Info** | Additional information or safety notes related to the herbicide. |
