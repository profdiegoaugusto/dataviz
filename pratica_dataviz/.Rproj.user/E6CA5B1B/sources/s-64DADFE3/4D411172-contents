# install.packages("ggplot2")
library(tidyverse)
extrafont::loadfonts(device="win")
library(ggplot2)
library(ggthemes)


olimpiadas <- read.csv("data/olimpiadas_brasil.csv", sep = ",", header=TRUE)
head(olimpiadas, 5) 

populacao_sudeste <- read.csv("data/populacao_sudeste.csv", sep = ",", header=TRUE)
head(populacao_sudeste, 5) 


# Gráfico de Barras


populacao_sudeste$regiao <- factor(populacao_sudeste$regiao, levels = populacao_sudeste$regiao[order(-populacao_sudeste$populacao)])
maxPopulacao <- max(populacao_sudeste$populacao)

maxPopulacao



ggplot(populacao_sudeste, aes(x=populacao_sudeste$regiao, y=populacao_sudeste$populacao)) +
    geom_bar(stat="identity", fill="steelblue") + 
    scale_y_continuous(limits=c(0, maxPopulacao), labels=function(x) format(x, big.mark = ".", decimal.mark = ",", scientific = FALSE)) +
    theme_tufte() +
    theme(axis.title.x = element_blank(),
          axis.title.y = element_blank())



# Gráfico de Barras Horizontal




# Histograma






# Gráfico de Dispersão




# Mapa de Calor (Heatmap)





# Gráfico de Linhas





# Gráfico de Área





# Gráfico de Área Empilhada




# Gráfico de Barras Empilhadas





# Gráfico de Barras Agrupadas



# Gráfico de Setores (Pizza)





# Gráfico de Setores (Rosca)





# Treemap




