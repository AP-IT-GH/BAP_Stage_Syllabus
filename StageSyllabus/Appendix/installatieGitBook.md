# Gitbook installatie handleiding
Je scriptie moet geschreven worden in markdown en dient steeds ook naar een pdf geconverteerd te worden. We gaan hier voor [GitBook](https://github.com/GitbookIO/gitbook) gebruiken (zie voorbeeld in  je studentrepo in de map Scriptie)

## Git installatie en setup
*De kans bestaat dat je Git al hebt geinstalleerd dit kan door [GitHub Desktop](https://desktop.github.com) of [SmartGit](http://www.syntevo.com/smartgit/). In dat geval kan je de eerste stap overslaan.*

Download [Git](http://www.syntevo.com/smartgit/) en start de installatie. Tijdens de setup selecteer je **Use Git from the Windows Command Prompt**. 
Na de installatie test je of je Git overal kan gebruiken door cmd (Start => Run => cmd) te openen en vervolgens git [enter] in te voeren. Dit moet de help text van git tonen, als dit het geval is kan je doorgaan naar de Node.js installatie.

### Voor Git Desktop en SmartGit gebruikers (of als git.exe na installatie niet werkt)
Werkt je git.exe commando niet? Dan is het path naar de plek waar dit commando staat niet toegevoegd aan je systeem variabelen. 
Voeg Git toe aan de PATH variabele van windows: (Open Control Panel => System And Security => System => Advanced System Settings => Environment variables)

Onder **User variables for [UserName]** staan jou omgevings variabelen. Als PATH hier al tussen staat klik je hier op en vervolgens op Edit, anders klik je op New en geef je deze de naam PATH.
Als waarde geef je het path naar je git.exe:

*  Git setup: `C:\Program Files (x86)\Git\bin` 
*  SmartGit: `C:\Program Files (x86)\SmartGit\git\cmd`
*  Git Desktop: `C:\Users\[UserName]\AppData\Local\GitHub\PortableGit_[Random numbers and letters]\cmd` (ga dit eerst via explorer zoeken)

*__Let Op!__
Als je een bestaande PATH bewerkt voeg je het Git path toe __achter__  het bestaande PATH __gescheiden met ;__
Vb: `C:\mijn\bestaande\path;C:\Users\Robert\AppData\Local\GitHub\PortableGit_c2ba306e536fdf878271f7fe636a147ff37326ad\cmd`*
Als je klaar bent sluit je alle vensters door op Ok te klikken en test dit vervolgens door een command prompt (Start => Run => cmd) te openen en vervolgens git [enter] in te voeren. Indien dit werkt kan je vervolgens verder gaan naar de Node.js installatie.

## Node.js installatie
GitBook is een programma gebouwd op Node.js, dit moeten we dus eerst installeren.
*Als je een volledige installatie van VisualStudio hebt gedaan is Node.js waarschijnlijk al geïnstalleerd. Test dit door in de cmd `npm --version`uit te voeren. Als dit een versienummer geeft kan je verder gaan naar de GitBook installatie.*

Om Node.js te installeren download je [hier](https://nodejs.org/download/release) de juiste setup file (\*.msi). Start de setup en voer een volledige installatie uit.
Test vervolgens of Node.js werkt door een **nieuwe** cmd te openen en `npm --version` uit te voeren. Werkt dit dan kan je doorgaan naar de GitBook installatie.

## Gitbook installatie
Om GitBook te installeren open je cmd en voer vervolgens volgende opdracht uit:  `npm install gitbook-cli -g`.
Als dit klaar is is GitBook  geïnstalleerd.

Lees vervolgens [deze](https://github.com/GitbookIO/gitbook#how-to-use-it) tekst en experimenteer wat.
**Merk op dat git init niet meer hoeft in je scriptie map. Test dit best ook even in eigen map zodat je zeker bent dat alles goed werkt.**

## Pdf Generatie
Het commando `gitbook pdf` kan je gebruiken om je tekst naar een pdf te outputten. Hiervoor heb je volgens de gitbookdocumentatie ebook-convert nodig. De eenvoudigste manier om dit te installeren is door eenvoudigweg de open source [ebook manager "Calibre"](http://calibre-ebook.com/download) te installeren. Merk op dat dit niet zal werken indien je de portable versie van Calibre installeert.
Voeg nu `C:\Program Files\Calibre2` toe aan je PATH variabele, dit zorgt er voor dat gitbook ebook-convert.exe kan aanroepen.
**Merk op dat je PATH ondertussen ook volgende locatie bevat `C:\Users\[UserName]\AppData\Roaming\npm` voor Node.js.**

# En nu?
Het is aanbevolen om eerst de uitleg op https://github.com/GitbookIO/gitbook  bij "Book Format" te lezen. Bekijk zeker hoe je de SUMMARY.md file kunt gebruiken om met meerdere files te werken zodat je tekst niet in 1 groot document terechtkomt.

Uiteraard zal je ook de, uiterst eenvoudige, Markdown (MD) syntax moeten leren. Hiervoor zijn tal van websites zoals https://help.github.com/articles/markdown-basics/ en http://markdowntutorial.com/ .

# Tip: Snel book builden
Telkens je je gitbook wilt compileren (naar een website of pdf) dien je bijvoorbeeld het commando `gitbook pdf` in te typen. Je kan dit proces versnellen door in de root van je gitbook een .bat bestand toe te voegen (bv `buildnbook.bat`). In dit bestand zet je dan de commando's die je wilt uitvoeren (in mijn geval: `gitbook pdf`). Telkens je nu dit .bat bestand uitvoert zal je boek gecompileerd worden.
