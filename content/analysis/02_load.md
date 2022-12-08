---
Title: load
Description: Report about load
Template: reports
# hidden: true
---

Analys av laddningstid för tre av Sveriges största matbutikers hemsidor
=======================

Analys av Sveriges tre största livsmedelkoncerners laddningstid och om de kan optimeras av deras hemsidor.

Urval
-----------------------

Urvalet är begränsat inom detaljvaruhandel för livsmedel. Endast dem tre största livsmedelbutikerna, ICA, Coop och Hemköp, baserat på SVTs undersökning från år 2019. Se länk nedan:

https://www.svt.se/nyheter/inrikes/trots-butikskopet-ica-etta-pa-matmarknaden

Metod
-----------------------

Besök sida av intresse, använd verktyget https://pagespeed.web.dev/?utm_source=psi&utm_medium=redirect och analysera prestandan för mätpunkterna:

Prestanda,

Tillgänglighet,

Bästa Lämpliga Praktiken (BLP),

Sökoptimering

Resultat
-----------------------

<div class="palette-container">
<div class="table-details-container">
<h2>Data</h2>
<table class="table-color-details">
    <thead>
        <tr>
            <th>Hemsida</th>
            <th>Prestanda</th>
            <th>Tillgänglighet</th>
            <th>BLP</th>
            <th>Sökoptimering</th>
            <th>Total</th>
        </tr>
    </thead>
        </tr>
        <td>ICA Desktop</td>
        <td>75.33</td>
        <td>83.00</td>
        <td>100.00</td>
        <td>100.00</td>
        <td>358.33</td>
    </tr>
        </tr>
        <tr>
        <td>Coop Desktop</td>
        <td>59.67</td>
        <td>83.00</td>
        <td>100.00</td>
        <td>83.00</td>
        <td>325.67</td>
    </tr>
    <tr>
        <td>ICA Mobil</td>
        <td>26.33</td>
        <td>81.00</td>
        <td>100.00</td>
        <td>100.00</td>
        <td>307.33</td>
    </tr>
    <tr>
        <td>Coop Mobil</td>
        <td>38.00</td>
        <td>83.00</td>
        <td>100.00</td>
        <td>86.00</td>
        <td>307.00</td>
    </tr>
        <tr>
        <td>Hemköp Desktop</td>
        <td>31.00</td>
        <td>77.00</td>
        <td>92.00</td>
        <td>100.00</td>
        <td>300.00</td>
    </tr>
    <tr>
        <td>Hemköp Mobil</td>
        <td>12.00</td>
        <td>73.00</td>
        <td>88.67</td>
        <td>98.00</td>
        <td>271.67</td>
    </tr>
</table>
</div>
<div class="google-table">
<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vS6nAnnB0Vw4gSKUgj1-fVndQAtuGRbQHUR06gajzdyItLyAM6G-QhAzm1g2LyAmzkU1YXx1ExKqiUo/pubhtml?widget=true&amp;headers=false"></iframe>
</div>
</div>

Analys
-----------------------

ICA desktop totala poäng rankas 1 med totala poäng 358.33. Överlag en bra och snabb sida men prestandan visade på 75 poäng. Den största anledning är Total blocking time som drar ner prestandan med 30% d.v.s. tiden sidan är blockad från interaktion med användaren som musklick och dylikt. En åtgärd är att reducera DOM trädet för att minska minnelagring och style kalkylering. Hemsidan visar på effektiv sökoptimering av moterer som exempelvis google och god datasäkerhet mot XSS attacker. 

Coop mobil rankas på 4 plats med totala poäng 307.00. Prestandan var mycket dålig med endast 35 poäng och det finns många möjligheter för optimering bl.a. att endast ladda bilder som användaren tittar på och på så sätt minska tiden innan användaren kan interagera med hemsidan. En annan möjlighet är att minska på användning av Javascript som inte används eller att optimisera bilder. 

Hemköp mobil och desktop hamnar i botten och där den förstnänmda endast hade 271.67 poäng. Prestandan här vara bara 11 poäng. Den första optimiseringen som kan göras är att sätta en bestämd width och height på bilderna för att minska att bilderna skiftar. Likt coop så kan man använda sig av lazy-loading offscreen eller optimiera bilderna.

Generellt så visar alla hemsidor på både laptop och mobil på god sökoptimering men alla sidor hade dålig prestanda men i många fall kan detta förbättras genom bättre bildoptimering. I en enkel google sökning hamnar ICA högst upp bland de olika livsmedelsbutikerna, sedan COOP och sist Hemköp vilket stämmer väl överens med sökoptimeringen.

Alla sidor hade relativt långsam laddningstid men ICA var snabbast men hade också minst storlek. Hemköp laddade snabbare än Coop vilket var förvånande då både Coop och Hemköp hade ungefär samma storlek men Coop hade bättre prestanda. En sannolik anledning kan vara att Hemköp hade lägre resurser jämfört med Coop.

Vinnaren är ICA som hade bäst resultat och laddade snabbast. Tvåa kommer Hemköp som laddades snabbare än Coop. Sist kommer Coop som hade bättre prestanda än Hemköp men laddade långsamt. 

För att klassas som snabb bör en hemsida ladda klart inom 500ms. Då hinner läsaren inte uppfatta skiftande layouts eller annat (om man inte aktivt tittar efter detta). Samtliga laddades långsammare än 500ms vilket uppfattas som långsamt.


Referenser
-----------------------

Ange de eventuella referenser du använder dig av, om några.

Prestandamätare
https://pagespeed.web.dev/report?url=https%3A%2F%2Fica.se%2F&form_factor=desktop

CLS
https://web.dev/cls/

TBT
https://web.dev/tbt/

ICAs hemsida
https://www.ica.se/

Hemköps hemsida
https://www.hemkop.se/

Coops hemsida
https://www.coop.se/


-----------------------

Författare:

Ludvig Ogenblad