Un cop s’ha acabat d’escriure el programa, el conjunt de fitxers de text
resultants, on es troben les instruccions, es diu que contenen el **codi font**.
Aquest codi font pot ser des d’un nivell molt alt, molt a prop del llenguatge
humà, fins a un de nivell més baix, més proper al codi de les màquines, com
ara el codi assemblador.

El procés anomenat compilació és la traducció del codi font dels fitxers del
programa en fitxers en format binari que contenen les instruccions en un format
que el processador pot entendre. El contingut d’aquests fitxers s’anomena **codi
objecte**. El programa que fa aquest procés s’anomena **compilador**.

El **codi objecte** és el codi font traduït (pel compilador) a codi màquina, però
aquest codi encara no pot ser executat per l’ordinador.

El **codi executable** és la traducció completa a codi màquina, duta a terme per
l’enllaçador (en anglès, _linker_). El codi executable és interpretat directament
per l’ordinador.

L’ **enllaçador** és l’encarregat d’inserir al codi objecte les funcions de les llibreries
que són necessàries per al programa i de dur a terme el procés de muntatge
generant un arxiu executable.

Una **llibreria** és una col·lecció de codi predefinit que facilita la tasca del programador
a l’hora de codificar un programa.

El concepte de **màquina virtual** sorgeix amb l’objectiu de facilitar el desenvolupament
de compiladors que generen codi per a diferents processadors.

La **compilació** consta de dues fases:
* La primera parteix del codi font a un llenguatge intermedi obtenint un
programa equivalent amb un menor nivell d’abstracció que l’original i que
no pot ser directament executat.
* La segona fase tradueix el llenguatge intermedi a un llenguatge comprensible
per la màquina.

La **màquina virtual Java (JVM)** és l’entorn en què s’executen els programes Java.
És un programa natiu, és a dir, executable en una plataforma específica, que és
capaç d’interpretar i executar instruccions expressades en un **codi de bytes** o (el
bytecode de Java) que és generat pel compilador del llenguatge Java.
