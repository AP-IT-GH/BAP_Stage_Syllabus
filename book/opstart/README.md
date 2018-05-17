{% import "../vars.md" as vars %}
# Opstart
De opstart van de BAP / Stage gebeurt in 5 stappen
1. Infosessie
2. Toewijzing van stageplaats
3. Introductie met stageplaats
4. Administratieve taken
5. start stage op stageplaats

## Infosessie
Tijdens de infosessie wordt de algemene werking van de BAP / Stage toegelicht,
de info van deze sessie komt uit deze stage syllabus

## Toewijzing van stageplaats
De toewijzing van de stageplaats gebeurt volgens ranking, deze is gebaseerd op
het gewogen puntentotaal van de student. Hierdoor krijgt de beste student zijn
eerste keus. We gaan de lijst verder af, moest een student zijn eerste keus
niet meer beschikbaar zijn dan wordt de tweede genomen en zo verder.

## Introductie met de stageplaats
Als de stages verdeeld zijn, wordt er door de stagecoördinator een
introductiemail verstuurd. Hierna is het aan de student om een afspraak te
maken met het bedrijf en de nodige documenten in orde te brengen.

## Administratieve taken
Nadat de introductie gemaakt is, is het aan de student om de nodige
administratie in orde te brengen. De nodige documenten zijn:

* het *Stagecontract/stageovereenkomst* opstellen en het stagereglement
  ondertekenen,
* Risicoanalyse en werkpostfiche van het bedrijf (zie voorwaarden onderaan)
* Kopie van het Stage Syllabus bezorgen aan het stagebedrijf.
* Github repo forken en voorbereiden.


### Stagecontract en stagereglement
Deze documenten staan in [Documenten]({{ vars.docsUrl }}).

Volgende stappen dien je te ondernemen:
1. Gelieve beide documenten samen met je promotor (school en bedrijf) vooraf in
   te vullen.
2. Druk de documenten in *drievoud* af.
3. Onderteken de documenten.
4. Geef *alle 3* de exemplaren aan je stagegever
5. Deze dient de 3 versies te ondertekenen (mogelijk moet dit via juridische of
   HR-dienst van bedrijf te gebeuren en nadien aan jou terug bezorgen)
6. Je levert de *3* ondertekende versies (met handtekeningen van jezelf en het
   bedrijf) aan de stagecoördinator. Deze zal zorgen voor de handtekening van
   de AP Algemeen directeur
7. Nadien krijg je 2 exemplaren. Een is voor je stagegever, de ander is voor
   jezelf.
8. Stagecontract toevoegen als PDF aan je BAP/Stage repo.

*Lees het stagecontract en stagereglement grondig na opdat je duidelijk weet
wat je rechten en plichten zijn.*


#### Wat waar invullen
* Wie moet wat waar invullen:
  * Pagina 1: veld 2 "stagegever" wordt ingevuld door het bedrijf 
  * Pagina 2: veld 3 "student-stagiar" vul je zelf in.
  * Pagina 3: art 1 : dit spreek je samen met bedrijf af. Meestal zal je
    functie "jr ontwikkelaar" of iets dergelijks zijn. 
  * Pagina 2: art 2:  De eerste zin moet zijn: "De stage bedraagt {{ vars.aantalStageDagen }}  dagen in de
    periode van {{ vars.startStage }} tot {{ vars.eindeStage }}"
  * Pagina 2: art 3: De eerste persoon is je (voorlopige) AP-promotor, met
    functie "lector". De 2e persoon is de (voorlopige) persoon die je dagelijks
    gaat opvolgen bij het bedrijf. Dit moet dus iemand van IT zijn, niet van
    HR.  Op de laatste lijn zet je best "e-mail, bij dringende zaken gsm".
  * Pagina 3: art 6: Meestal zal hier 0 euro staan. Uiteraard is het bedrijf
    vrij hier een bedrag te zetten indien nodig. 
  * Pagina 3: art 7: dit moet de HR-dienst van het bedrijf invullen . In onze
    sector is de kans klein dat een passend gezondheidstoezicht moet gebeuren.
  * Pagina 6: alle partijen tekenen de 3 exemplaren op hun lijntje + naam en
    voorafgegaan door "gelezen en goedgekeurd"

