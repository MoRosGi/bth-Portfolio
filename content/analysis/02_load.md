Load
=======================

I den uppgiften ska jag analysera tre olika webbplatser med fokus på deras laddningstid.


Urval
-----------------------

Valet av webbplatser har blivit gjort genom att välja tre webbsidor som innehåller viktig information för allmänheten (särskilt i Skåne för den sista):<br>
[Polisen](https://polisen.se/)<br>
[1177](https://www.1177.se/)<br>
[Skånetrafiken](https://www.skanetrafiken.se/)


Metod
-----------------------

Metoden använder verktyget [Google Pagespeed](https://pagespeed.web.dev/) för att se vilka betyg och tips som visas för att prestandaoptimera respektive webbplats både för Desktop och Mobile. För att notera sidans laddningstid tillsammans med antalet resurser som laddas samt sidans totala storlek används 'Developer Tool' för Google Chrome.


Resultat
-----------------------


<div class="embed-container">
<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSrRgleI_dfneVE00Mk2wsJBrWhbLqhMd8RojaJQ_-hXw5vvDbB-uziQ7QfswkGL_zqyC1mKTEv60LQ/pubhtml?widget=true&amp;headers=false" title="load table"></iframe>
</div>

<p>Polisen hemsidan har en väldigt bra 'performance', det enda poäng som kunde förbättras är bilderna, som kunde ha särskilda bredd och höjd.</p>
<p>1177 hemsidan har några problem som kunde fixas: för stor 'layout' (i div element), ett bättre 'cache policy' för att minska laddningstid för varje besök, ta bort oanvänd css filer.</p>
<p>Skånetrafiken hemsidan har också en del problem som minskar 'performance' såsom: fel bild format som ökar laddningstid, bilder som saknas 'encoding', bilder som kunde förminskad, oanvänd javascript filer.</p>


Analys
-----------------------

<p>Efter att ha tittat hemsidorna 'performance' med 'Google Pagespeed' verkar problemen om bilder såsom fel format, saknas högt och bredd, fel 'encoding', det vanligaste genom alla tre sidor som jag har valt.</p>

<p>Om man jämför 'performance' av hemsidorna är det utan tvekan Polisen hemsidan som vinnar.</p>
<p>Det är viktigt att notera att polisen hemsidan har att totalt storlek av 948 kB som är ganska litet jämför 1177 och Skånetrafiken (respektive 2.3 MB och 9.2 MB). Om man räknar snabbt dataöverföringen är det 1177 med 15.593 Mbits/s som vinner matchen.</p>

<p>En snabb laddningstid kunde vara 1s medan en långsam en kunde vara 4s.</p>
<p>Med detta kan vi se att Skånetrafiken är över det långsamma gränsen, Polisen hemsidan klarar att stanna under det snabba gränsen och 1177 är knappt över det snabba gränsen.</p>
<p>Själv märker jag en skillnad mellan Polisen och 1177 hemsidorna jämför Skånetrafiken hemsidan, man kan se innehållet snabbare med de två första. Däremot kan jag inte säga att jag upplevde en lång tid innan att kunna se innehållet av Skånetrafiken hemsidan heller. Det verkar att laddningstid är mest gjort på bakgrund element.</p>


Referenser
-----------------------

<p>Analysen har använt:<br>

Google Pagespeed<br>
Developer Tool<br>
Google Sheets</p>


Övrigt
-----------------------

Den analys har blivit skrivit av Morgane Girard.