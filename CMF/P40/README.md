# P40

Macros para poder visualizar y generar el P40

## Consideraciones de uso

![image](https://user-images.githubusercontent.com/36990078/152659344-a40a9833-7172-404c-b2a9-e5b2ce1fff60.png)


En la hoja "Inicio", no se deben insertar o eliminar columnas/registros, ya que hay datos como los que se muestran en la imagen superior, 
que se deben mantener en esa posición.

Los archivos deben estar en la misma carpeta donde se encuentre alojada la macros.

* FORMATO NOMBRE DE ARCHIVO

Viene por defecto P40DDMM, en donde P40 siempre debe ir, lo demás se puede cambiar dependiendo de como se genera los archivos en vuestros bancos,
por ejemplo en el banco Z se generan como P403112.dat, en donde P40 es el nombre de la CMF y 3112 corresponde al dia mes (DDMM).


* EXTENSION ARCHIVO

Es la extension del archivo, en el caso que en vuestros bancos no tenga extension o tengan otro como .txt, etc.., solo deben cambiar en donde dice ".dat" por ".txt" (sin las comillas)



## Procedimiento de uso


![image](https://user-images.githubusercontent.com/36990078/152659374-7f888e5d-da2a-4aa6-99a5-324b54fe6c88.png)


En la hoja de inicio se encuentra un pequeño paso a paso para visualizar y/o manipular los archivos, en donde:

*  Open P40

Se encarga de importar el archivo P40 en la hojas "01", "02", "03", la hoja "P40" es para poder pivotear los datos.

Nota1: Los datos que contienen decimales en el archivo, se deja con decimales en el excel, por ejemplo un campo que contiene informacion 9(02)V9(04) en el archivo se ve 060000,
pero en el excel aparecerá como 6,0000

Nota2: Los campos "Nominal Inicial" (Campo 16), "Nominal Actual" (Campo 17) y "Valor par" (Campo 23) del registro 1, se tratan como **string** o **campos de texto** en la importación, 
ya que el excel aguanta creo 15 digitos, Como todos estos campos son de largo 18 (14 enteros y 4 decimales), al importarlos como numerico el excel los redondeaba.

*  Genera P40

Este procedimiento se encarga de tomar la información de las hojas "01", "02", "03" y genera el archivo con el mismo nombre que el original pero agregando un "_FINAL"

## Versiones

# 1.0.0

Primera versión disponible
