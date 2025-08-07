---
title: "Alessandro LunAa"
author: "Jorge Espinosa"
date: "2025-08-01"
output: html_document
---


```{r}
library(readxl)
Tabla_Tidy_Distancia_6MWT_pre_y_post_IAM <- read_excel("C:/Users/Jorge/Desktop/Tabla_Tidy__Distancia_6MWT_pre_y_post_IAM.xlsx")

```

Respuesta 1
Hipòtesis: 
H0 = La rehabilitación cardiovascular domiciliaria (RCD) en pacientes con IAM no tiene mejora sobre la capacidad funcional
H1 = La rehabilitación cardiovascular domiciliaria (RCD) en pacientes con IAM tiene mejora sobre la capacidad funcional
Pregunta de investigaciòn = La rehabilitación cardiovascular domiciliaria (RCD) en pacientes con IAM tiene mejora sobre la capacidad funcional a travès de la pryeba de caminata?

R2
Primero Shapiro si teng normalidad utilizo T Test
si no tengo noramilidad utilizo Wilcoxon 

```{r}
Frame = data.frame(Tabla_Tidy_Distancia_6MWT_pre_y_post_IAM)
shapiro.test(Frame$Distancia_6MWT_m)
?shapiro.test

```

