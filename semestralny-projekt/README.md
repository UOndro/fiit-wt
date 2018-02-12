# Semestrálny projekt - eshop

## Zadanie
Vytvorte webovú aplikáciu - eshop, ktorá komplexne rieši nižšie definované scenáre vo vami zvolenej doméne (napr. elektro, oblečenie, obuv, nábytok). Presný rozsah a konkretizáciu scenárov si dohodnete s Vašim cvičiacim na cvičení.


## Termíny odovzdania
* **Odovzdanie 1. fázy projektu: 3. týždeň - 2.3. do 23:59 v AIS, 5 bodov,** vytvorenie skíc jednotlivých stránok pre 3 typy rozlíšení
* **Odovzdanie 2. fázy projektu: 6. týždeň - 23.3. do 23:59 v AIS, 10 bodov (8 + 2 body),** vytvorenie responzívnych šablón na základe vytvorených skíc/predloh (8 bodov); návrh dátového modelu a implementovaný relačný model (2 body)
* **Odovzdanie 3. fázy projektu: 8. týždeň - 6.4. do 23:59, 10 bodov,** implementácia logiky eshopu (server-side rendering) s využitím PHP frameworku (odporúčaný Laravel)
* **Odovzdanie 4. fázy projektu: 11. týždeň - 24.4. do 8:00, 15 bodov,** implementácia chatu (komunikácia v reálnom čase) a jeho integrácia do eshopu (vue.js + node.js) + finálna dokumentácia

## Termíny prezentovania
Študenti prezentujú kontrolné fázy projektu na cvičeniach, a to:
* **Prezentovanie 1. fázy projektu: 4. týždeň - 6.3.**
* **Prezentovanie 2. fázy projektu: 7. týždeň - 27.3.**
* **Prezentovanie 3. fázy projektu: 9. týždeň - 10.4.**
* **Prezentovanie finálneho projektu: 11. týždeň - 24.4. a 13. týždeň - 10.5.**


## Aplikácia - eshop
V poslednom kontrolnom termíne **aplikácia musí pozostávať aspoň z týchto častí**:
* **hlavná stránka** s možnostou vyhľadávania v produktoch (ideálne naprieč celou aplikáciou)
* **zobrazenie prehľadu všetkých produktov** z vybratej kategórie, s možnosťou základného filtrovania, rozumne stránkovaných (ak je to potrebné)
* **stránka s detailom o produkte** s možnosťou vloženia produktu do nákupného košíka
* **nákupný košík** s možnosťou vytvorenia objednávky
    * pozostávajúci aspoň z troch krokov, a to: sumarizácia daných položiek v košíku, výber dopravy a platby, dodacie údaje
* **stránka s výsledkami vyhľadávania**
* **prihlásenie a registrácia používateľa**
* **integrovaný chat** na (realtime) komunikáciu s pracovníkom eshopu
* **administrátorské rozhranie**
  * prihlásenie používateľa
  * stránka na pridanie/upravenie/vymazanie produktu
  * stránka na komunikáciu so zákazníkom/návštevníkom (chat)

**Aplikácia musí realizovať tieto prípady použitia:**

* zobrazenie prehľadu všetkých produktov z vybratej kategórie s možnosťou základného filtrovania, rozumne stránkovaných (ak je to potrebné)
* zobrazenie konkrétneho produktu - detail produktu
    * pridanie produktu do košíka
* zobrazenie nákupného košíka
    * zmena množstva pre daný produkt
    * odobratie produktu
    * výber dopravy
    * výber platby
    * vloženie dodacích údajov
    * dokončenie objednávky
* registrácia používateľa
* prihlásenie používateľa do eshopu
* prihlásenie používateľa do administrátorského rozhrania eshopu
* odhlásenie používateľa
* plno-textové vyhľadávanie v produktoch (angl. full-text search)
    * zobrazenie výsledkov vyhľadávania
* vytvorenie nového produktu cez administrátorské rozhranie
* upravenie existujúceho produktu cez administrátorské rozhranie
* vymazanie existujúceho produktu cez administrátorské rozhranie
* zobrazenie integrovaného chatu na stránkach eshopu
    * vytvorenie správy
    * zobrazenie histórie komunikácie aktuálneho sedenia
* zobrazenie chatu v administrátorskom rozhraní
    * vytvorenie správy
    * zobrazenie histórie komunikácie aktuálneho sedenia

## Dátový model
V druhom kontrolnom termíne sa odovzdáva JPG (JPEG) obrázok logického dátového modelu reprezentovaného UML class diagramom a implementovaný model v SQL databáze - schéma SQL DDL, ktorým sa vytvára (odporúčaný PosgreSQL).

Vo štvrtom kontrolnom termíne sa odovzdáva kompletná databáza, a teda dáta aj schéma. Diagram logického a fyzického dátového modelu bude súčasťou dokumentácie.

## Spôsob odovzdávania
Výstupy všetkých kontrolných bodov sa odovzdávajú do AISu. Databáza sa odovzdáva kompletná (dáta aj schéma, resp. DDL).

Odovzdávajú sa všetky zdrojové kódy aplikácie, okrem samotných rámcov a knižníc z manažéra balíkov (composer, npm). V prípade, že študent modifikoval používanú knižnicu, je potrebné pribaliť aj zmenené knižnicu a uviesť zmenu s odôvodnením v dokumentácii.

Odovzdáva sa ZIP alebo RAR archív.


## Oneskorenie odovzdania
V kontrolnom termíne sa môže odovzdanie oneskoriť maximálne o 3 dni.

Za každý deň oneskoreného odovzdania je študentovi odobratých 25% bodov z pôvodného maxima (deň po termíne študent získa 3/4 bodov, dva dni po termíne 1/2, atď.) 

 Neskoršie odovzdanie nie je možné. Neodovzdanie niektorej časti projektu znamená nesplnenie podmienok absolvovania predmetu.

## Implementačné prostredie
Odporúčané technológie:
* Laravel PHP rámec
* PostgreSQL relačný databázový systém

Povinné technológie pre implementácia chatu:
* Node.js
* Vue.js

Použitie iných technológií, napr. iný PHP rámec alebo relačný databázový systém je podmienené súhlasom cvičiaceho (jazyk PHP je povinný).


## Dokumentácia
Dokumentácia musí obsahovať minimálne tieto časti:
* zadanie
* diagram logického a fyzického dátového modelu spolu s ich opisom
* opis návrhu / návrhové rozhodnutia
* prog. prostredie
* opis implementácie jednotlivých scenárov