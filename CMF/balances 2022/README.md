# Balances 2022


Macros para la visualizacion y analisis de los balances que se deben informar a la CMF desde el año 2022


## Consideraciones de uso

![image](https://user-images.githubusercontent.com/36990078/148296288-b7535c82-0339-4a0e-9200-55f95c5b0019.png)


En la hoja "Inicio", no se deben insertar o eliminar columnas/registros, ya que hay datos como los que se muestran en la imagen superior, 
que se deben mantener en esa posición.

Los archivos deben estar en la misma carpeta donde se encuentre alojada la macros.

* FORMATO NOMBRE DE ARCHIVO

Viene por defecto MXXMMYY, en donde MXX siempre debe ir, lo demás se puede cambiar dependiendo de como se genera los archivos en vuestros bancos,
por ejemplo en el banco Z se generan como MB21121.dat, en donde MB2 es el nombre de la CMF y 1121 corresponde a mes año (MMYY).


* EXTENSION ARCHIVO

es la extension del archivo, en el caso que en vuestros bancos no tenga extension o tengan otro como .txt, etc.., solo deben cambiar en donde dice ".dat" por ".txt" (sin las comillas)

* CONTADOR PARA SUMA DE TOTALES

Este parametro es usado en el botón "Corrige Totales" de las hojas "Valida MXX", lo que hace es copiar tantas veces hasta el valor del parámetro dado.
Esto es para los ajustes que se hacen y requieren varios niveles de sumatorias de IFRS padres (efecto cascada).

## Procedimiento de uso

![image](https://user-images.githubusercontent.com/36990078/147419500-38280620-ec9f-4fa9-9530-c0d46bf7cd09.png)

En la hoja de inicio se encuentra un pequeño paso a paso para visualizar y/o manipular los archivos, en donde:

*  Open MB's

Se encarga de importar los archivos MB4, MB3, etc...

*  Copia MB's

Este procedimiento se encarga de tomar la información de las hojas de "MXX Inicial" y los lleva a las hojas "Valida MXX", esto para que puedan manipular los datos.
En las hojas validan van a notar dos bloques, al lado izquierdo de la descripción de los IFRS, es donde se realizan los ajustes, estos ajustes se deben realizar 
en los IFRS de mayor detalle, ya que en lado derecho verán que existen sumatorias para mantener los totales en orden.

Una vez finalizado el ajuste ejecutan el botón corregir totales para que actualice las sumatorias de los IFRS padres.

*  Copia MX3

Este procedimiento realiza lo mismo que el anterior, pero para aquellos Bancos que posean sucursales, les recomiendo usar este procedimiento por sucursal que requieran visualizar.

*  Normaliza

LLeva los datos desde las hojas "Valida MXX" hacia las hoja de "MXX Inicio", para poder preparar la información para el siguiente procedimiento que es el que genera los archivos.

*  Genera MB's

Genera los archivos MXX desde la hoja "MXX Inicio", quedan en el mismo directorio pero añadiendo en el nombre "_Final" para que no se pisen los archivos originales.




## Versiones

## 1.0.5

Correccion suma de total 821200100, se modifica en todas las hojas de MCX

## 1.0.4

Correccion suma de total 845250000, se agrega ifrs 845250600 a la suma. Esto en los MCX

## 1.0.3

Se agrega IFRS 845500600 (Pasivos por impuestos diferidos no asociados a diferencias temporales imponibles) en las hojas valida para los MCX

## 1.0.2

Cuando se hace un ajuste en algún IFRS base, el botón "Corrige Totales" de las hojas "Valida MXX", solo estaba corrigiendo la sumatoria del primer nivel, por lo tanto, para corregir los niveles superiores, se tenía que ejecutar varias veces el botón hasta tener todo OK.

Se añadió un parámetro en la hoja de "Inicio" (Celda AI9 ) que es el valor de cuantos ciclos va copiar el procedimiento. Este valor lo pueden cambiar.

## 1.0.1

Correccion de suma en los MB para los siguientes item:

- ACTIVOS POR DERECHO A USAR BIENES EN ARRENDAMIENTO / 175000000
- Otros instrumentos financieros / 123000000
- PASIVOS FINANCIEROS A COSTO AMORTIZADO / 240000000
- Obligaciones con bancos / 244000000
- PATRIMONIO / 300000000


Correccion de suma en los MR para los siguientes item:

- Otros instrumentos financieros / 411450000
- Obligaciones con bancos / 412280000
- Obligaciones con bancos / 416280000
- RESULTADO FINANCIERO POR DAR DE BAJA ACTIVOS Y PASIVOS FINANCIEROS A COSTO AMORTIZADO Y ACTIVOS FINANCIEROS A VALOR RAZO / 432000000
- RESULTADO FINANCIERO POR CAMBIOS, REAJUSTES Y COBERTURA CONTABLE DE MONEDA EXTRANJERA / 433000000
- Resultados por reajustes por tipo de cambio / 433200000
- Colocaciones comerciales / 433250400
- GASTO POR PÉRDIDAS CREDITICIAS / 470000000


# 1.0.0

Primera versión disponible, realizado con el empalme contable de la CMF versión 49591