### Risicoanalyse
* Ieder bedrijf met uitzondering van zelfstandigen zonder werknemers moet deze documenten reeds bezitten voor de werknemers van het bedrijf. In dat geval dient de stagegever je een kopie van deze documenten te bezorgen.
* Indien je terecht komt bij een zelfstandige zonder werknemers mag je gebruik maken van het document risiconalyse dat je via dhr Smets kan verkrijgen.*Merk op dat in quasi alle andere gevallen dit document door het bedrijf zelf beschikbaar dient te worden gesteld.*
* Het is belangrijk dat je de juiste versie afgeeft. Indien het bedrijf werknemers heeft, is het zinloos het ter beschikking gestelde document te gebruiken aangezien dit document in dat geval toch niet geldig is.


### Stagesyllabus
Zorg ervoor dat je stagegever en stagementor een versie van de stagesyllabus
krijgen (dit document) zodat ook zij op de hoogte zijn van alle afspraken en
regels.  Het is jouw verantwoordelijkheid dat je de afspraken erin nakomt (**je
stagebedrijf mag, maar hoeft geen rekening te houden met de syllabus: je hebt
m.a.w. 2 verschillende planningen die je zelfstandig zal moeten leren
beheren**).

### Github Repository
Al je documenten en documentatie dien je in te schrijven voor de GitHub Classroom. Je dient daarvoor de structuur te gebruiken van de *BAP StudentRepo*.
Uiteraard mag je waar nodig in de mappen extra zaken toevoegen (ordelijk houden
aub). De inhoud van deze repo is eigendom van de AP Hogeschool. Bespreek wel
met het bedrijf, welke informatie je juist mag delen, zodat er geen IP wordt
"gemixt".

Je kan je [hier]({{ vars.ghClassUrl }}) inschrijven in de classroom.

#### Hoe ga je te werk
* Ga naar Digitap en open daar in de cursus Bachelorproef en stage de "cursusdocumenten" map.
* Volg de "invite"-link getiteld "Je private repo"
* Maak via de invite een nieuwe repo aan. **Let op de naamgeving:** deze moet AchternaamVoornaam_BAP1718 zijn. Heet je dus Jos Stoffels dan zal je repo als naam StoffelsJos_BAP1718 hebben.

Vervolgens, *mogelijkheid A*
* Download vervolgens de mappenstructuur van de voorbeeldrepo [hier](https://github.com/AP-Elektronica-ICT/BAP_Stage_StudentRepo/archive/master.zip)
* Unzip deze zip en plaats de content van de hoofdmap in je nieuwe repo. (dus de readme.md file en de overige mappen moeten in de root van je repo terechtkomen)
* Commit al deze nieuw toegevoegde zaken aan je repo en je kan beginnen.

*Mogelijkheid B*

* Open een shell met Git en clone de BAP_Stage_StudentRepo met
`git clone https://github.com/AP-Elektronica-ICT/BAP_Stage_StudentRepo.git`
* Ga naar de directory met de repo
`cd BAP_Stage_StudentRepo`
* Verander de remote origin van originele repo naar eigen repo
`git remote remove origin` en dan
`git remote add origin (jouw repo giturl hier)`
* Push de locale repo naar GitHub
`git push -u origin master`
* Commit al deze nieuw toegevoegde zaken aan je repo en je kan beginnen.


#### Tijdens de stage
* Standaard ben je geen admin van de repo. Indien je andere mensen toegang wil geven tot je repo, dan dien je admin-rechten via de stagecoördinator aan te vragen. *Het is aanbevolen dat ook je stagementor toegang heeft tot je repo.*
* Je repo hoeft niet als primaire repo gebruikt te worden voor je werk op het bedrijf. Indien het bedrijf bijvoorbeeld een eigen sourcecontrol-systeem heeft, dan gebruik je deze voor al je code. 
* Je gebruikt deze repo minstens als primaire punt voor je **scriptie, log, presentaties en verslagen**.
