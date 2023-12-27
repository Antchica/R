``` R
#Instalamos y cargamos las librerías
library(writexl)
library(googledrive)
library(rmarkdown)
library(RODBC)
library(data.table)
library(DBI)
library(odbc)
library(reactable)
library(scales)
library(lubridate)
library(dplyr)

#Cargamos la ruta de la tarea que queramos automatizar
path_data <- "Ruta de la tarea a automatizar"

#Seleccionamos el archivo que se va a automatizar
render(file.path(path_data, "mi_documento.Rmd"))

#Indicamos la ruta de Drive donde queremos que se guarde el archivo automatizado y el archivo que queremos subir
file <- "ruta de la carpeta de Drive"
archivo_local <- file.path( "Ruta de la tarea a automatizar", paste0("mi_documento", ".html")

#Indicamos el nombre con el que queremos que se guarde y el formato
nombre_en_drive<- paste0 ("Nombre_documento", Sys.Date(), ".html")

#Subimos el archivo a Google Drive
file_uploaded <- drive_upload (path = file,
                         media = archivo_local,
                         home = nombre_en_drive,
                         type = "html")
```
