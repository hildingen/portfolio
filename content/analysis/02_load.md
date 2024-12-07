Webbplatsers laddningstid och användbarhet
=======================

Uppgiften handlar om att analysera tre webbplatser på deras laddningstid och användbarhet.

Urval
-----------------------

*** 

- [Arken zoo](https://www.arkenzoo.se/)
- [lidl](https://www.lidl.se/)
- [Guldfynd](https://www.guldfynd.se/)

Jag valde att analysera tre "webbutiker" för att med vetskap så innehåller webbutiker mycket bilder som kan påverka laddningstid.

Metod
-----------------------

Pagespeed Insights används i google chrome för att mäta de tre webbplatsernas användbarhet och laddningstid. 
Det kommer väljas ut tre undersidor där det mäts både mobil version och dator version.
Resultaten "Prestanda", "Tillgänglighet", "Bästa metoder" och "SEO" skrivs in in i ett google kalyklark. Värden mäts 1-100 där 100 är bästa resultat.
Varje undersida kommer att inspekteras med "inspect" i google chrome. Under network fliken i inspector kommer sidan laddas om tre gånger och medelvärdet av "load", "MB transferred" och "MB resources" kommer att skrivas in i kalkylarket.

Resultat
-----------------------

*** 

### Arken zoo

![Arken zoo bild](../assets/img/arken-zoo.png)

#### Undersidor
- [Första](https://www.arkenzoo.se/hund)
- [Andra](https://www.arkenzoo.se/valp)
- [Tredje](https://www.arkenzoo.se/kampanj-katt)

#### Möjliga förbättringar

- Skicka bilder i modernare bildformat
- Sätt "width" och "height" på alla bilder
- Använda bilder med rätt storlek

Vi kan med detta se att det finns yttligare åtgärder för just bilder som kan fixas på webbplatsen.

*** 

### Lidl

![Lidl bild](../assets/img/lidl.png)

#### Undersidor
- [Första](https://www.lidl.se/c/veckans-frukt-groent/a10059764?tabCode=Current_Sales_Week)
- [Andra](https://www.lidl.se/c/information/s10017074)
- [Tredje](https://www.lidl.se/c/vara-varor-mejeri-ost/s10018056)

#### Möjliga förbättringar

- Sätt "width" och "height" på alla bilder
- Använda bilder med rätt storlek
- Minska DOM-träd

Vi kan med detta se att det finns optimeringar att göra på både med bilder och DOM-träd.

#### Data som samlades in

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQ-HlLEapBaAen4kMLNZX2TzW7WTXbkz2w1pqIazCFp272nc_mAD235LQLyxXox6XgZZtWk4ukh0y6w/pubhtml?widget=true&amp;headers=false"></iframe>

*** 

### Guldfynd

![Guldfynd bild](../assets/img/guldfynd.png)

#### Undersidor
- [Första](https://www.guldfynd.se/artiklar/herr/kategorier/ringar/)
- [Andra](https://www.guldfynd.se/artiklar/herr/kategorier/ringar/)
- [Tredje](https://www.guldfynd.se/till-barnen)

#### Möjliga förbättringar

- Sätt "width" och "height" på alla bilder
- Använda bilder med rätt storlek
- Minska DOM-träd

Vi kan med detta se att det finns optimeringar att göra på både med bilder och DOM-träd.


Analys
-----------------------

Vi kan se att det finns förbättringar att göra på alla tre webbplatser och det finns liknande möjliga förbättringar för alla tre.
Det som alla tre har gemensamt är att alla bilder inte har någon satt "width" och "height" vilket kan vara en typisk sak för webbshops. Vi kan även se att DOM-träden på Lidl (1188 element) och Guldfynd (2303 element) var väldigt stora och om man skulle lyckas reducera dem något kan det på verka laddningstiden positivt.

Vid analysen av webbplatserna kunde vi se att laddningstiderna för undersidorna varierade någonstans mellan 1-2 sekunder men med lite olika storlek på sidorna. Det som skildje sig åt när vi inspekterade webbplatserna med inspector var storleken på hemsidorna (MB resources). Där sticker gulfynd iväg lite med ett snitt på 10.5 MB medans lidl och och arken zoo ligger mellan 5-8 MB. Trots att Guldfynd har något större resurser på webbplatsen laddar den något snabbare överlag än de två andra webbplatserna. 

#### Rangordning resultat
1. Lidl
2. Guldfynd
3. Arken zoo

Enligt resultatet så rangordnas Lidl först då överlag var det bättre resultat om man slår ihop alla värden. På dator version varierar prestandad mellan 85-97 och tillgängligheten mellan 93-94 vilket är ett väldigt bra resultat. PÅ mobil versionen ligger prestandan mellan 58-75 och tillgängligheten mellan 95-96 vilket också är ett okej resultat. 

I botten hittar vi Arken zoo och det som sänkte resultatet rejält var mobilversion där jag fick fram väldigt dåligt resultat, prestandan varierade mellan 14-27 och tillgängligheten 72-73. På dator versionen får vi en prestanda mellan 25-55 och tillgänglighet mellan 73-74. Om vi jämför detta med Lidl så ser vi en enorm skillnad. 

Guldfynd ligger mitt emellan Lidl och Arken zoo med en prestanda på mobil version mellan 40-45 tillgänglighet mellan 84-85. PÅ datorversionen får vi prestanda mellan 63-74 och tillgänglighet mellan 82-84. 

För mig ligger laddningstiden på 2 sekunder. Över 2 sekunder så tycker jag det är för mycket i vissa lägen och att man då behöver optimera sidan för att få ner laddningstiden. Alla sidor i min analys klarade min gräns och därav ingen kommentar på laddningstiden. 

Övrigt
-----------------------

Skriven av David Hildingsson. 