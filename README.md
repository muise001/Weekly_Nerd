# De Weekly Nerd

Welkom op de weekly nerd pagina van mijn github. Afgelopen half jaar hebben we wekelijks gastcolleges gehad van bedrijven, de opleiding en vrienden van de opleiding. Hieronder heb ik vijf "Weekly Nerds" samengevat. Veel leesplezier.

## Inhoudsopgave
  - Git en Github
  - Weekly Nerd @ Tam / Tam
  - Accesability @ Schiphol Group
  - Smashing Magazine @ Icons Meeting
  - Bruce Lawson - Web Standards 
  
  
# Git en Github
  ### Inleiding
  De weekly nerd over git, github en het verschil ertussen werd gegeven op 14 februari door Titus Wormer op de HvA. Ik had zelf al eerder met github gewerkt, maar ik wist er weinig vanaf. Dit college gaf me meer inzicht over samenwerken via github, open source en licenties.
  
  ## Wat zijn Git en Github
  Github. een sociaal netwerk voor nerds. Github wordt namelijk gebruikt door miljoenen gebruikers. Voor een leek die nog nooit gewerkt heeft met Github of misschien niet eens weet wat het is: Github is een online werkomgeving waar je makkelijk code kan uploaden, bewerken en updaten. Het mooie van Github is ook dat je samen met anderen aan je projecten kan werken. Je kan de code van je team makkelijk updaten, samenvoegen en bewerken. Hoe dan? Hier volgt een stappenplan:
  1. Je maakt een github pagina aan voor jou project en nodigt anderen uit om mee te werken
  2. Je upload de basis van het project (bijv. lege HTML-, CSS- en JS-bestanden). Deze Push je in de master.
        - Pushen is het uploaden van code naar een branch. Een "branch" kan je zien als een kopie van het hoofdbestand waar je op verder werkt.
  3. Zowel jij als je teamgenoot maken feature-branches aan van de master en geven het project vorm.
        - Stel jij hebt gewerkt aan een klok en je teamgenoot aan een kalender, dan noem je de branches bijvoorbeeld `feature/klok` en `feature/kalender`
  4. Tussentijds maken jij en je teamgenoot `commits` van bepaalde voortgang. Bijvoorbeeld van de stijl van de klok. Door namelijk je werk te committen, wordt het al upgeload naar Github. Hierdoor raak je niet je code kwijt, mocht je computer tussentijds crashen.
  5. Als je eenmaal klaar bent met de klok, dan maak je je laatste commit. Deze push je naar Github. In github maak je een pull-request. Dat kan je zien als een aanvraag om je werk samen te voegen. Github kijkt dan of het mogelijk is om je werk samen te voegen (te mergen), of geeft aan dat er "merge-conflicten" zijn. Deze zijn (vaak) gemakkelijk op te lossen.
  6. Als je werk is gemerged ben je klaar met de feature-branche "klok". Nu kan je een nieuwe feature-branche opstarten en dan begin je weer bij stap 3.
  
Het stappenplan hierboven geeft in grote lijnen aan hoe Github werkt. Git is een commandline taal die gelinkt is aan Github. Github is de website en Git staat op je computer. Door bepaalde command-lines kan jij terwijl je aan het werk bent via Git je werk uploaden naar github.

  ##### M'n werk zit erop. Wat nu?
  Stel je denkt klaar te zijn met een project (projecten zijn namelijk nooit af), dan kunnen gebruikers issues naar je sturen. Dit kan je zien als bugs of fouten in de applicatie die je aan het maken bent. Deze Issues kan je openen om de aanvraag te accepteren en weer sluiten als je de bug gefixt heb.
  
  ##### Ik krijg zoveel issues. Wat nu?
  Stel je applicatie wordt gebruikt door het grote publiek, dan kan je ervoor kiezen om het "Open source" te maken. Dit houd in dat andere mensen mee kunnen werken aan jou product. Deze mensen kunnen bijvoorbeeld ook Pull-requests aanmaken en Issues afhandelen. 
  
  ##### Mijn buurman heeft een idee om mijn applicatie te gebruiken voor een alternatief idee.
  Leuk! Je kan je buurman toestemming geven om jou applicatie te "Forken" en dan kan hij er zelf aan verder werken in een soort kopie. Het werk dat hij doet belemmert niet jou code of voortgang en hij kan zelf toevoegen wat hij wilt. Bij hem wordt namelijk een nieuwe repository aangemaakt, maar wel met de code die jij al geschreven hebt.
  
  ##### Is dat wel legaal, misschien gaat hij er wel met de buit vandoor.
  Het is legaal, mits hij jou bepaalde credits geeft. Dit werkt via bepaalde Licenties. Een licentie kan je zien als een lijst met regels die jij degene die jou "forkt" geeft, waarin staat wat hij wel en niet mag doen. Bekende licenties zijn:
   - MIT
   - GPL
   - ISC
   - LGPL
   
