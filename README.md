---
title: "DS 202 Final Project"
author: "Aidan Bobholz"
date: "2024-03-30"
output: html_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

# Title
## Dairy Data

# Team Members
## Aidan Bobholz and Gavin Anderson

# Data
```{R, include = FALSE}

# Load the readxl package
library(tidyverse)
library(readxl)


library(readr)

# Read the CSV file from GitHub
url <- "https://github.com/AidanBobholz/DS202_Final_Group_16/raw/main/pcconsp_1_csv.csv"
dataset <- read_csv(url, col_names = TRUE)

```

```{R}

str(dataset)

```

```{R}


summary(dataset)
```

# Questions:
## What is the current trend of dairy products?

```{R}

# Load necessary libraries
library(ggplot2)
library(reshape2)
library(viridis)


my_palette <- viridis(22)

# Reshape data into long format
melted_data <- melt(dataset, id.vars = "Year")

# Create density plot
ggplot(melted_data, aes(x = Year, y = value, color = variable)) +
  geom_line()+
  theme(axis.text.x = element_text(angle = 90, hjust = 1, vjust = 0.5))+
  scale_color_manual(values = my_palette)



```

*This visual will be in works of improvements but as a start helps show the major variables in this dataset. Also we can find that the value of fluid beverage milk has been on a constant decline. By working on this visual further we may see even more trends with dairy products.*


## What is the most popularly consumed dairy product?

```{R}

my_palette <- viridis(22)

# Reshape data into long format
melted_data <- melt(dataset, id.vars = "Year")

# Create density plot
ggplot(melted_data, aes(x = variable, y = value)) +
  geom_boxplot()+
  theme(axis.text.x = element_text(angle = 90, hjust = 1, vjust = 0.5))



```

*In this bar plot we can see that the most valuable product is Milk fat basis by a long shot. *



**More questions are to come as we continue to go through this dataset**
