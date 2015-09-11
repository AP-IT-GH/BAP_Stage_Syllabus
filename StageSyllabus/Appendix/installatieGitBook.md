# Gitbook installatie handleiding
Je scriptie dient geschreven te worden in markdown en steeds ook naar een pdf geconverteerd te worden. We gaan hierbvoor [gitbook](https://github.com/GitbookIO/gitbook) gebruiken (zie voorbeeld in  je studentrepo in de map Scriptie)
## Git installatie en setup
Installeer eerst Git via https://git-scm.com/downloads 
Zorg ervoor dat het ``git.exe`` commando overal beschikbaar is. Test dit door een command prompt (Start=>Run>cmd) te openen en vervolgens git [enter] in te voeren. Indien dit werkt kan je vervolgens verder gaan naar Gitbook installatie.

###Git systemwide toevoegen
Werkt je git.exe commando niet? Dan is het path naar de plek waar dit commando staat niet toegevoegd aan je systeem variabelen. Standaard staat deze exe op ``C:\Program Files (x86)\Git\bin``.
Dit path voeg je toe aan je PATH systeem variabele, zoals [hier](http://windowsitpro.com/systems-management/how-can-i-add-new-folder-my-system-paths) uitgelegd.


## Gitbook installatie

https://nodejs.org/download/

Zeker npm package manager kiezen. 

Voort vervolgens volgende opdracht uit:  ``npm install gitbook-cli -g``

Lees vervolgen [deze](https://github.com/GitbookIO/gitbook#how-to-use-it) tekst en experimenteer wat.
**Merk op dat git init niet meer hoeft in je scriptie map. Test dit best ook even in eigen map zodat je zeker bent dat alles goed werkt.**


## Pdf Generatie

Het commando ``gitbook pdf`` kan je gebruiken om je tekst naar een pdf te outputten. Hiervoor heb je volgens de gitbookdocumentatie ebook-convert nodig. De eenvoudigste manier om dit te installeren is door eenvoudigweg de open source [ebook manager "Calibre"](http://calibre-ebook.com/download) te installeren. Merk op dat dit niet zal werken indien je de portable versie van Calibre installeert.

# En nu?

Het is aanbevolen om eerst de uitleg op https://github.com/GitbookIO/gitbook  bij "Book Format" te lezen. Bekijk zeker hoe je de SUMMARY.md file kunt gebruiken om met meerdere files te werken zodat je tekst niet in 1 groot document terechtkomt.

Uiteraard zal je ook de, uiterst eenvoudige, Markdown (MD) syntax moeten leren. Hiervoor zijn tal van websites zoals https://help.github.com/articles/markdown-basics/ en http://markdowntutorial.com/ .

# Tip: Snel book builden
Telkens je je gitbook wilt compileren (naar een website of pdf) dien je bijvoorbeeld het commando ``gitbook pdf`` in te typen. Je kan dit proces versnellen door in de root van je gitbook een .bat bestand toe te voegen (bv ``buildnbook.bat``). In dit bestand zet je dan de commando's die je wilt uitvoeren (in mijn geval: ``gitbook pdf``). Telkens je nu dit .bat bestand uitvoert zal je boek gecompileerd worden.
