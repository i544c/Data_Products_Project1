---
title: "Data Product Project 1 - Map"
author: "Author: Isaac G Veras"
Date: "05/10/2023"
output: html_document
---


```{r install packages, include = FALSE}
knitr::opts_chunk$set(echo = FALSE)

if (!require("pacman")) install.packages("pacman")
pacman::p_load(
        pacman,
        leaflet
)
```

## João Pessoa City, Paraiba State - Brazil

**`Octuber 21, 2023`**


```{r Coordenadas do Brasil}
# Coordenadas do Brasil (centro geográfico)
brasil_lat <-  -7
brasil_long <- -34.8

leaflet() %>%
        setView  (lng = brasil_long, lat = brasil_lat, zoom = 10) %>%
        addTiles() %>%
        addPopups(lng = brasil_long, lat = brasil_lat, popup = "Paraiba, Brasil")
```
![dpp1](https://github.com/i544c/Data_Products_Project1/assets/104391905/79cb7b7a-ef84-41a3-80f9-fa4910e69a19)
