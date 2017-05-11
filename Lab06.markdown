##            Laboratorio 06 - Visualización de Proteínas usando VMD
_____________

#####                                    Nombre: Cristian Valdebenito


###  **Parte 1: Actividad en clase.**
  


   

1. Señale el método experimental por el cual se resolvió la estructura de la proteína 1OS1 y la resolución que tiene. 
        
        El método experimental con el cual se resolvió la estructura de la
        proteína 1SO1 fue es de difracción de rayos X con una resolución de
        1.8 Å.
        
2.  Identifique las moléculas cristalizadas en el PDB, (PISTA: proteínas, moléculas orgánicas, ligando, agua, iones, etc.).

        Se identificaron cuatro ligandos, los que corresponden a 
        adenosin-5’-trifosfato, ácido pirúvico, ion calcio y ion magnesio. 

3. Identificar aminoácidos cercanos (4 angstrom) al residuo 20 de la proteína. Señalar código de 3 letras y número de residuo del aminoácido (Ej: Lys45, Val87, etc.).

        Se identificaron 9 residuos de aminoácidos.
        PRO9, ASP22, LEU118, LYS116, VAL20, SER18, ASP19, LE17, HIS21.
 

4. Señale el número de moléculas de agua del sistema si las hubiese.


        Tk Console: set AGUA [atomselect top "waters"]
                    $AGUA num.
        Se identificaron 260 moléculas de agua en el sistema.



5. ¿Cuál es el centro de la molécula de ATP? 
        
        El centro de la molécula de ATP está localizado en las siguientes 
        coordenadas.
        X: 28.141870498657227 
        Y: 10.711871147155762 
        Z: 13.21480655670166


6. Indique el tamaño (x, y, z) de todo el sistema.

        El tamaño total de todo el sistema tiene las siguientes coordenadas:
            X1: -4.01800012588501              X2: 69.56400299072266 
            Y1: -27.242000579833984            Y2: 29.253999710083008 
            Z1: -19.19300079345703             Z2: 37.26100158691406

        X: 73.58200311660767
        Y: 56.496000289916992
        Z: 56.45400238037109


7. ¿Cuáles son los aminoácidos ubicados a 3 Å de la molécula PYR?

        Graphics → Representation→ selected atoms: protein and same residue 
        as within 3 of resname PYR
        
        Los aminoácidos ubicados a 3 Å de la molécula PYR son:
        ARG65, TYR207.

8. Señale la distancia entre los carbono alfa (name CA) de los aminoácidos Gln34 y Thr8.


        La distancia entre el carbono alfa (name CA) de los aminoácidos 
        Gln34 y Thr8 obtenida de VMD es de 23,61.

9. Indique la descripcion (name, type, index, residue, resname, resid, chain, x, y, z) del atomo “serial 3391”

        Name: NE1
        Type: NE1
        Residue: ---
        Resname: TRP
        ResID: 443
        Localización:
            X: 23,735
            Y: 19,156
            Z: 6,034
10. Indique que ion se encuentra más cercano al ATP y señale las distancias correspondientes (PISTA: Considerar el ultimo fosforo del ATP name PG). 

        Los iones que se encuentran más cercanos al ATP son el Ca, con una     
        distancia de 3,556 y Mg con 3,730.