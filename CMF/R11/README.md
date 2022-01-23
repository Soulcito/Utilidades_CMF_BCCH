# R11

Macros para poder visualizar y generar el R11 

## Consideraciones de uso

![image](https://user-images.githubusercontent.com/36990078/150664965-30405836-3a35-4865-9223-7154c545732d.png)


En la hoja "Inicio", no se deben insertar o eliminar columnas/registros, ya que hay datos como los que se muestran en la imagen superior, 
que se deben mantener en esa posición.

Los archivos deben estar en la misma carpeta donde se encuentre alojada la macros.

* FORMATO NOMBRE DE ARCHIVO

Viene por defecto R11YYYYMM, en donde R11 siempre debe ir, lo demás se puede cambiar dependiendo de como se genera los archivos en vuestros bancos,
por ejemplo en el banco Z se generan como R11202112.dat, en donde R11 es el nombre de la CMF y 202112 corresponde al año mes (YYYYMM).


* EXTENSION ARCHIVO

Es la extension del archivo, en el caso que en vuestros bancos no tenga extension o tengan otro como .txt, etc.., solo deben cambiar en donde dice ".dat" por ".txt" (sin las comillas)



## Procedimiento de uso

![image](https://user-images.githubusercontent.com/36990078/150664977-94f0fa82-6b84-4a4a-909a-70b7a9fcd5b2.png)


En la hoja de inicio se encuentra un pequeño paso a paso para visualizar y/o manipular los archivos, en donde:

*  Open R11

Se encarga de importar el archivo R11 en la hoja "R11".

*  Genera R11

Este procedimiento se encarga de tomar la información de la hojas "R11"y genera el archivo con el mismo nombre que el original pero agregando un "_FINAL"

## Versiones

# 1.0.0

Primera versión disponible
