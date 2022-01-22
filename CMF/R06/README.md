# R06

Macros para poder visualizar y generar el R06 

## Consideraciones de uso

![image](https://user-images.githubusercontent.com/36990078/150652093-74b868c5-037e-4bfc-9ade-384e3c4648ab.png)


En la hoja "Inicio", no se deben insertar o eliminar columnas/registros, ya que hay datos como los que se muestran en la imagen superior, 
que se deben mantener en esa posición.

Los archivos deben estar en la misma carpeta donde se encuentre alojada la macros.

* FORMATO NOMBRE DE ARCHIVO

Viene por defecto R06YYYYMM, en donde R06 siempre debe ir, lo demás se puede cambiar dependiendo de como se genera los archivos en vuestros bancos,
por ejemplo en el banco Z se generan como R06202112.dat, en donde R06 es el nombre de la CMF y 202112 corresponde al año mes (YYYYMM).


* EXTENSION ARCHIVO

Es la extension del archivo, en el caso que en vuestros bancos no tenga extension o tengan otro como .txt, etc.., solo deben cambiar en donde dice ".dat" por ".txt" (sin las comillas)



## Procedimiento de uso

![image](https://user-images.githubusercontent.com/36990078/150652140-2454e9da-b57c-4026-a7a2-4dd53245d58e.png)

En la hoja de inicio se encuentra un pequeño paso a paso para visualizar y/o manipular los archivos, en donde:

*  Open R06

Se encarga de importar el archivo R06 en la hojas "01", "02", "03", la hoja "R06" es para poder pivotear los datos.

Nota: Los datos que contienen decimales en el archivo,se deja con decimales en el excel, por ejemplo un campo que contiene informacion 9(02)V9(03) en el archivo se ve 06000,
pero en el excel aparecerá como 6,000

*  Genera R06

Este procedimiento se encarga de tomar la información de las hojas "01", "02", "03" y genera el archivo con el mismo nombre que el original pero agregando un "_FINAL"


## Versiones

# 1.0.0

Primera versión disponible
