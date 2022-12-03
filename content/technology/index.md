---
Title: Technologies
Description: This is our Landing page for technologies.
Template: technologies
---

<div class="all-technologies">

<div class="tech-box tech-title" markdown="1">

# Technologies

</div>



<div class="tech-box tech-html" markdown="1"> 

# [HTML](technology/html)


HyperText Markup Language (HTML) utgör tillsammans med HyperText Transfer Protocol (HTTP) grunden i webben. Webbsidor skrivs i HTML och skickas sedan över internet med hjälp av HTTP.

HTML beskriver innehåll och struktur för våra webbplatser och gör det möjligt att ladda andra dokument till exempel CSS eller JavaScript filer.

HTML använder sig av element beskrivna av taggar. Nedan är ett exempel på ett textstycke med en länk i:


```html
<p>En länk till min <a href="minwebbplats.html">webbplats</a></p>

```

</div>


<div class="tech-box tech-css" markdown="1"> 

# [CSS](technology/css)

Cascading Style Sheets är språk för att beskriva utseende av element i ett markup language till exempel HTML. CSS är en av tre teknologier som utgör fundamentet för webben.

I CSS använder vi selektorer för att beskriva vilka element vi vill påverka och deklarerar sedan stilen för elementen i ett block.

Om vi till exempel vill sätta färgen för alla textstycken till blå gör vi på följande sätt.

```css
p {
    color: blue;
}
```

</div>

<div class="tech-box tech-php" markdown="1"> 

# [PHP](technology/php)

PHP är ett populärt skriptspråk som främst används för att skapa webbplatser med dynamiskt innehåll. PHP är det mest använda server-side programmeringsspråk på webben med uppåt 80% av alla webbplatser som använder det.

PHP är ett objekt-orienterad programmeringsspråk, som med senare versioner kan vara hård typat och till och med JIT.

Ett program som skriver ut alla jämna siffror mellan 1 och 100 kan se ut på följande sätt i JavaScript:

```php
<?php
for ($i = 1; $i <= 100; $i++) {
    if (!($i % 2)) {
        print($i);
    }
}
```

</div>


<div class="tech-box tech-py" markdown="1"> 

# [Python](technology/python)

Python är ett programmeringsspråk som lanserades 1991 av Guido van Rossum. Programmeringsspråket är dynamiskt typad och betecknas som ett generellt programmeringsspråk då det kan tillämpas inom många domäner.

Programmeringsspråket utmärkar sig genom att alla datatyper är baserat på klasser och objekt. En annan aspekt som skiljer Python från andra språk är att indentering används för att särskilja block i koden.

Ett program som skriver ut alla jämna siffror mellan 1 och 100 kan se ut på följande sätt i Python:

```python
for number in range(1, 100 + 1):
    if not number % 2:
        print(number)
```

</div>


<div class="tech-box tech-js" markdown="1"> 

# [JavaScript](technology/javascript)

JavaScript är ett prototyp-baserat skriptspråk. JavaScript utgör tillsammans med HTML och CSS grunden för webben. JavaScript är dynamiskt, svagt typat och hanterar funktioner som första-klass-objekt.

JavaScript använder sig av C-like syntax, men har annars inget gemensamt med programmeringsspråket Java.

Ett program som skriver ut alla jämna siffror mellan 1 och 100 kan se ut på följande sätt i JavaScript:

```javascript
for (let i = 1; i <= 100; i++) {
    if (!(i % 2)) {
        console.log(i);
    }
}
```
<br>
</div>



<div class="tech-box tech-git" markdown="1"> 

# [GIT](technology/git)

Git är ett distribuerat versionshanteringssystem som skapades 2005 av Linus Torvalds. Git skapades för att hantera ändringar för Linux-kärnan.

Att Git är ett distribuerat system innebär att inget centralt arkiv behövs. Ett centralt arkiv behövs dock om flera utvecklare vill samarbeta om samma kod.

Git är tradionellt sett ett CLI verktyg, men en del GUI baserade verktyg har utvecklats för att underlätta tröskeln att börja med Git.

</div>


<div class="tech-box tech-sql" markdown="1"> 

# [SQLite](technology/sqlite)

SQLite är en filbaserad databas som använder sig av frågespråket Structured Query Language (SQL). Datatyper som man kan använda sig av är begränsade i förhållande till exempelvis MySQL eller PostGreSQL.

</div>

</div>
