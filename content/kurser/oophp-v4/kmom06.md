---
author:
    - mos
category:
    - kurs oophp-v3
    - kurs oophp
revision:
    "2018-02-26": "(PB1, mos) Arbetsmaterial oophp v4."
    "2017-04-28": "(A, mos) Första utgåvan."
...
Kmom06: Enhetstestning
==================================

[WARNING]
**Version 4 av oophp.**

En uppdaterad version av kursen är under bearbetning och kursen ges första gången vårterminen 2018.

[/WARNING]

<!--
Repetition o förbered projektet.
Komplett databas för eshopen.
Mer enhetstestning.
Enhetstestning mot databas?
(travis o codecoverage, scrutinizer, etc. Kanske)
-->

[FIGURE src=image/snapvt17/phpunit.png?w=w3 caption="Enhetstestning med PHPUnit via en Makefile."]

<small><i>(Detta är instruktionen för kursmomentet och omfattar det som skall göras inom ramen för kursmomentet. Momentet omfattar cirka **20 studietimmar** inklusive läsning, arbete med övningar och uppgifter, felsökning, problemlösning, redovisning och eftertanke. Läs igenom hela kursmomentet innan du börjar jobba. Om möjligt -- planera och prioritera var du vill lägga tiden.)</i></small>


<!--stop-->




Läsanvisningar  {#lasanvisningar}
---------------------------------

*(ca: 2-4 studietimmar, inklusive extra läsning i referenslitteraturen efter eget val)*



###Artiklar {#artiklar}

Läs följande.

1. Bekanta dig översiktligt med de olika delarna av manualen i [MySQL om optimering](https://dev.mysql.com/doc/refman/5.7/en/optimization.html). Se vilka delar som kan optimeras och på vilket sätt. Skumma igenom de olika delarna.

1. Bekanta dig kort och översiktligt med [PHPUnits dokumentation](https://phpunit.de/manual/current/en/). Kika över innehållsförteckningen och skumläs kapitel 2 och 3 som ger dig en grov introduktion till hur du jobber med phpunit.

1. Bekanta dig kort och översiktligt med [Xdebug för PHP](https://xdebug.org/) och kika snabbt över vilken dokumentation som finns. Se vilka funktioner Xdebug kan tillföra till din utvecklingsmiljö. Vi kommer enbart använda Xdebug för att PHPUnit behöver det för att generera kodtäckning.



Övningar & Uppgifter  {#ovningar_uppgifter}
-------------------------------------------

*(ca: 12-16 studietimmar)*


###Övningar {#ovningar}

Gör följande övning, den förbereder dig inför uppgifterna.

1. Installera [PHPUnit](labbmiljo/phpunit) och [Xdebug](labbmiljo/xdebug) för att kunna köra enhetstester med kodtäckning på din lokala maskin.

1. Jobba igenom exemplet `example/phpunit/README.md` (i kursrepot) som visar dig grunderna i enhetstester med phpunit och kodtäckning. Kopiera och spara filerna till `me/kmom06/phpunit` så du kan testa skriva ett eget testfall.

<!--
Artikel om hur man skriver bra SQL frågor på ett optimerat sätt.
-->



###Uppgifter {#uppgifter}

Följande uppgifter skall utföras och resultatet skall redovisas via me-sidan.

1. Gör uppgiften "[Skapa enhetstester till Anax Lite](uppgift/skapa-enhetstester-till-anax)". Spara uppdateringarna du gör i ditt `me/anax-lite` och del-uppgiften för `Guess` utför du i `me/kmom06/phpunit`.

1. Pusha och tagga ditt Anax Lite, allt eftersom och sätt en avslutande tagg (6.0.\*) när du är klar med alla uppgifter i kursmomentet.

<!--
1. Gör uppgiften "[Dokumentera din ER-modell med Reverse Engineering](uppgift/dokumentera-din-er-modell-med-reverse-engineering)". Spara resultatet i `me/kmom06/er3`. Det är samma sak som du gjort i föregående kmomentent, det handlar om att få med de uppdateringar du nyss gjort.
-->



Resultat & Redovisning  {#resultat_redovisning}
-----------------------------------------------

*(ca: 1-2 studietimmar)*

Läs [instruktionen om hur du skall redovisa](./../redovisa).

Se till att följande frågor besvaras i texten:

* Har du tidigare erfarenheter av att skriva kod som testar annan kod?
* Hur ser du på begreppet enhetstestning och att skriva testbar kod?
* Hur gick det att hitta testbar kod bland dina klasser i Anax Lite?
* Vilken är din TIL för detta kmom?