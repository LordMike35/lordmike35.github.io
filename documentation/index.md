---
layout: wp
title: Dokumentácia
---
### Vyjadrenie k požiadavkam zadania
**Podstránky:**
* _/_ - domovská stránka
* _/human_ - opis záujmov mimo informatiky
* _/programmer_ - opis informatických záujmov
* _/contact_ - kontaktné info
* _/wp_ - podstránka na publikovanie zadaní z WP
* _/documentation_ - dokumentácia vzhľadom na zadanie

**Layouty:**
* _default_ - základný layout, do ktorého sa vnárajú iné layouty, jeho súčasťou je header html docu, header, footer ale aj hlavný container
* _welcome_ - jeho súčasťou je fotka a nadpis, použítý na podstránkach contact a domovskej stránke
* _wp_ - layout upozornujuci na asociaciu podstránok s predmetom WP, taktiez meni nastavenia velkosti písma contentu
* _life_ - pridáva na pravu stranu panel fotiek a vo vrchnej náhodne vyberá zo zoznamu idolov, použítý na podstránkach programmer a human

**Pluginy:**
* _jemoji_ - zabezpečuje možnosť používať emotikony :+1:

**Premenné:**
* _page.title_ - viackrát použítá premenná, ktorá vracia nadpis aktuálnej podstránky
* _content_ - napĺňa obsah layoutov
* _site.title_ - vracia nadpis webstránky
* _site.email_, _site.instagram_username_, _site.github_username_ - naše vlastné premenné, ktoré sme si zadefinovali v súbore _config
* _site.time_ - vracia aktuálny dátum, použíté vo footeri
* _idol_, _idol.name_, _idol.description_ - premenná naplnená tagom assign, má v sebe uloženého jedného z idolov, použítá v layoute life
* _site.static_files_ - všetky statické subory stranky, použité v layoute life
* _image.path_ - cesta k obrázku

**Dátové súbory:**
* _idols.csv_ - uchováva v sebe zoznam mien rôznych známych osobností, spolu s ich opisom

**Filtre:**
* _site.data.idols | sample_ - vyberá jedného náhodného idola
* _site.time | date_to_string_ - konvertuje aktuálny čas do stringu

**Tagy:**
* _% assign_ - priradzuje hodnotu nejakej premennej, v šablóne life
* _% for image in site.static_files % % endfor %_ - cyklus prechádzajúci cez všetky súbory
* _% if image.path contains 'images/slider' % % endif %_ - tag kontroluje, či sa obrázok nachádza v priečinku slider 
* _% include header.html %, % include footer.html %_ - includuje obsah súborov do daného súboru

**Štýly:**
* _main.css_ - použili sme jediný style súbor, do ktorého sme postupne vpisovali všetko čo sme potrebovali




