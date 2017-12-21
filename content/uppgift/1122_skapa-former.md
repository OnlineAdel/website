---
author: lew
revision:
    "2017-12-08": (A, lew) First version for v2.
category:
    - oopython
...
Skapa former
===================================

[FIGURE src=/image/oopython/kmom02/skapa-former.png?w=c5 class="right"]

Uppgiften går ut på att med hjälp av klasser, Flask, jinja2 och CSS, skapa former som visas i applikationen. Formerna ska skapas med hjälp av ett formulär och ritas ut i en annan route.

<!--more-->


Förkunskaper {#forkunskaper}
-----------------------

Du har gått introduktionskursen i Python.  
Du har läst artikeln "[GET, POST i Flask](kunskap/flask-get-post)".  
Du har läst artikeln "[Klass relationer](kunskap/klass-relationer)".  



Introduktion {#intro}
-----------------------    

Vi ska leka med former. Vi ska utgå ifrån en basklass och skapa subklasser för olika former. Formerna ska skapas med hjälp av ett formulär och metoden POST. Om man anger fel dimensioner så ska formen inte ritas ut. Värden som ska anges är typ av objekt, bredd (px), höjd (px), positionen (x och y) där formen ska ritas ut samt en bakgrundsfärg. Till varje form ska det finnas en info-ruta där formens höjd, bredd och area ska skrivas ut. Utgå ifrån en basklass, `Shape`, och skapa subklasserna `Square`, `Circle` och `Triangle`.

[YOUTUBE src=X8zYFHdbF3U width=630 caption="Så här kan det se ut när det är färdigt."]


Krav {#krav}
-----------------------

Börja med att skapa routes för uppgiften, en för att skapa former och en för att visa upp dem.

Arbeta i mappen Flask/.

```bash
# Ställ dig i kurskatalogen
cd me/flask/
```

1. Det ska vara möjligt att skapa `Square`, `Circle` och `Triangle`.

1. Alla klasser ska ärva från basklassen `Shape`.

1. Basklassen ska kräva att metoderna `get_area()` och `validate()` implementeras.

1. Varje subklass ska ha sin egna validering. Till exempel så måste höjd och bredd vara samma för att det ska bli en kvadrat eller cirkel.

1. Kommunikationen med klasserna ska skes via en Handler/Controller klass.

1. De ska finnas minst tre färger att välja mellan.

```bash
# Ställ dig i kurskatalogen
dbwebb validate flask
dbwebb publish flask
```

Rätta eventuella fel som dyker upp och validera igen. När det ser grönt ut så är du klar.



Extrauppgift {#extra}
-----------------------

1. Lägg till fler former, tex en [cylinder](https://sv.wikipedia.org/wiki/Cylinder) eller [hyptagon](https://sv.wikipedia.org/wiki/Heptagon).



Tips från coachen {#tips}
-----------------------

Tänk på att det går att använda inline style, tex: `<div style="posistion:absolute;top:10;left:50;">`.

Validera ofta. Så slipper du en massa valideringsfel i slutet av övningen.

Lycka till och hojta till i forumet om du behöver hjälp!