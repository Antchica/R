``` R
# Instalamos la librería
library(taskscheduleR)

#Añadimos el nombre que le queramos poner a la tarea que se va a automatizar.
#Indicamos la ruta del archivo que vamos a automatizar en Drive
#Indicamos si queremos que se automatize diariamente, semanalmente, mensualmente o anualmente
#Seleccionamos a la hora que queramos que se automatize y la fecha cuando queramos que empiece

taskscheduler_create (taskname = "Nombre_Archivo",
                      rscript = "ruta del archivo",
                      schedule = "DAILY", starttime = "08:00", startdate = "27/12/2023") ```
