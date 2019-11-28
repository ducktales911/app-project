# App project proposal
A timed todo list with gamification elements for iOS

Timeboxing is het vooraf beperken van de hoeveelheid tijd die men aan een bepaalde activiteit wil en mag besteden. Dit om te voorkomen dat iets uitloopt. In deze app kan je een takenlijst maken en aan elke taak een tijd toekennen. Het voordeel is dat je dan kunt berekenen hoe lang het gaat duren om alle taken af te ronden, en je dus niet meer plant dan wat in een dag gedaan kan worden. Daarnaast weet je hoe laat je ongeveer klaar gaat zijn met de belangrijke taken van de dag, waardoor je dus weet of je tijd hebt voor andere plannen.

## Visual sketch

![Sketch](https://raw.githubusercontent.com/ducktales911/app-project/master/doc/visual%20sketch.jpg)

## Main features

### MVP
- Taken worden toegevoegd en een tijd toegekend
- Vervolgens kan de gebruiker voor elke taak de timer laten lopen
- Bovenin het scherm staat:
  - Hoe laat je klaar bent met alle taken
  - De totale tijd van alle taken
- Melding wanneer de tijd voor de taak op is met de tekst "Time for [taak+1]" met Quick Actions:
  - Snooze = huidige taak verlengen
  - Beginnen met [taak+1]

### Optioneel te implementeren
- Een “nag” functie voor meldingen: blijf meldingen sturen totdat de gebruiker gehoor geeft (zoals de app “Due”).
Gamification element: je krijgt punten door het voltooien van taken. En minpunten als je taken uitlopen en als je te lange pauzes neemt.
- Sociaal element: je kunt vrienden toevoegen en hun punten zien.
- High scores
- Punten gaan verloren als je de app afsluit (tegen smartphone-verslaving, zoals de app “Forest”)
- Apple Watch app
- Een notepad functie waarop je kunt noteren wat je te binnen schiet.
- Taken toevoegen met gestures zoals in de app “Clear”.
- Synchronisatie tussen apparaten
- Universele app
- Dark Mode
- Pomodoro functie
  - Elke 25 minuten geeft de app een melding
  - Na elk werkblok gaat een pauze van 5 minuten in
- Punten worden verdient door:
  - Taken te voltooien (langere taken leveren meer punten op)
- Punten gaan verloren door:
  - Taken door te schuiven (aan het eind van de dag geven alle onvoltooide taken minpunten)
  - Taken uit te laten lopen: de wekker telt door nadat de tijd op is.
- Mogelijkheid om templates van takenlijsten aan te maken

## Prerequisites

- De data wordt ingevoerd door de gebruiker. Er zijn geen externe data bronnen nodig.

- Voor de cloud sync is kan gebruikt worden gemaakt van een iCloud storage API.

- Voor de eventuele high score functie moet gebruik worden gemaakt van een externe database zoals AWS of Oracle Cloud.

##### Vergelijkbare apps
- De app "Due" gebruikt herhalende meldingen om ervoor te zorgen dat de gebruiker de herinnering niet vergeet. Dit wil ik ook toepassen in deze app. Dit zorgt ervoor dat je niet de melding negeert (omdat je ergens mee bezig bent) en het vervolgens vergeet. Met een "actionable notifiction" kan je dan de keuze maken of je de taak als voltooid wilt markeren, of nog even door wilt gaan.
- De app "Forest" geeft je punten wanneer je de app geopend houdt. Dit wil ik als optie toevoegen onder de instellingen.
- De interface van de app "Clear" heeft een intuitieve manier om taken toe te voegen en te verwijderen met "gestures". Deze wil ik globaal overnemen zodat er minder knoppen nodig zijn die de interface rommelig maken.

##### Mogelijke problemen
 - De hoeveelheid mogelijke functies maakt het lastig om een UI te ontwerpen die makkelijk te leren is en fijn in gebruik.
  - Een manier om dit tegen te gaan is door de meer specifieke functies te "verstoppen" of standaard uit te schakelen en als optie toe te voegen in de instellingen
