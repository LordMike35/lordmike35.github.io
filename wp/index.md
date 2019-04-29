---
layout: wp
title: Webové publikovanie
---
Na tomto mieste budú postupne publikované vypracované zadania z predmetu Webové publikovanie.

[Zadanie 1](https://github.com/LordMike35/LordMike35.github.io) 
### Zadanie 2
#### Postup
Ako dokument sme si vybrali priebežnú správu o Bakalárskej práci. Keďže bola vo formáte pdf a konverter z formátu pdf do formátu xml sa nám nájsť nepodarilo,
ako medzikrok poslúžilo prekonvertovanie do formátu docx. Už pri konvertovaní z pdf do docx sa úprava a formátovanie textu... výrazne vytratilo, avšak
textová časť zostala v uspokojivej podobe. Následne sme jednotlivé xml sekcie prekopírovali na adekvátne miesta do šablóny mojabp.xml.
Vynechali sme pritom určité časti pôvodnej bakalárky, pretože mala priveľa strán. Šablónu mojabp.xml sme premenovali 
na test.xml a pustili sme sa do ručných úprav.

#### Vyjadrenie k celkovému vzhľadu
Kvôli zlému time managementu sa dokument úpravou veľmi nepodobá na pôvodný, avšak myslíme si, že vypracovanie tohto zadania splnilo svoj účel, pretože
sme dokázali korektne použiť všetky požadované konštrukcie a taktiež sme sa dokázali zorientovať v transformačných súboroch a upravili niektoré 
dôležité atribúty.

#### Vyjadrenie k požiadavkám zadania
* **Členenie textu na kapitoly, podkapitoly, prílohy, generovaný obsah..** - splnené v rámci celého dokumentu, 
* **Zvýraznenie slov, odrážky, číslovanie** - používané v rámci celého dokumentu
* **Odkazy na iné časti vlastného dokumentu** - v časti Úvod sa odkazujeme na niektoré kapitoly
* **Poznámka pod čiarou** - keďže v pôvodnom dokumente žiadna nie je, spravili sme jednu testovaciu v časti Úvod
* **Zoznam použitej literatúry a zdrojov vrátane ich citácie v texte** - demonštrácia na začiatku prvej kapitoly
* **Vloženie obrázku a tabuliek, odkazy na ne v texte; zoznam obrázkov a tabuliek v úvode alebo závere textu** - oba zoznamy boli korektne automaticky vygenerované
* **Vytvorenie registra pojmov** - splnené (v pôvodnom dokumente nebol)

### Zadanie 3
#### Postup 
Najskôr bolo potrebné vymyslieť z čoho bude prezentácia pozostávať. Rozhodli sme sa, že urobíme 5 typov slajdov - titulny, obyčajný textový, dvojstĺpcový textový,
slajd s veľkým obrázkom a slajd s dvoma veľkými obrázkami. Následne sme si začali písať DTD validačný súbor a popritom vytvárali príklady na rôzne slajdy.
Celkovo sme vytvorili 8 slajdov, ktorých validnosť sme si overili online nástrojov. 

Pri tvorbe transformačného súboru do XHTML sme sa pokúsili mať napamäti rozumné používanie konštrukcie apply-templates, čo sa nám myslím podarilo. 
Vzhľadom na časovú tieseň a našu neschopnosť v práci s CSS, výsledné slajdy vôbec nevyzerajú dobre (vyzerajú zle), avšak transformácia do html je podľa nášho
názoru spravená korektne. 

#### Vyjadrenie k požiadavkám zadania
* **opis typu dokumentu + opis účelu navrhnutých elementov** - rozhodli sme sa použiť DTD
* **vytvorenie ukážkovej XML prezentácie demonštrujúcej možnosti definície typu dokumentu** - 8 slajdová prezentácia demoštrujúca všetky nami navrhnuté konštrukcie
* **základný návrh XSL transformácií, ich vhodnosť, parametrizácia** - parametrizácia absentuje, vhodnosť necháme na posúdenie iných
* **vytvorenie XSLT pre konverziu prezentácie z XML** -> XHTML+CSS - xhtml sa podarilo, css nie
* **vytvorenie XSLT pre konverziu prezentácie XML -> PDF** - X