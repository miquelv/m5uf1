####Característiques de la programació estructurada
#####Claredat

Hi haurà d’haver prou informació al codi per tal que el programa pugui ser
entès i verificat: comentaris, noms de variables comprensibles i procediments
entenedors...


#####Teorema de l’estructura

Demostra que tot programa es pot escriure utilitzant únicament les tres estructures
bàsiques de control:
  * **Seqüència**: instruccions executades successivament, una darrere l’altra
  * **Selecció**: la instrucció condicional amb doble alternativa, de la forma
“si condició, llavors SentènciaA, sinó SentènciaB”.
  * **Iteració**: el bucle condicional “mentre condició, fes SentènciaA”, que
executa les instruccions repetidament mentre la condició es compleixi.

#####Disseny descendent
És una tècnica que es basa en el concepte de “divideix i
venceràs” per tal de resoldre un problema en l’àmbit de la programació. Es tracta
de la resolució del problema al llarg de diferents nivells d’abstracció partint d’un
nivell més abstracte i finalitzant en un nivell de detall.

#####Programació modular
Consisteix en la divisió d’un programa en parts més manejables i independents anomenades **mòduls**.

En la majoria de llenguatges, els mòduls es tradueixen a:
* **Procediments**: són subprogrames que duen a terme una tasca determinada
i retornen 0 o més d’un valor. S’utilitzen per estructurar un programa i
millorar la seva claredat.
* **Funcions**: són subprogrames que duen a terme una determinada tasca i
retornen un únic resultat o valor. S’utilitzen per crear operacions noves que
no ofereix el llenguatge.
___

####Característiques de la programació orientada a objectes

Inconvenients de la programació estructurada:
* Les funcions i procediments comparteixen dades del programa, cosa que
provoca que canvis en un d’ells afectin a la resta.
* Al moment de dissenyar una aplicació és molt difícil preveure detalladament
quines funcions i procediments necessitarem.
* La reutilització del codi és difícil i acaba consistint a copiar i enganxar
determinats trossos de codi, i retocar-los. Això és especialment habitual
quan el codi no és modular.

#####Abstracció
És el procés en el qual se separen les propietats més importants d’un objecte
de les que no ho són. És a dir, per mitjà de l’abstracció es defineixen les
característiques essencials d’un objecte del món real, els atributs i comportaments
que el defineixen com a tal, per després modelar-lo en un objecte de programari.
En el procés d’abstracció no ha de ser preocupant la implementació de cada
mètode o atribut, només cal definir-los.

En la tecnologia orientada a objectes l’eina principal per suportar l’abstracció és la
**classe**. Es pot definir una classe com una descripció genèrica d’un grup d’objectes
que comparteixen característiques comunes, les quals són especificades en els seus
atributs i comportaments.

#####Encapsulació
Permet als objectes triar quina informació és publicada i quina informació és
amagada a la resta dels objectes. Per això els objectes solen presentar els seus
mètodes com a interfícies públiques i els seus atributs com a dades privades o
protegides, essent inaccessibles des d’altres objectes. Les característiques que es
poden atorgar són:
* Públic: qualsevol classe pot accedir a qualsevol atribut o mètode declarat
com a públic i utilitzar-lo.
* Protegit: qualsevol classe heretada pot accedir a qualsevol atribut o mètode
declarat com a protegit a la classe mare i utilitzar-lo.
* Privat: cap classe no pot accedir a un atribut o mètode declarat com a privat
i utilitzar-lo.

#####Modularitat
Permet poder modificar les característiques de cada una de les classes que defineixen
un objecte, de forma independent de la resta de classes en l’aplicació. En altres
paraules, si una aplicació es pot dividir en mòduls separats, normalment classes,
i aquests mòduls es poden compilar i modificar sense afectar els altres, aleshores
aquesta aplicació ha estat implementada en un llenguatge de programació que
suporta la modularitat.

#####Jerarquia
Permet l’ordenació de les abstraccions. Les dues jerarquies més importants d’un
sistema complex són l’herència i l’agregació.

L’herència també es pot veure com una forma de compartir codi, de manera que
quan s’utilitza l’herència per definir una nova classe només s’ha d’afegir allò
que sigui diferent, és a dir, reaprofita els mètodes i variables, i especialitza el
comportament.


#####Polimorfisme
És una característica que permet donar diferents formes a un mètode, ja sigui en
la definició com en la implementació.

La sobrecàrrega (_overload_) de mètodes consisteix a implementar diverses vegades
un mateix mètode però amb paràmetres diferents, de manera que, en invocar-lo, el
compilador decideix quin dels mètodes s’ha d’executar, en funció dels paràmetres
de la crida.

La sobreescriptura (_override_) de mètodes consisteix a reimplementar un mètode
heretat d’una superclasse exactament amb la mateixa definició (incloent nom de
mètode, paràmetres i valor de retorn).
