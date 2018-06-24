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
   
   
