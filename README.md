# Librerias de Proyeccion


## Instaladores

Para instalar todas las librerias requeridas para realizar las estimaciones y proyecciones use el programa Instaladores. Solo sera necesario usarlo una vez.

## Programas

Estas librerias realizan el proceso de proyección del PIB en Panama, así como proyecciones para otras variables de interes relevantes. Estas librerias constan de los siguientes archivos:

<ol> 

### <li> Bases de Datos </li>
    
### ConstruccionBasedeDatos

En este programa se construye la base de datos usada para las estimaciones y proyecciones, se calculan los estadisticos descriptivos y als correlaciones.


### <li> Estimaciones ARIMA </li>

### ARIMA

Se realizan la estimacion, proyeccion y evaluacion de los modelos ARIMA.


### <li> Estimaciones Kalman interpolacion </li>

### Kalman

Se realiza la estimacion del modelo Kalman de interpolacion.

### Interpolacion

Se realiza la interpolacion y proyeccion usando el método de Kalman.

### Evaluacion

Se realiza la evaluación del modelo de interpolacion.

### <li> Estimaciones Nowcast </li>

### nowcast

Se estima el modelo de nowcast.

###  nowcast_kalman

Libreria auxiliar.

### proyeccion_nowcast

Se realiza la proyeccion usando el método de nowcast.

</ol> 

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

Bases usadas para las estimaciones.

#### <li> baseARIMA </li>

Proyecciones ARIMA

#### <li> baseInterpolacion </li>

Proyeccion usando el metodo de interpolacion

#### <li> baseNowcasting </li>

Proyeccion usando el metodo de nowcast

</ol> 
    
## Proceso de proyecciones

### Proyeccion mensual - ARIMA

1. Actualice la base de datos dentro de input: bd_Panama
2. Corra el programa ARIMA
3. Los resultados se guardan dentro de resultados con el nombre baseARIMA

### Proyeccion mensual - Interpolacion

1. Actualice la base de datos dentro de input: bd_Panama
2. Corra el programa Interpolacion
3. Los resultados se guardan dentro de resultados con el nombre baseInterpolacion

### Proyeccion trimestral - Nowcasting

1. Actualice la base de datos dentro de input: bd_Panama
2. Corra el programa proyeccion_nowcast
3. Los resultados se guardan dentro de resultados con el nombre baseNowcast