# Balances 2022


Macros para la visualizacion y analisis de los balances que se deben informar a la CMF desde el año 2022


## Consideraciones de uso

![image](https://user-images.githubusercontent.com/36990078/147419447-9f2a5bdb-46d1-469e-a281-a2cebb8a30a0.png)

En la hoja "Inicio", no se deben insertar o eliminar columnas/registros, ya que hay datos como los que se muestran en la imagen superior, 
que se deben mantener en esa posición.

Los archivos deben estar en la misma carpeta donde se encuentre alojada la macros.

* FORMATO NOMBRE DE ARCHIVO

Viene por defecto MXXMMYY, en donde MXX siempre debe ir, lo demás se puede cambiar dependiendo de como se genera los archivos en vuestros bancos,
por ejemplo en el banco Z se generan como MB21121.dat, en donde MB2 es el nombre de la CMF y 1121 corresponde a mes año (MMYY).


* EXTENSION ARCHIVO

es la extension del archivo, en el caso que en vuestros bancos no tenga extension o tengan otro como .txt, etc.., solo deben cambiar en donde dice ".dat" por ".txt" (sin las comillas)


## Procedimiento de uso

![image](https://user-images.githubusercontent.com/36990078/147419500-38280620-ec9f-4fa9-9530-c0d46bf7cd09.png)

En la hoja de inicio se encuentra un pequeño paso a paso para visualizar y/o manipular los archivos, en donde:

### 1) Open MB's

Se encarga de importar los archivos MB4, MB3, etc...

### 2) Copia MB's

Este procedimiento se encarga de tomar la información de las hojas de "MXX Inicial" y los lleva a las hojas "Valida MXX", esto para que puedan manipular los datos.
En las hojas validan van a notar dos bloques, al lado izquierdo de la descripción de los IFRS, es donde se realizan los ajustes, estos ajustes se deben realizar 
en los IFRS de mayor detalle, ya que en lado derecho verán que existen sumatorias para mantener los totales en orden.

Una vez finalizado el ajuste ejecutan el botón corregir totales para que actualice las sumatorias de los IFRS padres.

### 3) Copia MX3

Este procedimiento realiza lo mismo que el anterior, pero para aquellos Bancos que posean sucursales, les recomiendo usar este procedimiento por sucursal que requieran visualizar.

### 4) Normaliza

LLeva los datos desde las hojas "Valida MXX" hacia las hoja de "MXX Inicio", para poder preparar la información para el siguiente procedimiento que es el que genera los archivos.

### 5) Genera MB's

Genera los archivos MXX desde la hoja "MXX Inicio", quedan en el mismo directorio pero añadiendo en el nombre "_Final" para que no se pisen los archivos originales.




## Versiones

### 1.0.0

Primera versión disponible, realizado con el empalme contable de la CMF versión 49591
