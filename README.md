# Analysis of trends in Dairy Consumption in the United States

#### Aidan Bobholz and Gavin Anderson

## Introduction

The goal of this project is to explore data sets around the Dairy Industry to better understand trends in the usage of dairy commodities. As with most agricultural markets there have been notable events that occur in which cause massive changes in the usage of agricultural commodities. Analysis on this topic can give us as students in agriculture a better insight into the ways in which the dairy market is effected. Our end goal is to identify the major trends in dairy commodity usages and find reasons that may be attributed to the increased or decreased usages.

To follow this goal we will explore further into these questions:

1.  What is the most consumed dairy commodity?

2.  What are the trends in consumption of dairy products?

3.  Does corn production trends follow the trends of dairy consumption?

4.  Does the sale price of Alfalfa production effect dairy consumption?

5.  How does Average price paid for milk effect dairy consumption?

6.  Does milk cow costs have an effect on dairy consumption?

## Data

### Structure

The link to our datasets can be found at <https://www.ers.usda.gov/data-products/dairy-data.aspx>. We are using the "Dairy products: Per capita consumption, United States (Annual)" as our major dataset and will have additional datasets added to compare trends in; corn production and the Annual milk production and factors affecting supply (Annual).

### Cleaning

First in cleaning the data frames we needed to manual format the source datasheets. The USDA had formatted the datasheets in a way that tidyverse would have a harder time getting them formatted to use than it would take for us to manual edit them. In editing them we formatted it so that there was column headers with descriptive names of their values. This was done for all three datasheets used.

After this manual cleaning of the data frames we had then imported them into our Rmarkdown file,

``` r

dataset <- read.csv("pcconsp_1_csv.csv")
```

### Variables

-   Year: The year in which the data point was collected.
-   Fluid_Beverage_Milk: The amount of milk as a beverage consumed in the U.S. per capita.
-   American_Cheese: The amount of American cheese consumed in the U.S. per capita.
-   Other_than_American_Cheese: The amount of cheese other than American cheese consumed in the U.S. per capita.
-   Cottage_Cheese: The amount of Cottage cheese consumed in the U.S. per capita.
-   Butter: The amount of butter consumed in the U.S. per capita.
-   Dry_Whole_Milk: The amount of Dry_Whole_Milk consumed in the U.S. per capita.
-   Nonfat_and_Skim_milk_powder: The amount of Nonfat_and_Skim_milk_powder consumed in the U.S. per capita.
-   Dry_Butter_Milk: The amount of Dry_Butter_Milk consumed in the U.S. per capita.
-   Dry_Whey_and_Whey_Protein_Concentrate: The amount of Dry_Whey_and_Whey_Protein_Concentrate consumed in the U.S. per capita.
-   Regular_Ice_Cream: The amount of Regular_Ice_Cream consumed in the U.S. per capita.
-   Low_Fat_Ice_Cream: The amount of Low_Fat_Ice_Cream consumed in the U.S. per capita.
-   Frozen_Yougurt (is NA needs removed)
-   Sherbet: The amount of Sherbet consumed in the U.S. per capita.
-   Other_Frozen_Dairy: The amount of Other_Frozen_Dairy consumed in the U.S. per capita.
-   Water_And_Juices: The amount of Water_And_Juices consumed in the U.S. per capita.
-   Yougurt_Other_Than_Frozen: The amount of Yougurt_Other_Than_Frozen consumed in the U.S. per capita.
-   Whole_Condensed_Milk_Canned: The amount of Whole_Condensed_Milk_Canned consumed in the U.S. per capita.
-   Whole_Condensed_Milk_Bulk: The amount of Whole_Condensed_Milk_Bulk consumed in the U.S. per capita.
-   Skim_Condensed_Milk_Bulk_Canned: The amount of Skim_Condensed_Milk_Bulk_Canned consumed in the U.S. per capita.
-   Milk_fat_basis: The amount of Milk_fat_basis consumed in the U.S. per capita.
-   Skim_solids_basis (Is NA needs removed)

## Results

#### What is the most consumed dairy commodity?

![](sales_counts.jpeg){width="632"}

The most consumed dairy commodity is Beverage milk by far per capita in the United States.

#### What are the trends in consumption of dairy products?

![](trends_facet.jpeg)

Overall in trends most commodity groups of dairy products have been trending down overtime, while the cheese commodity group has actually been increasing overtime.

#### Does corn production trends follow the trends of dairy consumption?

Reply #3

#### Does the sale price of Alfalfa production effect dairy consumption?

Reply #4

#### How does Average price paid for milk effect dairy consumption?

Reply #5

#### Does milk cow costs have an effect on dairy consumption?

Reply #6

## Conclusion

In the conculusion...
