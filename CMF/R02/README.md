# R02

Macros para poder visualizar y generar el R02 

## Consideraciones de uso

![image](https://user-images.githubusercontent.com/36990078/150641017-cc1f70a5-e609-4453-a96e-22cff89b4ad5.png)


En la hoja "Inicio", no se deben insertar o eliminar columnas/registros, ya que hay datos como los que se muestran en la imagen superior, 
que se deben mantener en esa posición.

Los archivos deben estar en la misma carpeta donde se encuentre alojada la macros.

* FORMATO NOMBRE DE ARCHIVO

Viene por defecto R02MMYY, en donde R02 siempre debe ir, lo demás se puede cambiar dependiendo de como se genera los archivos en vuestros bancos,
por ejemplo en el banco Z se generan como R021221.dat, en donde R02 es el nombre de la CMF y 1221 corresponde al mes año (MMYY).


* EXTENSION ARCHIVO

Es la extension del archivo, en el caso que en vuestros bancos no tenga extension o tengan otro como .txt, etc.., solo deben cambiar en donde dice ".dat" por ".txt" (sin las comillas)



## Procedimiento de uso

![image](https://user-images.githubusercontent.com/36990078/150641064-19116357-b432-4ee1-b739-88b7329a1800.png)


En la hoja de inicio se encuentra un pequeño paso a paso para visualizar y/o manipular los archivos, en donde:

*  Open R02

Se encarga de importar el archivo R02 en la hojas "01", "02", "03", "04", la hoja "R02" es para poder pivotear los datos.

Nota: Los datos que contienen decimales en el archivo,se deja con decimales en el excel, por ejemplo un campo que contiene informacion 9(01)V9(03) en el archivo se ve 6000,
pero en el excel aparecerá como 6,000

*  Genera R02

Este procedimiento se encarga de tomar la información de las hojas "01", "02", "03", "04" y genera el archivo con el mismo nombre que el original pero agregando un "_FINAL"


## Versiones

# 1.0.0

Primera versión disponible
