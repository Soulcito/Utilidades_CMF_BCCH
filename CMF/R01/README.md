# R01

Macros para poder visualizar y generar el R01 

## Consideraciones de uso

![image](https://user-images.githubusercontent.com/36990078/148623679-f1577dd3-f636-48be-af00-841d2d4fc4e4.png)


En la hoja "Inicio", no se deben insertar o eliminar columnas/registros, ya que hay datos como los que se muestran en la imagen superior, 
que se deben mantener en esa posición.

Los archivos deben estar en la misma carpeta donde se encuentre alojada la macros.

* FORMATO NOMBRE DE ARCHIVO

Viene por defecto R01YYYYMM, en donde R01 siempre debe ir, lo demás se puede cambiar dependiendo de como se genera los archivos en vuestros bancos,
por ejemplo en el banco Z se generan como R01202112.dat, en donde R01 es el nombre de la CMF y 202112 corresponde al año mes (YYYYMM).


* EXTENSION ARCHIVO

Es la extension del archivo, en el caso que en vuestros bancos no tenga extension o tengan otro como .txt, etc.., solo deben cambiar en donde dice ".dat" por ".txt" (sin las comillas)



## Procedimiento de uso

![image](https://user-images.githubusercontent.com/36990078/148623690-41faa176-86ec-4b4b-a4cf-88a34985493a.png)


En la hoja de inicio se encuentra un pequeño paso a paso para visualizar y/o manipular los archivos, en donde:

*  Open R01

Se encarga de importar el archivo R01 en la hojas "01", "02", "03", "04", la hoja "R01" es para poder pivotear los datos.

Nota: Los datos que contienen decimales en el archivo,se deja con decimales en el excel, por ejemplo un campo que contiene informacion 9(03)V9(03) en el archivo se ve 006000,
pero en el excel aparecerá como 6,000

*  Genera R01

Este procedimiento se encarga de tomar la información de las hojas "01", "02", "03", "04" y genera el archivo con el mismo nombre que el original pero agregando un "_FINAL"


## Versiones

# 1.0.0

Primera versión disponible
