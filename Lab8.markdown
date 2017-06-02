##            Laboratorio 08 - Modelado por homologia
_____________

#####Nombre: Cristian Valdebenito


###  **Parte 1: Selección de templados por puntaje DOPE.**
  
![Dope](https://cloud.githubusercontent.com/assets/28108405/26705996/e22af8e0-4707-11e7-8fc9-db6610acd9ff.JPG "Puntaje dope")

*Se seleccionó el target_4.pdb como el mejor templado y                 target_3.pdb con el peor. Se cargarón ambas secuencias en el programa VMD con el fin de realizar un multiseq.*

### **Parte 2: Modelamiento por homologia**

**Sección 1.- Modelamiento por homología de la cadena A de 3LRX con el mejor templado.** En las imágenes se observa la superposición del templado target_4 con la estructura de la proteína 3RLX reportada en protein bank, se observa que a pesar de ser congruente en la mayor parte de las secciones, en otras se observan diferencias en la disposición espacial de loops que unen las hélices de la proteína, siendo estas últimas similares entre el templado y la originalmente reportada.

![4.1](https://cloud.githubusercontent.com/assets/28108405/26706222/b0f20726-4709-11e7-8297-7445c672632f.JPG "")

![4.2](https://cloud.githubusercontent.com/assets/28108405/26706343/9a761fc2-470a-11e7-88d7-fde769411879.JPG "")

![4.3](https://cloud.githubusercontent.com/assets/28108405/26706347/a5ca7b0c-470a-11e7-865f-46fb1771d82a.JPG "")

![4.4](https://cloud.githubusercontent.com/assets/28108405/26706349/af6f77ca-470a-11e7-9f2a-4f0e79d66628.JPG "")


**Sección 2.- Modelamiento por homología de la cadena A de 3LRX con el peor templado.** En las imágenes se observa la superposición del templado target_3 con la estructura de la proteína 3LRX reportada en protein blank, se observa que hay congruencia en ciertas secciones mientras que en otras la diferencias es muy visible, variando la disposición espacial de loop y de estructuras secundarias como sabanas beta y hélices alfa, determinando de esta manera que el templado no tiene mayor congruencia con la proteína originalmente reportada.
        
![3.1](https://cloud.githubusercontent.com/assets/28108405/26706688/49b7201a-470d-11e7-815f-ed049169c9e2.JPG "")

![3.2](https://cloud.githubusercontent.com/assets/28108405/26706698/54906b4a-470d-11e7-9e41-d3ba1759d3f1.JPG "")

![3.3](https://cloud.githubusercontent.com/assets/28108405/26706713/64d774a8-470d-11e7-9b99-d9460f3ddb98.JPG "")

![3.4](https://cloud.githubusercontent.com/assets/28108405/26706721/70fc4916-470d-11e7-962d-1cb6ae235217.JPG "")


##Comparación.

Al comparar la homologia se observa que target_4 es un mejor modelo de templado debido a que no interfiere de forma abrupta en las estructuras secundarias de las proteinas. A pesar de que de igual manera interfiere en la disposición espacial del peptido, este no se ve mayoritariamente comprometido en su estructura, a diferencia del templado target_3 el cual interfiere de una manera significativa en las estructuras secundarias en general de la proteína. De esta manera se puede observar representativamente la direfencia entre un templado que posee puntaje DOPE considerado bueno dentro de los rangos con uno de una escala mayor que es considerado mas erroneo. 