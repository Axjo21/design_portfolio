
Hur kan bildintensiva sidor förbättra sin laddningstid och användbarhet?
=======================
Denna analys försöker ta reda på hur bild- och/eller video-intensiva sidor hanterar sitt innehåll, ifall innehållet påverkar sidans prestanda negativt samt eventuella förbättringsmöjligheter. 
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

Sidornas allmänna prestanda och användbarhet kommer också analyseras genom Dev-tools Network för att närmare se hur lång tid sidan tar att ladda, hur många resurser den laddar in samt sidans totala storlek. 


Resultat
-----------------------
<div class="embed-container">
    <iframe class="iframe" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vR0IHwt2tLPGaC0fRYermaFoLnNI4wrLKaaWs8t2DFEU10Ik29PN4-1xBfRdzjyf1lHyhvm2cLMWGjD/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false" title="Reasearch Data" frameborder="0" allowfullscreen>
    </iframe>
</div>

## Övre delen av arket specificerar sidornas resultat för SpeedPage Insights
Sidornas resultat var snarlika. Endast British Museum fick en godkänd snittprestanda på dator. IMDb var nära att lyckas på datorn och National Geographic fick ett dåligt snittvärde. Samtliga sidor fick ett misslyckat resultat på mobilen. 

Trenden för samtliga sidor var att lyckas bra med bland annat First Input Delay och First Contentful Paint, och mindre bra med Largest Contentful Paint samt Interaction to Next Paint.

Trenden var även att samtliga sidor hade bättre optimering för dator än för mobila enheter.
Det som var mest utmärkande med resultaten var att National Geographic fick ett bättre resultat på både LCP (Largest Contentful Paint) och CLS (Cumulative Layout Shift) på mobilen jämfört med datorn. 
## Nedre delen av arket specificerar sidornas resultat för Devtools Network
British Museum var den klara vinnaren för Devtools analysen med 8 gånger så snabb laddningstid. Däremot laddade de även in avsevärt färre resurser och sidans totala storkek var mindre än de andra.

Analys
-----------------------
Det ligger i samtliga sidors intresse att optimera både prestanda och användbarhet. 

Då samtliga sidor är bildintensiva bör de tillämpa bild och video optimering. Med det sagt får man inte glömma att eftersom sidornas innehåll utmärks av bilder så är det även i deras intresse att visa upp så skarpa och högkvalitativa bilder som möjligt. Det handlar alltså om att hitta en balans mellan bildkvalité och sid-prestanda.

## National Geographic
 <a href="%base_url%/image/national_geographic.png" target="_blank" aria-label="View image in original size.">[View Image...]
    <picture>
        <source media="(max-width: 375px)" srcset="%base_url%/image/national_geographic.png?save-as=jpg&q=60&w=374">
        <img src="%base_url%/image/national_geographic.png?save-as=jpg&q=60&w=1000" alt="Nat-Geo">
    </picture>
</a>
National Geographic bör reducera JavaScript som inte används. Eftersom National Geographic fick ett dåligt LCP värde så bör de optimera innehållet genom att förslagsvis spara bilderna som .jpg eller använda en lägre bildkvalite för att öka prestandan. National Geographic bör även förbättra deras Interaction to Next Paint värde, något som är viktigt för användarvänligheten. 

## British Museum
 <a href="%base_url%/image/british_museum.png" target="_blank" aria-label="View image in original size.">[View Image...]
    <picture>
        <source media="(max-width: 375)" srcset="%base_url%/image/british_museum.png?save-as=jpg&q=60&w=374">
        <img src="%base_url%/image/british_museum.png?save-as=jpg&q=60&w=1000" alt="British-Museum">
    </picture>
</a>
British Museum bör skicka med bilder i ett modernare bildformat.
Utöver Largest Contentful Paint fick British Museum ett bra resultat på samtliga mätområden.
British Museum fick bäst resultat, men å andra sidan så laddas det inte in lika många resurser som för de andra sidorna. 

Alltså; även fast de fick ett bra resultat så är det viktigt att hålla sidan uppdaterad. 

## IMDb
 <a href="%base_url%/image/imdb05.png" target="_blank" aria-label="View image in original size.">[View Image...]
    <picture>
        <source media="(max-width: 375)" srcset="%base_url%/image/imdb05.png?save-as=jpg&q=60&w=374">
        <img src="%base_url%/image/imdb05.png?save-as=jpg&q=60&w=1000" alt="imdb">
    </picture>
</a>

IMDb bör minska serverns första svarstid.
IMDB använde ett flertal iframe videos, både deras iframes och bilder bör optimeras. Att sänka kvaliten på bilderna är något som de bör överväga då de inte gör reklam för filmerna och inte heller har som huvudsyfte att visa upp högkvalitativa bilder, till skillnad från National Geographic. 

Då det ligger i National Geographics intresse att visa högkvalitativa bilder hade ett alternativ kunnat vara att helt enkelt minska sidans totala innehåll eftersom det är den största sidan bland urvalet. 

## Slutsats
Vinnare för denna analys var British Museum, därefter kom IMDb och sist kom National Geographic. 

Ifall sidorna haft lika mycket innehåll hade deras resultat varit snarlikt, och de hade alla misskyckats med att nå PageSpeed Insights standard för en snabb sida. Detta visar på hur krävande bilder kan vara på en websida och vilken utmaning det kan vara att optimera bilder. 

Själv upplever jag sidor med laddningstid under 2s som snabba. Man märkte en markant skillnad på British museums och de andras laddningstid. Endast British Museum klarar 2s laddningstiden. 

Övrigt
-----------------------
I ett fortsatt arbete av en liknande rapport hade undersökningen kunnat inkorporera en större mängd verktyg, samt ytterligare tekniker som att inspektera källkoden för att åstadkomma en ännu utförligare analys. 

PageSpeed Insights är ett bra verktyg, men i mitt arbete märkte jag en del brister. Bland annat visades olika värden (2,9s jämfört med 11,2s) för Largest Contentful Paint på två platser i diagnosen för samma sida och enhet. 


### Denna analys skapades självständigt av mig, Axel Jönsson.
