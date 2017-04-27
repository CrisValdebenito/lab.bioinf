##            Laboratorio 04 - Filogenética Molecular
_____________

#####                                    Nombre: Cristian Valdebenito


###  **Parte 1: Plataforma phylogeny.fr y preparación de datos**
  


   

1. ¿Qué cosas ofrece este portal? 
        

        
        Phylogeny.fr es un portal de alto rendimiento que ofrece programas para el análisis filogenético de manera integral y ‘‘pipeline’’ flexibles.
        
2.  ¿Para qué tipo de usuario está diseñado?
        
        Phylogeny.fr está diseñado para ayudar a biólogos que no tienen experiencia en el análisis de filogenias, ayudando de esta manera a analizar sus datos de una manera robusta.

3. Menciona 5 tipos de análisis que se pueden realizar en el portal de acuerdo a la documentación

        Se pueden realizar los siguientes tipos de análisis.
        Alineamiento múltiple: MUSCLE. T-Coffee, ClustalW y ProbCons
        filogenia de secuencias: PhyML, TNT, BioNJ y MrBayes.
        Tree viewers: TreeDyn, Drawgram, Drawtree y ATV
        Alineamiento refinado: Gblocks y Jalview.
        Búsqueda de secuencias homologas: Blast 




###  **Parte 2: Filogenia del gen SRY.**

***Filogenia n°1: ProbCons, GBlocks, MrBayes, y TreeDyn***


![filogenia 1](https://github.com/CrisValdebenito/lab.bioinf/blob/master/phylo_tree.png "Filogenia N°1")


***Filogenia n°2: ClustalW, "Remove positions with gaps", TNT, y TreeDyn***

![filogenia 2](https://github.com/CrisValdebenito/lab.bioinf/blob/master/img2.png "Filogenia N°2")



1. ¿A qué se refiere el paso de *Alignment curation* y para qué sirve?


        Aligment curation consiste en parámetro de análisis de los diferentes alineamientos producidos por un grupo de secuencias que determina las posiciones que están mal alineadas, rellenando con GAPs, y regiones que divergen con el fin de obtener un análisis filogénico más preciso debido a la base biológica con la que se cuenta.


2. ¿Cuál es la diferencia entre BioNJ y Neighbor? (Pista: revisa la documentación) 
        
        La diferencia entre BioNJ y neighbor recae en la limitación en cuanto a las taxas que pueden analizar, siendo BioNJ mayor (<5000 taxas) en relación a neighbor (<500 taxas).

3. Corre de nuevo las filogenias pero esta vez sin *Alignment curation*. ¿Cuál es el efecto en las filogenias?

        Al desactivar ‘aligment curation’ la filogenia varia parcialmente, enlazando nuevas especies y variando de número de división de estos. Al compararlo por la filogenia realizada anteriormente esta varia, pero no completamente ya que se mantienen unidas algunas especies relacionadas evolutivamente. Por otro lado la relación evolutiva de las distintas especies se ven alteradas siendo la mas representativo la del homosapiens, que al usar ClustalW sin Aligment curation se observa que es una especie menos evolucionada del el caballo.

4. Describe las diferencias entre las filogenias que has estimado: cantidad de grupos mono-fileticos, relaciones que potencialmente cambiaron, etc.

        Al comparar las filogenias obtenidas con (ProbCons, GBlocks, MrBayes, y TreeDyn) y la obtenida con (ClustalW, "Remove positions with gaps", TNT, y TreeDyn) nos damos cuenta que la filogenia realizada con ProbCons posee menos cantidad de grupos mono-fileticos en comparación a la de ClustalW al igual que ciertas relaciones, siendo la más notoria la integración de Gavia stellata un ave de la familia de las gaviotas a un grupo mono-filetico (filogenia ClustalW) donde predominaban especies mamíferas. Por otro lado la filogenia ProbCons muestra datos de relación entre las diferentes especies que permite un análisis más fácil y demostrativo a diferencia de ClustalW. Por otro lado las relaciones evolutivas varían mucho en ambas filogenias, tomando como ejemplo el Odobenus rosmarus, el cual en ClustalW se observa menos evolución que en ProbCons.
        Esta incongruencia entre ambas filogenias puede deberse a las diferencias de matrices que utiliza cada programa para realizarlas, pero lo que más destaca al analizar las filogenias realizadas con Aligment curation como las que no, es el observar el papel importante que juega está en la distribución de los arboles filogenéticos. Esto se puede deber a que al ‘’curar’’ los alineamientos se elegirá el que tenga más sustentabilidad biológica y un puntaje alto, de esta manera acertando de manera más indicada a la realidad de la organización evolutiva que ha ocurrido.