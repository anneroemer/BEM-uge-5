# BEM-uge-5

Opgave:

Lav et markdown (md) dokument på din Github.

Og skriv hvad der tales/beskrives på følgende tidspunkter i videoen:

(emnet startes ved tiden og varer x-antal minutter)

03.50 - 05.20 - 06.30 - 08.57 - 19.05 - 20.50 - 22.06 - 24.20

Og afslutningsvis skal du nu med egne ord skrive lidt om hvad du fik ud af videoen.


## ** 3.50 - Objekt oriented programming **

Decoupling: handler om at adskille elementerne så de er lettere at ramme indidviduelt. 
Single responsibility principle: sørge for at den individuelle css kode er så simpel som muligt. Dvs. at den ikke håndterer mange opgaver på én gang.
Encapsulation: at en css regel kan tages ud og bruges andre steder...? 


## ** 5.20 - emne **

Samme som ovenstående...?


## ** 6.30 - OOCSS Pattern identification **

Man identificerer mønstre der går igen for mange elementer og laver et overordnet "modul" der kan bruges mange forskellige steder. I hans eksempel med et facebook layout: .media der gælder alt indhold, og dernæst .img og .bd (body). 


## ** 8.57 - SMACSS Scalable Modular Architecture **

Overordnede gruperinger af indhold:

Base - HTML objekter ex: H2, ul, a og ID's.

Layout - store sektioner i html'en. Ex. header, sidebar, body, footer.

Module - som beskrevet i 6.30. Moduler der beskriver et mønster. Genbrugelige.

State - i forbindelse med javascript. Kan være fx. .active-state. State er noget der afgør hvordan noget blive displayet.

Theme - ex. Valentinsdags tema, blåt tema etc. Nærmest aldrig brugt. 


## ** 19.05 - Specificity **

To css regler der rammer det samme: den der står længst nede i style sheetet vinder.
Jo mere specifik en selector er, jo større chance er der for at den overruler andet css. En dobbelt selector vil derfor have større vægt og overrule en single selector. 
Ex. .body h1 vs. .body-h1. Så selvom at de rammer samme element, og den ene class sidder specifikt på det element, vi gerne vil ramme, vil den dobbelte selector vinde.


## ** 20.50 - emne **

Samme som ovenstående. 


## ** 22.06 - emne **

En ID vil overrule alt andet. Der skal skrives omkring 600 classes før de måske vil kunne overrule en ID.


## ** 24.20 - emne **

CSS regler bliver læst bagfra. Dvs. "nav ul li" finder alle li'er. Dernæst alle li'er der ligger i en ul. Dernæste alle de li'er i ul'er som ligger i en nav. En specifik class henvender sig derimod direkte til det givne element man gerne vil have fat i. 

En flat selector bliver indlæst hurtigere, det er nemmere at finde rundt i, det er nemmere at lave en class der gør det modsatte fx og overrule den første class, fordi de har præcis den samme specificity. 

## **Hvad fik jeg ud af videoen**

Specifikke classes skrevet med samme syntaks er en kæmpe fordel, fx når man arbejder på større projekter eller hvis andre skal bruge ens kode. Det er nemmere at hive fat i noget indhold og ændre det/pille det ud, uden at resten af indholdet bliver 
påvirket. Det gør at alt har samme specificity, så at de forskellige css regler ikke ligger og spærrer for hinanden. ID's er bedste at bruge udelukkende til js hooks - ikke til styling, da de vil overrule alle andre regler der er lavet.