![Sketchnotes Github](https://github.com/muise001/Weekly_Nerd/blob/master/Sketchnotes/github.JPG)
   
> Bron : [aantal gebruikers Github](https://www.quora.com/How-many-users-does-GitHub-have) 
   
# Weekly Geek @ Tam/Tam

### Inleiding
Tam/Tam is een vrij groot internetbedrijf met meerdere kantoren. Een van hun vestigingen zit in Amsterdam en de andere vestiging zit in Rotterdam. Tam/Tam vertelde over hun werkwijze, code-setup en over DEPT. DEPT, een online agency is in het leven geroepen door Tam/Tam. DEPT moet je zien als een samenwerking tussen meerdere grote bedrijven door de hele EU. Op het moment zijn er 13 bedrijven aangesloten bij DEPT. Deze zijn vooral te vinden in het Verenigde Koninkrijk, Nederland en Duitsland. Het doel van DEPT is om ALLES te kunnen leveren op internet-gebied. Denk aan VR, AR, IOT, Online Marketing en natuurlijk "gewoon speciale" websites. DEPT heeft al vele grote klanten gehad. Denk aan de Rabobank, ebay, Walibi, Tui, Tom Tom, KLM, Microsoft, Adidas, Zalando, KPN, G-Star en vele anderen. Tam/Tam zelf houdt zich vooral bezig met Front-end.

## Werkwijze Tam/Tam
Tam/Tam heeft al veel ervaring in het werkveld. Hierdoor hebben ze een soort formule bedacht waarmee ze aan elke website beginnen. Een van hun setups ziet er als volgt uit:
  - HTML      - Samen met nunjucks
  - JS        - ES6 Modulair opgesteld
  - SCSS      - ITCSS
  - Webpacks  - gulp en webpack

HTML en ITCSS werken samen. ITCSS staat voor : "Inverted Triangle CSS" en moet een soort template CSS worden voor de HTML. Je gebruikt hierbij grote duidelijke class-names die een element altijd hetzelfde stijlen. Zo kan je bijvoorbeeld een setup hebben zoals :
  ```
  .bigButton{
    width: 50%;
    Font-size 2rem;
    padding: 1rem 0;
    border: 3px solid black;
  }  
  
  .bgColorRed{
    background-color: red;
  }
  
   .bgColorBlue{
    background-color: red;
  }
  
  .fixedLeft {
    position: fixed;
    left: 0
  }
``` 
Je kan dan een button bepaalde classes hiervan meegeven waardoor hij er altijd goed uit blijft zien. Er zouden ook andere classes in kunnen zoals `.smallButton` `.fixedRight` etc. Zolang de classnames maar duidelijk genoeg zijn.

![ITCSS](https://github.com/muise001/Weekly_Nerd/blob/master/Sketchnotes/itcss.png)

## Een (part-time) weekje Tam/Tam - Walibi project

|MA|DI|WO|DO|
|:-:|:-:|:-:|:-:|
|MAMO (Maandagochtend Meeting)|Kickoff|Beginnen Basics|Klant komt langs|
|Dev Meeting|Start Front-end setup|fe-shelf|testers|
|Inschattingen doen|Trello board opzetten|Accesibility check|domibo|
|||stand-up||

![Sketchnotes Tam/Tam](https://github.com/muise001/Weekly_Nerd/blob/master/Sketchnotes/tamtam.JPG)

> ITCSS extra informatie : [xfive.co](https://www.xfive.co/blog/itcss-scalable-maintainable-css-architecture/)

# Ischa Gast en Tom @ Schiphol Group
### Inleiding
Voor deze Weekly Nerd zijn we afgereisd naar de Schiphol Group. Dit is een gebouw vol met kantoren waar onder andere ook gewerkt wordt aan de website van schiphol. De sprekers waren Isha Gast en Tom. Isha Gast is een front-end developer die zich vooral bezig houdt met accesability. Tom is een blinde man die lessen geeft aan mensen die (pas kort) blind zijn. Deze lessen gaan over hoe je je computer en telefoon kan gebruiken zonder dat je kan zien. 

## Isha Gast
> 100% van de mensen heeft een beperking.

Met dit statement begon Isha Gast zijn college. Isha houdt zich dagelijks bezig met accesibilty. Bijna elke dag "valt hij bedrijven" aan via Twitter met tests die hij gerunt heeft op hun website om hiermee te laten zien dat het "accesibility-wise" beter kan. Als het aan Isha Gast ligt moet het web voor iedereen toegankelijk zijn. Met iedereen bedoelt hij ook echt iedereen. Of je nou blind, kleurenblind, spastisch, oud, slecht-ziend, doof of kaal bent, je moet moeiteloos het web kunnen verkennen. Hij gaf ons de volgende tips over kleuren die we "nooit" moeten gebruiken:
  - Lichtblauw
  - Lichtgroen
  - Oranje
  - Wit op Oranje
Hij vertelde ook dat wat wij zien totaal niet representatief is voor bijvoorbeeld kleurenblinden. Kijk bijvoorbeeld naar de ING website. De hele site is oranje en "call-to-action buttons" zijn vaak oranje met een witte tekst. Voor niet-kleurenblinden mensen een prima contrast, maar voor wel-kleurenblinden mensen onsleesbaar. 

### Tips en Tools
In het kader van "Het web een betere plek maken voor iedereen", gaf Isha Gast ons een tips en tools die accesibility-wise noodzakelijk zijn.
- Tips
  - Focus state 
    - Een custom focus-state is heel belangrijk voor slecht-zienden en kleurenblinden mensen. Dat komt omdat bijvoorbeeld de lichtblauwe kleur van de default focus-state van google chrome voor hen slecht te zien is
  - Headers
    - Headers zijn ook belangrijk. Niet alleen voor de semantiek van de code of pagina, maar ook voor blinden. Screenreaders lezen namelijk de Headers voor en bieden headers aan als navigatie
  - Kleur contrast optimaliseren voor kleurenblinden en slecht-zienden
  - Skip to content button
    - Een skip to content button is belangrijk voor blinden en mensen die moeite hebben om een muis te gebruiken. Deze mensen gebruiken namelijk van de "tab" knop. Door een "skip to content knop" toe te voegen, hoeven mensen bijvoorbeeld niet 300x te tabben voordat ze bij hetgene zijn waar ze voor komen op de website.
    
- Tools
  - Colour Contrast Analyser
    - Dit is een tool die de contrasten van een website meet. Hij heeft aan of een kleur goed te zien is voor kleurenblinden, maar ook of bepaalde contrasten goed werken. 
  - Funkify
    - Funkify is een hele goede tool waarbij je allemaal scenario's kan naspelen op een website. Zo kan je bijvoorbeeld Dyslectie "aanzetten" waardoor letters in een woord steeds van positie veranderen, "Elderly-Mode" om de hele website een beetje blurry te maken, "Zonlicht-Mode" om het contrast te creeëren alsof er een hele velle zon op je scherm schijnt en vele anderen. Door deze tools te gebruiken kan je rekening houden met de scenario's die deze toel biedt. Bij "zonlicht-mode" kan je er bijvoorbeeld voor zorgen dat je headers groter of dikker worden, zodat ze altijd goed te zien zijn, Bij "Elderly-mode" kan je bijvoorbeeld zien of je lettertype groot genoeg is etc.
    
## Tom
Tom is een blinde man vanaf zijn geboorte. Hij vertelde dat hij altijd veel met computers had gewerkt. Hij was erg fan van MS-Dos. Dit is een command-line taal waarbij je alleen tekst hoefde in te voeren en tekst terug kreeg. Het was voor hem een kwestie van commands uit je hoofd leren en klaar. Tegenwoordig zijn computers niet meer "Tekst-based", maar "Visual-based". Dit was voor Tom een moeilijke switch. Gelukkig kwam er al snel screenreader-compattibility. Hierdoor kon hij alsnog werken op een computer omdat alles voor hem werd voorgelezen. Voor hem en eigenlijk alle andere blinden is het cruciaal dat je sneltoetsen kan gebruiken. Hij gaf het voorbeeld van Microsoft Word. Hij vond dit een fijn programma om te gebruiken. Dit komt hij alles kan benaderen met sneltoetsen. Hij zou het ook fijn vinden als er sneltoetsen of "skip-to-content" knoppen kwamen op websites.

Nadat Tom klassikaal de website Dumpert bezocht, gaf hij nog een aantal tips:
  - Headers altijd boven het plaatje
    - Hierdoor weet je waar het plaatje over gaat en kan er geen verwarring komen over welke titel hoort bij welk plaatje
  - Headers zijn heel belangijk
    - Screenreaders kunnen navigeren door headers. Het is dus belangrijk dat titels H1 zijn en subtitels H2. Als je alles H1 maakt, weet Tom niet meer wat nou wel belangrijk is en wat niet. 
  - Labels bij inputs in forms
    - Labels zijn belangrijk omdat Tom dan tehoren krijgt wat er gevraagd wordt bij een input-veld
  - Voice Over op de iPhone werkt ontzettend goed
  - Autoplay voor filmpjes is een slecht idee
    - Aangezien filmpjes audiovisueel zijn en de screenreader voorleest, is het moeilijk om de pauzeknop te vinden, omdat een filmpje door je screenreader heen praat.
    
![Scetchnotes SchipholGroup](https://github.com/muise001/Weekly_Nerd/blob/master/Sketchnotes/schiphol.JPG)

# Smashing Magazine @ ICONS Meeting
### Inleding
De desginer van de [Smashing Magazine](https://www.smashingmagazine.com/) website kwam op de HvA vertllen over patterns op het web, de website van Smashing en hoe je een website "Pleasureable" kan maken. 

## Make boring interesting
Wat de deginer van Smashing vertelde is dat niet elke website _plat_ of _saai_ hoeft te zijn. De website van Smashing zit vol met "leuke" features. Zo is er op elke pagina wel een kat te vinden, zijn er legio animaties, zijn de forms klantvriendelijk, zijn er custom focus states en is er een coupon voor iedereen. De laatste vond ik het leukst. Hij vertelde dat veel mensen (waaronder ik) altijd bij het bestellen van producten op internet eerst Google afspeur om ook maar de kleinste korting te krijgen. Vaak resulteerd dit in een uur Googlen en geen of een verlopen coupon. Daar hebben ze bij Smashing iets op gevonden. Stel je voert een ongeldige over verlopen coupon in, dan komt er onder het coupon vlakje een section te staan waarin staat "This coupon looks __Fishy__, Why don't you try the coupon-code __Fishy__ instead. Vervolgens voer je "Fishy" in als coupon-code en je krijgt 1% korting. 

Het gaat ook niet per se om de korting. Het gaat om het gevoel dat je gewonnen van het systeem, door korting te krijgen terwijl je het eigenlijk niet verdient. 

#### Fun patterns
Ook vertelde hij over leuke patterns mensen hebben ontwikkeld om het web leuker te maken. Hieronder volgt een lijstje van voorbeelden die hij gaf.
  - Creative Popup
    - Niets op een website is zo irritant als een Popup. Daar hebben ze op de website van het [Volkshotel](https://www.volkshotel.nl/nl/) iets op gevonden. De popup is namelijk een hand die een bordje vasthoudt en je muis volgt. Dit ziet er grappig uit en het voelt niet als een popup.
  - Funny Login  
    - De "fun login" was een normaal login-venster waar je je e-mail adres en wachtwoord in moest voeren. Alleen stond er een SVG boven. Dat was een ijsbeer. Als je je e-mail invoerde volgde de ogen van de ijsbeer waar je aan het typen was. Daar alleen al word ik vrolijk van. Maar daarna... Als je je wachtwoord invoerde, deed de ijsbeer zijn handen voor zijn ogen. Als je vervolgens op "show password" klikte, deed hij een van zijn handen een beetje open en keek hij door z'n vingers mee.
  - You MUST be 18 to visit this page
    - Een website waar je cigaren kon kopen, moest volgens de wet de geboortedatum vragen aan haar bezoekers om ze door te laten. Deze website had dat gedaan. Alleen waren de invoervelden alvast ingevult. De 34ste dag van de 13de maand uit het jaar 1854. Dit deden ze omdat het hun toch niet uitmaakt wie er op hun site komt, maar het MOEST van de wet.
    
#### Storytelling
Wat belangrijk is aan een website is dat je een verhaal vertelt. Dit kan zelfs op een hele subtiele manier. 
  - Een chinese website over bomen, gebruikt in plaats van pijljes op de site het icoon van een boompje om dingen aan te wijzen.
  - Weber wilt op hun website laten zien wat hun Barbeques allemaal kunnen. Dit kan uiteraard met foto's, maar in het kader van storytelling doen ze dit op een andere manier. Ze hebben een interactive 3D animatie gemaakt van hun Barbeques, zodat het voelt alsof je de barbeque bedient en niet de website. 
  
> Als je goed nadenkt over een website en echt een verhaal over wilt brengen, dan is het ook veel leuker om deze te gebruiken  
![Sketchnotes Smashing](https://github.com/muise001/Weekly_Nerd/blob/master/Sketchnotes/smashing.JPG)

# Bruce Lawson - W3C over webstandards
### Inleiding
Het W3C is een groep mensen die verantwoordelijk zijn voor de taal HTML. Zij bedenken en leggen webstandaarden vast. Bruce Lawson zit bij deze groep. Op de HvA vertelde hij over het begin van standaarden, webstandaarden, kleuren en pornosterren en knakworsten. 

## The beginning of the web......... Standards
##### De Piano
Vroeger voordat het web er was, had je piano's. Huh? Ja, piano's. Niet zomaar piano's, maar piano's die zelf speelden. Net als een draaiorgel, speelde die muziek af via gaten in papier. Fascinerend. Wat was nou het probleem? Niet elke piano-roll werkte op elke piano. Dat kwam omdat het ene bedrijf smaller papier gebruikte dan andere bedrijven. Daarom moest je dus voor het ene liedje die piano hebben en voor een ander liedje die andere. Daar moest verandering in komen, vonden vele gebruikers.

Die verandering kwam er. De bedrijven die die piano-rolls maakte, regelde een vergadering. Hierin bespraken ze hoe breed, dik en hoe groot de gaten moesten zijn in de piano-rolls om het op elke piano te kunnen afspelen.

##### De Trein
Jaren later, toen niemand meer zo'n piano had. Had je hetzelfde probleem met treinrails. Elk land in West-Europa had treinen en treinrails, maar niet elke trein paste op elk spoor. In Engeland hadden ze bijvoorbeeld het spoor de breedte gegeven van twee paarden. In andere delen van Europa hadden ze andere maatstaven gebruikt. Hierdoor kwam het wel eens voor dat treinen bij de grens volledig overgetilt moesten worden om verder te kunnen rijden. Uitendelijk hebben ze opgelost door standaarden te stellen.

Hetzelfde gold voor het web. In het begin van het web was het een zooitje. Hier moest verandering inkomen. Daardoor is het W3C gesticht. 

## Not quite standard yet...
Patenten. We mogen het er eigenlijk niet over hebben, maar door het gebruik van patenten kunnen veel websites bepaalde functionaliteiten niet gebruiken. Amazon had een belangrijk patent. ["The single click checkout"](https://en.wikipedia.org/wiki/1-Click). Dit patent was in het leven geroepen om het betalen en invullen van gegevens makkelijker temaken. Als je was ingelogd en je wilde iets kopen, hoefde je maar op één knop te drukken en de volgende dag lag het in je brievenbus. Geweldig. 

Dit pattern die bedacht is door Amazon, was een pattern die meerdere webshops wilde gebruiken. Helaas laat de wet dat niet toe. Dit zorgt voor een automatiserings-achterstand bij andere webwinkels. 

> The biggest enemy of the web-standards is patents - Bruce Lawson

##### Opera
Bruce is een tijd werkzaam geweest bij de internetbrowser "Opera". Hier hadden ze de regel dat je het nooit en te nimmer mocht hebben over patenten. Deze regel was in het leven geroepen door (wederom) de wet. In de wet staat namelijk dat als je een patent toch gebruikt zonder dat je daar toestemming voor hebt, een boete moet betalen. Is het zo dat je wist dat het patent bestond, maar het evengoed gebruikte zonder toestemming, dan moest je 3x de waarde van die boete betalen. Hierdoor mocht je niet e-mailen over patenten, praten over patenten en eigenlijk niet eens denken aan patenten.

![Sketchnotes Bruce Lawson](https://github.com/muise001/Weekly_Nerd/blob/master/Sketchnotes/w3c.JPG)

# Einde
Bedankt dat je de tijd hebt genomen om dit verslag door te lezen. Hopelijk heb je net zo van het lezen genoten als ik van het bijwonen van deze lezingen en het schrijven van dit verslag. Helaas heb ik niet de Weekly Nerd van de Hacketon erin. Dit komt om dat ik helaas niet aanwezig kon zijn op de Hacketon ivm herkansingen. Des al niet te min hoop ik dat ik het op deze manier goed heb opgelost. En nogmaals bedankt voor het lezen.

> Emiel Muis
