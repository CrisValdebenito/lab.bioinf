##            Laboratorio 10 - Análisis	de	simulación	molecular
_____________

#####Nombre: Cristian Valdebenito


###  **Parte 1: Plugins VMD.**
  
1. RMSD Tratectory tool

    Es un plug-in cuyo objetivo es añadir mayor soporte a los cálculos y alineación de las trayectorias al plug-in RMSD. Sus principales funciones son: cálculo de rmsd en trayectorias, alinear marcos en la trayectoria, ajustes iterativos, intercambio de funcionamiento entre átomos equivalentes, generar estadísticas básicas (media, desviación estándar, mínimo y máximo) y resalte de átomos equivalentes de la selección rmsd.

        RMSD es la medida de la distancia media entre los átomos de proteínas
        superpuestas donde se mide habitualmente la similitud en la 
        estructura tridimensional por la RMSD de las coordenadas atómicas 
        después de la superposición óptima del cuerpo rígido. 


2. El plug-in NAMD Energy proporciona comandos tanto una interfaz de usuario gráfica y de texto para la evaluación de las energías utilizando NAMD. NAMDEnergy aplicará los cálculos de energía deseadas a cada trama de la molécula seleccionada, a menos que se selecciona un parámetro de salto marco diferente.

        NAMD (Nanoscale Molecular Dynamics) es un software para simulación de
        dinámica molecular, escrito utilizando el modelo de programación}
        paralelo Charm ++ y se utiliza a menudo para simular sistemas grandes
        (millones de átomos). 

3. El plugin salt bridges permite buscar los puentes salinos formados en una proteína a lo largo de una trayectoria. La búsqueda se puede restringir a una selección y / o un intervalo de trama dada por el usuario.

4. El plugin hBonds cuenta el número de enlaces de hidrógeno formados a lo largo de una trayectoria. La búsqueda puede limitarse a una sola selección o entre dos selecciones distintas, así como una gama trama dada por el usuario.



### **Parte 2: Estabilidad entre la proteína orexina y SUV.** 

*Las orexinas, también llamadas hipocreatinas, son los nombres comunes puestos a un par de hormonas neuropéptidas excitantes que fueron simultáneamente descubiertas por dos investigadores en cerebros de rata. La orexina promueve el estado de vigilia jugando un rol importante del en la influencias metabólicas del ritmo circadiano y de la deuda de sueño para determinar si un animal debe estar dormido o despierto y activo.
Belsombra (suvorexant, SUV), es un medicamento recetado para adultos con problemas para conciliar el sueño y o mantener el sueño, utiliza un enfoque nuevo que bloquea selectivamente los receptores de orexina, que es un neurotransmisor en el cerebro involucrado en la promoción de la vigilia, o el sistema de alerta en el cuerpo.*

*  RMSD Trayectory tool.

