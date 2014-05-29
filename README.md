RiskGame introductie
======================

### De opdracht
**Eisen aan de opdracht:**
- De opdracht moet tof zijn om te bouwen.	
- De opdracht geeft de student genoeg diepgang.	
- De opdracht maakt gebruik van ten minste 3 objecten, waarvan 1 een overervingsrelatie heeft met een ander object.	
- Bij de opdracht is het logisch om een MV* patern toe te passen.	
- Er zijn meerdere events nodig voor een goede werking van het programma.

======================

### Mijn opdracht: RiskGame
Ik maak een spel (genaamd: RiskGame). 
RiskGame is een spel waarin twee spelers 'turn-based' tegen elkaar opnemen om zoveel mogelijk gebieden te pakken en daarover controle te houden.
Elke speler krijgt zijn eigen kleur en beheerd zijn eigen troepen en gebieden.
De spelers winnen zodra ze alle gebieden hebben of dat ze na een bepaald aantal beurten de meeste munten hebben of gebieden beheersen.

#### De kaart
De kaart van RiskGame is vierkant en bestaat uit allemaal kleine gebieden.
De gebieden zijn zichtbaar door de kleine vierkantjes.
Als speler is het de bedoeling dat je alle gebieden gaat beheersen en dat je deze gebieden onder controle gaat houden.

Dit is een voorbeeld van de kaart:

![kaart RiskGame](https://raw.githubusercontent.com/SEALdvd/FED01_0846138_RiskGame/master/Overige_bestanden/res/kaart.png "Kaart RiskGame")

#### Gebieden
Er zijn verschillende gebieden die je als speler kan veroveren.

De gebieden:
- normaal gebied: +1 munt
- kasteel gebied: +3 munten + 1 schat

Een gebied kan maximaal drie troepen hebben van een enkele speler.
Onderstaand staat er een voorbeeld van een afbeelding van de gebieden (links: normaal en rechts: kasteel):

![gebieden RiskGame](https://raw.githubusercontent.com/SEALdvd/FED01_0846138_RiskGame/master/Overige_bestanden/res/gebieden.png "Gebieden RiskGame")

Elk gebied wordt staat onder controle door een van de spelers of door 'niets'.
De gebieden krijgen als rand (border) de kleur van de speler of een normale zwarte rand als het door niets wordt beheerd.

#### Munten
Een speler krijgt door gebieden te beheersen elke beurt munten erbij.
Elk gebied levert een aantal munten op waarmee de speler later extra troepen kan bijbouwen.
Het is ook mogelijk dat een speler door een bepaald aantal munten te bereiken het spel te winnen.
Elke speler krijgt vijftien munten in het begin waarbij de speler troepen kan kopen.

#### Schatten
Een kasteel levert schatten op.
Als een schat wordt opengemaakt dan krijgt de speler direct een bonus.
Een schat wordt random gekozen.

Bonussen:
- geen bonus (65% kans)
- 5 munten erbij (20% kans)
- 10 munten erbij (10% kans)
- 20 munten erbij (5% kans)

#### Troepen en troepen verplaatsen
Elke speler krijgt drie troepen in het begin, wat gelijk staat aan het maximaal aan troepen in een gebied.
Om troepen te kopen moet de speler het gebied selecteren waarin de speler de extra troepen wilt hebben.
De troepen kosten vijf munten per stuk en het maximaal aantal troepen wat in een gebied kan staan blijft het maximum.
Dus gebieden waar een of twee troepen staan kunnen enkel versterkt worden.

Het is mogelijk om troepen te verplaatsen. Er zijn wel twee soorten verplaatsingen: veroveringen en versterkingen.
Troepen kunnen alleen aan aangrenzende gebieden lopen.
Je verplaats altijd het maximale aantal troepen.

##### Versterkingen
Om je eigen gebieden te versterken verplaatst moet de speler het gebied aanklikken waaruit de troepen komen.
Daarna klikt de speler de plaats aan waar de troepen moeten staan. 
Je kan alleen troepen verplaatsen als er in het aangrenzende gebied minder dan drie troepen staan en het gebied waar de versterking vertrekt minimaal twee troepen staan.
Er blijft altijd een enkele eenheid achter waaruit de versterking is vertrokken.

##### Veroveringen
Hierbij valt de speler een andere speler of een gebied aan zonder speler.
Als speler klik je eerst je eigen gebied aan dan het gebied waar de andere speler staat.
Dan is het mogelijk om de troepen te verplaatsen.
Als aanvaller is het mogelijk om maximaal met twee troepen aan te vallen en minimaal met een.
Het aantal troepen dat de aanval niet overleeft is gelijk aan de troepen die de verdediger heeft staan.

Mogelijke scenario's:
| Gebied aanvaller	| Aanval	| Gebied verdediger   | Winnaar (overlevende troepen)  |
| :--------------------|:-------------:| :------------------:|------------------------------:	|
| 1     		| 0		| 1  	      	      |	Geen aanval mogelijk		|
| 2     		| 1     	| 1	              | Niets (0)			|
| 3 			| 2      	| 3                   | Verdediger (1)			|
| 3 			| 2      	| 2                   | Aanvaller (1)			|
| 2 			| 1      	| 3                   | Verdediger (2)			|

### Afbeelding(en)
![RiskGame gameplay](https://raw.githubusercontent.com/SEALdvd/FED01_0846138_RiskGame/master/Overige_bestanden/res/voorbeeldGame.png "RiskGame gameplay")
