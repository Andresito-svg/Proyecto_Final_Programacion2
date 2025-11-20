# Proyecto_Final_Programacion2
La base de datos elegida tiene 1001 datos, dentro de los cuales se encuentra informacion como: marca, modelo, especificaciones propias de ram, almacenamiento, etc. Se realizó una limpieza y analísis de datos. De este proceso se obtuvieron diversas conclusiones, este dataset fue tomado de kaggle "World Smartphone Market 2025". 

Grupo 3

## Integrantes
-Andres Romero

-Daniela Buitrago

-Juliana Guerra 

## Explicación:

### Archivos:

-Global_Mobile_Prices_2025_Extended.

-Proyecto.IPYNB

### Cantidad de datos:

Filas:1000

Columnas:15

### Tipo de dato:

-Brand: Object.

-Model: Object.

-Price_usd: int64.  

-Ram_gb: int64.

-Storage_gb: int64.  

-Camera_mp: int64.

-Battery_mah: int64.

-display_size_inch: float64.

-Charging_watts: int64.

-5g_support: object.

-os: object. 

-processor: object.

-rating: float64.

-release month: object.

-Year: int64.

## Diccionario de los datos:

-Brand: Nombre del marca del celular. 

-Model: Modelo del celular. 

-Price_usd: Precio del celular en dolares. 

-Ram_gb: Cantidad de gb de ram que tiene el celular. 

-Storage_gb: Capacidad de almacenamiento en gb del celular. 

-Camera_mp: megapixeles de la cámara frontal. 

-Battery_mah: Capacidad de mah de la bateria. 

-display_size_inch: Tamaño en pulgadas de la pantalla. 

-Charging_watts: Capacidad de cargar en watts del celular. 

-5g_support: configuración de 5G. 

-os: Sistema operativo. 

-processor: Tipo de procesador.

-rating: calificación de los críticos.

-release month: Mes de salida al mercado.

-Year: Año de salida al mercado.

## Instrucciones para ejecutar el notebook y activar el entorno:
-Paso 1:
Debido a que el proyecto fue realizado en Google Colab, primero se debe montar el Google Drive para acceder al excel en el cual está la base de datos. Esto se realizó con el siguiente código:
"from google.colab import drive
drive.mount('/content/drive')"

-Paso 2:
Luego de montar el entorno se ubica la dirección del archivo excel usando la siguiente línea:
%cd "//content/drive/MyDrive/Colab Notebooks/Universidad/Progra 2/Proyecto/"

-Paso 3:
Continuando se descargan e instalan las librerias necesarias usando el comando import _ as _ , que en este caso fueron:
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
import numpy as np

-Paso 4:
Como siguiente paso se cargó la base de datos, que tiene como nombre "Global_Mobile_Prices_2025_Limpia1.xlsx". Para poder usar esta base se le asignó un nombre y uso el comando pd.read_excel como se muestra a continuación:
df = pd.read_excel("Global_Mobile_Prices_2025_Limpia1.xlsx")

-Paso 5:
Finalmente se verificó que no hubiera ningún inconveniente, por lo que se usaron los siguientes comandos:
df.head(10)
df.info()
df.shape
los cuales sirven para revisar los primeros 10 datos de la base de datos, la información de las variables (Tipo,Nulo) y las filas y columnas.