![fig1](https://github.com/CrisValdebenito/lab.bioinf/blob/master/Captura.JPG?raw=true "")

           Figura 1. Simulación de las interacciones entre orexina y SUV. Se observa que las 
           interacciones atómicas entre orexina (azul) y SUV (roja) no tiene un punto de 
           fluctuación, teniendo mayor cercanía en angstrom entre los frame 30 y 60 
           aproximadamente.
           

Al analizar el grafico de la simulación de interacción entre la proteína orexina y su ligando SUV, observamos que no hay mayor unión proteína-ligando, debido a que no se aprecia ningún punto de fluctuación entre sus átomos. A pesar de esto se observa que la unión entre ambos, a pesar de no ser “justa” se mantiene estrecha llegando a un mínimo de 0,3 angstrom aproximadamente de distancia entre la proteína y el ligando, dando a entender de que existen fuerzas que permiten su interacción. Esto se puede deducir debido a datos recientes que sugieres que suvorexant interactúa de manera eficiente con la proteína orexina impidiendo su función.

* NAMD energy.

![Fig2](https://github.com/CrisValdebenito/lab.bioinf/blob/master/Captura2.png?raw=true "")

        Figura 2.- Simulación de NAMD energy de proteína orexina y ligando SUV. Se observa en 
        la gráfica dos tipos de energía libre de unión proteína-ligando, en celeste energía 
        electrostática, en azul fuerzas de van der Waals y en negro energía total en kcal/mol.


Al observar el grafico, observamos los datos de energía libre de unión de la proteína orexina a su ligando suvorexant, apreciando que las fuerzas de van der Waals interfieren de manera más espontanea que las energía electrostática en la unión de ambas proteínas, siendo estas uniones no covalentes y relativamente débil, explicando de esta manera la distancia entre los dos compuestos (Fig.1). Por otro lado observamos que la energía libre total es menor entre los frame 30 y 60 aproximadamente, siendo concluyente con la gráfica de distancia de unión, dando a concluir que ambas proteínas no están estrechamente unidas debido a interacciones no covalentes, pero que a su vez la unión ocurre en proceso espontaneo.


* Salt bridges.

Al analizar bajo el plug-in Salt bridges dieron como resultados 14 interacciones de tipo enlace iónico, las cuales fueron obtenidas como archivos .dat los cuales muestran la fuerza de los enlaces en la trayectoria. 

Asp66/Lys2, Asp102/Arg119, Asp162/Arg242, Asp162/Lys241, Glu5/Lys2, Glu69/Arg253, Glu69/Lys2, Glu143/Arg164, Glu143/Lys79, Glu163/Arg242, Glu254/Arg253, Glu287/Lys284, Glu288/Lys32, Glu288/Lys284

![Fig3](https://github.com/CrisValdebenito/lab.bioinf/blob/master/Captura3.JPG?raw=true "")

        Figura 3.- Grafica de energía de puente salino entre aminoácidos Glu134 y Lys79. Se 
        observa la energía de estabilidad entre el enlace iónico de Glu134 y Lys79, teniendo 
        un mayor peak entre los frame 16 y 24.
        

Al observar el grafico observamos la estabilidad del enlace iónico entre los aminoácidos Glu134 y Lys79 pudiendo observar que esta se no se mantiene estable durante la trayectoria, pudiendo asociarlo a la distancia entre el ligando y la proteína (Fig.1) pudiendo observar que existe un rango de distancia óptimo para que el enlace tenga mayor fuerza, pero que este se ve intervenido cuando la distancia de unión es mayor, pudiendo explicarse esta desestabilidad por las fuerzas de Van der Waals. De esto se concluye que los enlaces iónicos son otro tipo de fuerza no covalente que ayuda a la estabilidad de unión entre el ligando y la proteína. A pesar de este no ser tan espontaneo como las fuerzas de Van de Waals, proporcionan a su vez mayor fuerza y estabilidad de unión.


* HBonds.

![Fig4](https://github.com/CrisValdebenito/lab.bioinf/blob/master/Captura4.JPG?raw=true "")

        Figura 4.- Grafica de puentes de hidrogeno formados durante la unión proteína ligando. 
        Se observa la formación de puentes de hidrógenos al interactuar la proteína orexina 
        con el ligando SUV, siendo el valor de 1 como la presencia un puente de hidrogeno y 0 
        como la ausencia.
        

Tras analizar la gráfica de formación de puentes de hidrógenos (Fig.4) observamos que la mayor formación de estos se presenta entre los frames 30 y 70, siendo concluyentes con lo analizado en el figura 1 en cuanto a la distancia entre el ligando y la proteína, concluyendo que a pesar de no tener puntos fluctuantes es estabilizada por otras fuerzas que mantienen su unión estable en el tiempo, siendo estas mayoritariamente fuerzas de Van der Waals, las cuales promueven la unión espontanea, no covalente y estable entre orexina y suvorexant.


####Conclusión. 

*Al analizar la unión entre orexina y sovorexant, observamos que estos no poseen puntos de convergencia entre las distancias, dando a conocer que sus estructuras no están cercanamente unidas, si no que existe un espacio entre ellas. A pesar de estos tras analizar la energía de Van der waal y la energía electrostática electrostáticas en la trayectoria, se pudo determinar que estas conferían una fuerza de unión espontanea entre los frame 30 y 70 donde se producía mayor cercanía entre la proteína y el ligando. A pesar de que el proceso de unión es espontaneo, las fuerzas de Van de Waals no son fuertes, por lo que la estabilidad y la fuerza de unión es conferido por enlaces iónicos y puentes de hidrogeno.*

*Gracias al análisis de pudo determinar que la unión entre orexina y suvorexant es estable en el tiempo, y a su vez de unión transitoria, siendo suvorexant una droga óptima para la inhibición de los receptores de orexina.*