# C17

Macros para poder visualizar y generar el C17

## Consideraciones de uso

![image](https://user-images.githubusercontent.com/36990078/152620140-9d626a75-08d8-4dec-afbc-f7466d72a0bc.png)


En la hoja "Inicio", no se deben insertar o eliminar columnas/registros, ya que hay datos como los que se muestran en la imagen superior, 
que se deben mantener en esa posición.

Los archivos deben estar en la misma carpeta donde se encuentre alojada la macros.

* FORMATO NOMBRE DE ARCHIVO

Viene por defecto C17YYYYMM, en donde C17 siempre debe ir, lo demás se puede cambiar dependiendo de como se genera los archivos en vuestros bancos,
por ejemplo en el banco Z se generan como C17202112.dat, en donde C17 es el nombre de la CMF y 202112 corresponde al año mes (YYYYMM).


* EXTENSION ARCHIVO

Es la extension del archivo, en el caso que en vuestros bancos no tenga extension o tengan otro como .txt, etc.., solo deben cambiar en donde dice ".dat" por ".txt" (sin las comillas)


## Procedimiento de uso

![image](https://user-images.githubusercontent.com/36990078/152620262-4bee3dba-c789-48e5-83fe-4d32c7a7de98.png)


En la hoja de inicio se encuentra un pequeño paso a paso para visualizar y/o manipular los archivos, en donde:

*  Open C17

Se encarga de importar el archivo C17 en la hoja "C17".

*  Genera C17

Este procedimiento se encarga de tomar la información de la hojas "C17"y genera el archivo con el mismo nombre que el original pero agregando un "_FINAL"

## Versiones

# 1.0.0

Primera versión disponible
