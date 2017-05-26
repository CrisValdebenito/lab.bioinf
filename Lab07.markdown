##            Laboratorio 07 - Visualización de proteínas usando VMD
_____________

#####                                    Nombre: Cristian Valdebenito


###  **Parte 1: Representación de sistema de canal de potasio en membrana**
  


   

1. Obtén una representación similar a la del sistema de ubiquitin, separando proteína (cada cadena de un color distinto), lípidos, iones y agua en distintos métodos de dibujos, materiales y colores.
        

   ![Modelo](https://cloud.githubusercontent.com/assets/28108405/26471695/bcfbc2e4-4170-11e7-80ac-5ef5c96b8ae6.JPG "") 
        
        
2.  Genera una triple mutante en el sistema de canal de potasio, indica cuales son. Adjunta una captura de la ventana Display, Graphical Representation y Mutator, a tu informe comparando el sistema “wild type” con el mutado, contando los átomos de la proteína, ¿A que se debe la diferencia?. Verifica si el centro de la proteína cambia o no, ¿porque?

**Mutaciones.**
    
![mut1](https://cloud.githubusercontent.com/assets/28108405/26471783/1c0529e2-4171-11e7-98b7-2df9d98b59e1.JPG "")

![Mut2](https://cloud.githubusercontent.com/assets/28108405/26471804/3705a9ec-4171-11e7-8f28-f2881a0ad3a6.JPG "")

![Mut3](https://cloud.githubusercontent.com/assets/28108405/26471966/0ca4bef8-4172-11e7-9d96-1c5d82c70d29.JPG "")


 
 
* **Proteina Wild Type**
  
![wt](https://cloud.githubusercontent.com/assets/28108405/26471832/57a6e580-4171-11e7-9d70-c1b2e839057f.JPG "")

*    **Proteina mutada.**

![Mut](https://cloud.githubusercontent.com/assets/28108405/26471846/6cd3dc6a-4171-11e7-9def-d8302d53bbbf.JPG "")


   El numero de átomos ***Wild-Type*** fue de 6284 mientras que el de la mutante fue 6332, este aumento se debio a que los aminoácidos mutados poseián mayor cantidad de átomos en comparacion a los nativos conllevando a un aumento del numero total de atomos de la proteina. 

Por otro lado al evaluar el centro de la proteina se observarón los siguientes valores: 

 **Centro de triple mutante:**

        X: 0.0011918825330212712  

        Y: 0.0003472855023574084   

        Z: 5.610673427581787             

**Centro de Wild-Type:**
                            
        X: 0.0011920753167942166 

        Y: 0.0003518479934427887

        Z: 5.622564792633057

El cambio del centro de proteina se debe a que al generar mutaciones de aminoácidos estos alterarán la distribución espacial debido a los atomos que los componen, difiriendo de esta manera los valores espaciales entre WT y mutante.
    
 
       

3. ¿Qué tipos de iones hay? ¿Cuantos hay de cada tipo?

        Hay dos tipos de iones en el sistema, cloruro (Cl) y potasio (K)
        sumando un total de 70 iones, los cuales para Cl son 41 y para K
        son 29.

4. ¿Cuantos átomos de la selección “waters and name OH2” hay? ¿Cuántos átomos de la selección “waters” hay? ¿A qué se debe la diferencia de números? ¿Cuántas moléculas de agua tiene el sistema?

        Al seleccionar “waters and name OH2”, este da un total de 8.818
        átomos de agua, mientras que al seleccionar “waters” este nos
        dio un valor de 26.454. Esta diferencia se debe a que al
        seleccionar “waters and name OH2” el sistema nos dará el valor
        de las moléculas de aguas formadas por los átomos de oxigeno e
        hidrogeno, mientras que al seleccionar solamente “waters” nos 
        dará la suma total de átomos de oxigeno e hidrogeno que se
        encuentran en el sistema. Una manera de comprobar esto es
        multiplicando 8.818 por tres, que corresponde al número de
        átomos que conforman la moléculas de H2O el cual nos dará el
        valor de los átomos de agua (oxigeno/hidrogeno), de esta manera
        se puede determinar que 8.818 es el número de moléculas de agua
        en el sistema. 
     
  
5. ¿Cuántos átomos existen en la membrana lipídica? ¿Cuántas moléculas de POPC hay?

        Existen 14.472 atomos en la membrana lipídica de los cuales 108
        corresponden a la molecula POPC la cual es un componente
        principal de la bicapa lipídica.
        
6. ¿Cuántas moléculas de agua hay a 3 angstrom de la proteína?

        Hay un total de 510 moleculas de agua a 3 angstrom de la
        proteína. 
        CONSOLA TK: set agua [atomselect top "waters and name OH2 and
        same residue as within 3 of protein"]
        
7. Indique resname, resid, chain de los residuos que se encuentran a 6 angstrom de index 34980. (PISTA: considerar que la selección solo debe tomar atomos name CA de los residuos).

        ResName	ResID	Chain
        ALA 	 29    	  D
        GLY	     30	      D
        ALA      31	      D
        ALA	     32	      D
        THR      33	      D
        VAL	     34	      D
        LEU	     35    	  D
        LEU	     36	      D
        VAL	     37	      D
        SER	     102	  D


        