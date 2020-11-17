# Slides
gh pages slides and maps

## MAP
Guatemala.  Right on the fault that runs along The Americas, it has four active volcanoes and 37 in total.  The last spectacular eruption was in 2010 and the last tragical was in 2018.

```{r,  fig.align='default', echo=FALSE, comment=""}
library(leaflet)
gt_volcanoes <- data.frame(name =c("Tacaná", "Santa María", "Cerro Quemado", "Pacaya", "Fuego", "Santiaguito", "Tajumulco", "Acatenango", "Agua", "Atitlán", "Alzatate", "Amayo", "Cerro Redondo", "Cruz Quemada", "Culma", "Cuxliquel", "Chicabal", "Chingo", "Ipala", "Ixtepeque", "Jumay", "Jumaytepeque", "Las Vìboras", "Monterrico", "Moyuta", "Pakisis", "Quetzaltepeque", "San Antonio", "San Pedro", "Pecul", "Siete Orejas", "Suchitán", "Tahual", "Tecuanburro", "Tobon", "Tolimán", "Zunil"),
          alt = c(4093, 2540, 3370, 2552, 3763, 2500, 4220, 3976, 3766, 3537, 2050, 1544, 1267, 1620, 1027, 3004, 2900, 1775, 1650, 1292, 2176, 1815, 1070, 1285, 1662, 2830, 1904, 2514, 3020, 3505, 3370, 2042, 1716, 1962, 2087, 3158, 3542),
          lat = c(15.1167, 14.7333, 14.8, 14.3805, 14.4817, 14.7425, 15.0425, 14.5, 14.465, 14.5825, 14.4833, 14.3056, 14.3819, 14.1711, 14.2972, 15.8888, 14.7833, 14.5525, 14.5533, 14.4264, 14.6942, 14.3394, 14.2119, 14.55, 14.03, 14.6327, 14.6333, 14.7167, 14.65, 14.7167, 14.8, 14.192, 14.4333, 14.1539, 14.8, 14.6167, 14.7333),
          lng = c(-92.1, -91.5667, -91.5167, -90.6, -90.17, -91.5703, -91.9, -90.8833, -90.7431, -91.1864, -91.0375, -89.9958, -90.4306, -90.2778, -89.8778, -91.3983, -91.6667, -89.6378, -89.6442, -89.6842, -89.9936, -90.2589, -89.7267, -89.75, -90.1, -91.3044, -89.4433, -90.25, -91.2667, -91.4833, -91.5833, -90.4245, -89.9, -90.4025, -89.9167, -91.1833, -91.45))

gt_volcanoes %>% 
  leaflet() %>% 
  addTiles() %>% 
  addCircles(weight = 1, radius = sqrt(gt_volcanoes$alt)*70, color = "magenta")
```

