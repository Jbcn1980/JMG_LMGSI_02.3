# JMG_LMGSI_02.3



**_DESENVOLUPAMENT_**

Degut a que l'objectiu d'aquesta pràctica és acabar fent un petit joc online, he vist adient donar-li bastant importància a l'aspecte visual, així que el primer que he fet ha estat buscar les imatges.

Les imatges són extretes de https://pixabay.com/, totes tenen llicència Creative Commons CC0. En algunes l'única cosa que he fet ha estat esborrar el fons, en altres he agafat només una part que m'interessava i per últim, l'univers (la capa del fons) l'he fet superposant 2 imatges diferents i modificant algun paràmetre, com la transparència.

Totes les imatges que he creat les he desat a la corresponent carpeta, img, en format png perquè ofereix molt bona qualitat i sobretot perquè permet treballar amb transparències, després d'haver-les comprimit amb https://tinypng.com/; la imatge de background era massa pesada i com que a més no necessitaré transparència en aquesta imatge, aquesta la guardo en jpg. Les imatges originals i els arxius de projecte de photoshop els he guardat en una altra carpeta per si he de fer cap modificació més endavant (no la pujo perquè són gairebé 300 Mb i hi ha arxius massa grans).

Un cop tenia les imatges les he introduït totes en l'arxiu html assignant-lis un div id diferent a cadascuna. Amb aquest div id les he anat col.locant al seu lloc des del css. També des del css li he indicat quina era la imatge de fons i a més li he carregat un background de color negre, així mentres no carrega la imatge de fons no queda el fons en blanc.

A continuació he creat un menú de la mateixa forma, posant el codi mínim al html i després configurant tot des del css. Perquè quedés més integrat he posat el fons transparent. Les opcions inicials al menú eren les següents:
 
- Home
- How to play
- More games
- About us
- Contact

He fet un html nou amb el missatge clàssic 'en construcció', també utilitzant diferents imatges. He afegit una petita secció a la part inferior per tornar a la home. En principi tenia pensat que en el menú d'abans totes les opcions (a excepció del home, que correspon a index.html) redirigissin a aquest mateix html, però he vist que era incompatible amb fer servir l'opció active del menú. He fet varies còpies d'aquest arxiu i les he renombrat amb els noms de les seccions del menú, copiant el codi corresponent al menú i modificant l'opció active.

Fins ara tenim 5 arxius html, home (index.html) i 4 per la resta d'opcions del menú, totes iguals a excepció del menú, que remarca a quina secció de la web estem, i 2 css.

M'ha semblat que tenir un enllaç a la home des de la pròpia home era ridícul a més d'innecesari, i a index.html he modificat el menú respecte a la resta d'html. He aprofitat l'espai de l'enllaç home i on hauria d'estar l'enllaç a la home he posat el play. L'he destacat amb color verd perquè és la senyal d'inici que tenim assimilada pels semàfors, a més destaca sense ser cridaner.

He fet una altra còpia de l'arxiu en construcció i  l'he anomenat play. Ara al fer click al play de la home et redirigeix fins aquí.

A continuació he creat els marcadors que ens donen dades sobre la nau. Volia que fossin ben visibles però sense destacar excessivament. He escollit el gris metàl.lic perquè és elegant i recorda a la vora dels marcadors d'avions o cotxes antics, o també als ordinadors MacBook; tot relacionat amb tecnologia, igual que a un viatge espacial. Els valors inicials de velocitat i alçada els he buscat per internet.

Fins ara he estat treballant amb 2 css, el de la home i el de en construcció. Ara que ja tinc tots els elements col.locats, he fet una còpia de cada css i els he renombrat, així tenia l'original per a pantalles de més de 720px i el que acabava de copiar per poder-lo modificar i ajustar els elements per pantalles de menys de 720px.

No he acabat d'entendre com fer servir l'opció de sprites, per tant he passat directament a la minimificació. He fet una còpia de la carpeta del projecte, així ja tenia tots els html i css inclosos i amb les rutes adeqüades per trobar-se entre ells i trobar les imatges. He anat obrint un per un els html i els css i substituïnt el text pel mateix text minimificat, utilitzant https://www.willpeavy.com/minifier/.

Només ens queda validar el codi de tots els arxius utilitzats, farem els html amb https://validator.w3.org/ i els css amb https://jigsaw.w3.org/css-validator/.

Els css no m'han donat cap problema, en canvi en tots els html he tingut 2 errors:

- The character encoding was not declared. Proceeding using windows-1252
- Bad value 100% for attribute width on element img: Expected a digit but saw % instead

He averiguat que el primer error és degut a que no he introduït un charset al head i que havia d'haver emprat meta charset="UTF-8". Ho he intentat fer però em canvia les proporcions dels elements i ja no sóc a temps d'arreglar-ho, per tant, he preferit que em doni aquests errors però la web tingui un bon nivell estètic, per a la propera pràctica ja sé que és de les primeres coses a fer.

El segon error és perquè el width de img no pot ser un percentatge. Em passa exactament el mateix, al intentar arreglar aquest error em desmunta la pàgina i no sóc a temps d'arreglar-ho.

Ja per últim pujo el projecte al repositori JMG_LMGSI_02.3 de la versió indentada i la versió minimificada a un github branch.

Només em queda per comentar que al llarg de la pràctica he anat visualitzant el resultat tant amb Mozilla Firefox com amb Google Chrome, i a diferents tamanys de pantalla perquè tinc un monitor extern (17") connectat al portàtil (15"). A més, quan ja tenia configurades les media queries també ho comprovava per mòbils i tablets en ambdues orientacions amb f12 de Google Chrome.



**_WEBS CONSULTADES_**

http://fpadistancia.caib.es/course/view.php?id=286

https://www.w3schools.com/

http://es.html.net/tutorials/css/

https://www.jasoft.org/Blog/post/Las-rutas-relativas-en-archivos-CSS.aspx

http://www.esandra.com/usa-una-imagen-responsive-a-pantalla-completa/
