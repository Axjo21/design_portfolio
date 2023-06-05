Vad utmärker en sida med bra laddingstid och användbarhet?
=======================
Denna analys försöker ta reda på hur bild- och/eller video-intensiva sidor hanterar sitt innehåll, ifall innehållet påverkar sidans prestanda negativt samt möjliga förbättringsmöjligheter. 
Prestandan och användarvänligheten kommer att mätas enligt "Core Web Vitals" mätvärden. 

Urval
-----------------------
De sidor som analyseras i detta dokument är:
- [National Geographic](https://www.nationalgeographic.com/)
- [British Museum](https://www.britishmuseum.org/)
- [IMDb](https://www.imdb.com/)

Rapportens urval av sidor tog sin början i ett mål att analysera bild- och video-intensiva hemsidor. Jag ville undersöka sidor som hade
något gemensamt och som var snarlika på något sätt. Jag landade i att välja British Museum, National Geographic och IMDb eftersom de är alla välkända sidor som kan förväntas underhållas och förbättras med tidens gång.


Metod
-----------------------
Undersökningen bygger på prestanda-diagnoser genom verktyget "PageSpeed Insights" som mäter mot CWV (Core Web Vitals) standarden. 
Varje sida analyseras med hjälp av verktyget tre gånger och utifrån resultaten jobbar jag mot ett snittvärde för varje sida. Sidorna testas utifrån dator-baserade klienter samt mobila enheter.
Sidornas allmänna prestanda och användbarhet kommer också analyseras genom Dev-tools network, för att närmare se hur lång tid sidan tar att ladda, hur många resurser den laddar in samt sidans totala storlek. 


Resultat
-----------------------
Sidornas resultat var snarlika. Endast British Museum fick en godkänd snittprestanda på dator. IMDb var nära att lyckas på datorn och National Geographic fick ett dåligt snittvärde. Samtliga sidor fick ett misslyckat resultat på mobilen. 
Trenden för samtliga sidor var att lyckas bra med bland annat First Input Delay och First Contentful Paint, och mindre bra med Largest Contentful Paint samt Interaction to Next Paint.


### National Geographic
![National Geographic](../assets/img/national_geographic.png)
Trenden var även att samtliga sidor hade bättre optimering för dator än mobila enheter.
Det som var mest utmärkande med resultaten var att National Geographic fick ett bättre resultat på både Largest Contentful Paint och Cumulative Layout Shift på mobilen jämfört med datorn. 

### British Museum
![British Museum](../assets/img/british_museum.png)


### IMDb
![IMDb](../assets/img/imdb05.png)




Analys
-----------------------
Det ligger i samtliga sidors intresse att optimera både prestanda och användbarhet. Sidorna bör tillämpa 
Med det sagt så får man inte glömma att 
IMDB använde ett flertal iframe videos. 


Övrigt
-----------------------
För en mer utförlig analys hade man behövt använda mer än ett verktyg.
PageSpeed Insights är ett bra verktyg, men i mitt arbete märkte jag en del brister. Bland annat visades olika värden (2,9s jämfört med 11,2s) för Largest Contentful Paint på två platser i diagnosen för samma sida och enhet. 



Författare av rapport: Axel Jönsson