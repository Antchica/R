``` R
# Instalamos y cargamos la librería para obtener los datos
install.packages("nycflights13")
library(nycflights13)
data("planes")

###Visualización de datos

#Histograma de años de fabricación de aviones
ggplot(planes, aes(x = year)) +
  geom_histogram(binwidth = 1, fill = "skyblue", color = "black") +
  labs(title = "Histograma de años de fabricación de aviones", x = "Año", y = "Frecuencia")

###Gráfico de barras de fabricantes de aviones
ggplot(planes, aes(x = manufacturer)) +
  geom_bar(fill = "salmon", color = "black") +
  labs(title = "Cantidad de aviones por fabricante", x = "Fabricante", y = "Cantidad") +
  theme(axis.text.x = element_text(angle = 90, hjust = 1))

