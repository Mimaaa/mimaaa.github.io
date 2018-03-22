# Browser Technologies

## Opdracht 1.1

De twee dingen die ik heb gekozen zijn:

1. Custom Fonts
2. NO-JS

De websites die ik vaak bezoek/gebruik:

1. Tweakers
2. Moodle
3. MarktetingFacts

### Het experiment op Tweakers

#### Custom Fonts

- Er is geen afwijking of probleem te vinden. Ze hebben in de css een duidelijke fallback aangegeven (systeem fonts)

#### NO-JS

- Er gebeuren geen opvallende dingen. Ik kan de website blijven gebruiken zoals het bedoeld is. Het enige dat niet werkt is dat ik info-banners niet weg kan klikken. Ik kan nog wel blijven reageren op artikelen.

#### Oplossing

Een modal maken op basis van css als fallback

### Het experiment op Moodle

#### Custom Fonts

- Er gebeurt niet zoveel bijzonders.

#### NO-JS

- Er gebeurt niet zoveel bijzonders.
- Het my-profile submenu verdwijnt en de menu-items worden naast de profiel-foto als icoontjes getoond.

#### Oplossing

- Geen oplossing vereist

### Het experiment op MarketingFacts

#### Custom Fonts

- Ze gebruiken font-icons voor de social-media icoontjes en andere menu-items. Na het uitzetten van de custom fonts zijn deze niet meer zichtbaar.

#### NO-JS

- Het hele menu wordt uitgeklapt en dat neemt de hele pagina in beslag.
- Als je een comment wil plaatsen dan zie je gelijk de rode tekst tevoorschijn komen in plaats van dat die naderhand wordt getoond.


#### Oplossing

- SVG’s gebruiken ipv font-icons
- Een css menu ter fallback of een betere indeling van de content
- Gebruik maken van de css/html check

### Overige websites

Omdat de bovenstaande sites niet echt bijzonderheden naar voren brachten heb ik andere sites bekeken:

#### Airbnb

Airbnb werkt gedeeltelijk. Je kan zoeken op steden en het aanbod zien, maar je kan de kamer niet boeken, maar je kan dan weer niet de taal en valuta wijzigen.

#### Booking

Booking website blijft wel goed werken wanneer JS is uitgeschakeld, maar je kan niet boeken.

#### Virgin America

Virgin America heeft bij de Webby Awards de beste prijs voor UX gekregen, maar als je JS uitschakelt krijg je een witte pagina te zien.

#### The Guardian

The Guardian heeft bij de Webby Awards de beste prijs gekregen voor UX en wanneer ik JS uitschakel dan blijft de pagina nog redelijk goed werken. Enkele elementen zijn niet meer te zien/gebruiken (ex. weer).

## Opdracht 1.2

### 1. Javascript uitzetten

Ik heb gekeken naar wat er gebeurd als ik Javascript op de www.cmd-amsterdam.nl website uitschakel. Conclusie: er gebeuren teveel slechte dingen.

#### Homepage

Als Javascript aanstaat dan zie je dat er een mooie grote slider aanwezig is waarin ook een mooie grote foto staat, maar zodra ik Javascript uitzet dan is de hele slider verdwenen - wat vrij logisch is aangezien de slider op Javascript werkt - maar dat de foto verdwijnt lijkt mij niet zo heel handig. De foto is bedoeld om de sfeer ook enigszins over te brengen.

Met JS:

![alt text](https://github.com/Mimaaa/MINOR_WD_BROTECH/blob/master/Week1/img/hpjs.png "Javascript ingeschakeld")

Zonder JS:

![alt text](https://github.com/Mimaaa/MINOR_WD_BROTECH/blob/master/Week1/img/hpnojs.png "Javascript uitgeschakeld")

Oplossing

Als fallback zou het ideaal zijn om te zeggen: als de slider niet wordt ingeladen laat dan een normale foto zien. Wellicht met een noscript?

Bij het inladen van de slider.js worden ook twee buttons ingeladen die belangrijk voor de interactie kunnen zijn. Deze kunnen natuurlijk ook met html/css getoond worden.

#### Studentenwerk pagina

De homepage begeeft het al redelijk snel zonder JS, maar ik was toch benieuwd wat er zou gebeuren als ik een andere pagina zou bezoeken. Toen ik de studenwerk pagina bezocht kreeg ik alleen het onderstaande te zien in plaats van een mooie interactieve pagina zoals die wordt getoond wanneer JS aanstaat.

![alt text](https://github.com/Mimaaa/MINOR_WD_BROTECH/blob/master/Week1/img/studentenwerk-nojs.png "Studentenwerk-pagina zonder JS")

#### Overige

Nog wat andere dingen die mij opvielen zijn dat je ook niet kan zoeken op de website wanneer JS het niet meer doet.

### 2. Custom Fonts

Het enige wat er gebeurt is dat de custom icon fonts niet meer werken. In dit geval het zoek-icoon - dat vrij belangrijk is, maar eveneens de social media iconen.

Op de studentenwerk pagina doen de hartjes het ook niet meer.

Oplossing:

Het probleem kan worden verholpen door gebruik te maken van SVG's in plaats van custom fonts.

### 3. Kleur

Ik heb de tool Sim Daltonism gebruikt om te kijken wat er gebeurd als mensen met kleurenblindheid de website bezoeken en of bijvoorbeeld bepaalde knoppen nog goed te gebruiken/zien zijn, maar ook om te zien wat er met de contrasten gebeurd.

Hier waren geen bijzonderheden.

### 4. Images

De CMD-Amstedam site bestaat uit ontzettend veel plaatjes en op veel plaatjes zit ook een interactie.

#### Homepage

Hier mist natuurlijk de grote slider afbeelding, maar het is eveneens zonde dat hier de twee buttons weer niet te zien zijn.

#### CMD

Hetzelfde als op de homepage: de grote afbeelding uit de slider mist, maar natuurlijk ook de plaatjes die de content versterken.

#### Studentenwerk

Deze pagina is interessant, want hier zit een interactie-element op de afbeeldingen: wanneer je over de afbeeldingen hovered dan krijg je twee opties 1) view larger en 2) more details.

Op de desktop kan je alsnog over de alt tekst hoveren waardoor die twee opties naar voren komen, maar op mobiel zie je niet dat je deze opties hebt en daardoor kan een gebruiker niet verder naar de details.

#### Blog

Deze pagina gaat helemaal stuk, want elk plaatje is een link naar de blogpost.

Met plaatjes:

![alt text](https://github.com/Mimaaa/MINOR_WD_BROTECH/blob/master/Week1/img/blog-img.png "Plaatjes")

Zonder plaatjes:

![alt text](https://github.com/Mimaaa/MINOR_WD_BROTECH/blob/master/Week1/img/blog-noimg.png "Geen plaatjes")

#### Overige

Op de overige pagina's geldt grotendeels hetzelfde als bij CMD en Studentenwerk.

Oplossing:

Het enige wat je ziet gebeuren wanneer iemand over de plaatjes op de blog pagina hovered is dat de opacity veranderd. Het lijkt mij dat je helemaal geen Javascript nodig hebt om deze pagina interactief te maken. Een prima fallback kan zijn om simpelweg CSS te gebruiken om hetzelfde voor elkaar te krijgen, maar wellicht denk ik te simpel?

### 5. Breedband internet

Wanneer ik de snelheid naar DSL verlaag en de pagina ververs dan duurt het 10 seconden voordat de eerste interactieve content verschijnt. Met behulp van de technieken die wij bij Performance Matters hebben toegepast zijn er verschillende dingen mogelijk om de bruibaarheid van de CMD website significant te verbeteren.

Enkele technieken:

- Critical CSS
- Minify & gZip HTML/CSS/JS
- Image Compressions

### 6. Geen trackpad/muis

Ik heb het in Firefox en Chrome getest, maar er zijn helemaal geen focus styles aanwezig. Het lijkt erop dat deze op display: none staan. Heel erg vervelend natuurlijk, want op deze manier kunnen mensen die bijv. 1 arm niet kunnen gebruiken niet met de website interacteren.

Oplossing:

Duidelijke focus styles inplementeren.

### 7. Cookies

Als ik de cookies uitzet dan werkt de website nog prima. Ik heb even gekeken welke cookies aanwezig zijn en dat blijken alleen de Google Analytics cookies te zijn, dus niet iets waardoor bepaalde functionaliteiten het niet meer gaan doen.

### 8. localStorage

LocalStorage wordt toegepast voor een bepaalde Wordpress admin functionaliteit. Het is dus niet iets dat CMD-Amsterdam zelf heeft geimplementeerd. De website gaat daardoor dus ook niet stuk.
