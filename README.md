# Librerias de Proyeccion


## Instaladores

Este programa sirve para instalar las librerias requeridas para realizar las estimaciones y proyecciones. 
    
## Proceso de proyecciones


![alt text](https://github.com/ApoyoAnalytics/PIBNowcast/blob/cambio_de_nombre/proceso.jpg?raw=true)

### Proyeccion mensual - ARIMA (p1ARIMA)

1. Actualice la base de datos dentro de input: bd_Panama
2. Corra el programa p1ARIMA
3. Los resultados se guardan dentro de la carpeta resultados con el nombre baseARIMA

### Proyeccion mensual - Interpolacion (p2InterpolacionProyeccion)

1. Actualice la base de datos dentro de input: bd_Panama
2. Corra el programa p2InterpolacionProyeccion
3. Los resultados se guardan dentro de la carpeta resultados con el nombre baseInterpolacion

### Proyeccion trimestral - Nowcasting (p3nowcast)

1. Actualice la base de datos dentro de input: bd_Panama
2. Corra el programa p3_proyeccionnowcast
3. Los resultados se guardan dentro de la carpeta resultados con el nombre baseNowcast

## Programas de soporte

Estas librerias realizan las estimaciones necesarias para tener los parámetros de cada modelo usado en los procesos de proyección.
    
### ConstruccionBasedeDatos

En este programa se construye la base de datos usada para las estimaciones y proyecciones, se calculan los estadisticos descriptivos y las correlaciones.


### m1Kalman

Se realiza la estimacion del modelo Kalman de interpolacion.

### m2Evaluacion

Se realiza la evaluación del modelo de interpolacion.

### m3nowcast

Se estima el modelo de nowcast.

###  m4nowcast_kalman

Libreria auxiliar.

## Carpetas


### inputs

En esta carpeta se guarda el excel bd_Panama.xlsx, en donde se encuentran todas las series de las distintas frecuencias.

### model_nowcast

En esta carpeta se guardan los resultados de las estimaciones del programa nowcast.

### model_interpol

En esta carpeta se guardan los resultados de las estimaciones del programa kalman.

### resultados

En esta carpeta se guardan los resultados de las proyecciones de los distintos procesos:

<ol> 

#### <li> bd_all_estimacion </li>

Bases consolidada usadas para las estimaciones.

#### <li> baseARIMA </li>

Proyecciones ARIMA

#### <li> baseInterpolacion </li>

Proyeccion usando el metodo de interpolacion

#### <li> baseNowcasting </li>

Proyeccion usando el metodo de nowcast

</ol> 
