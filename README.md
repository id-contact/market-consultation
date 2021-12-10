*Deze marktconsultatie is inmiddels afgerond. Wij danken de partners die input hebben geleverd naar aanleiding van onze marktvraag.*

| Inleiding | [Plugin Telefonie](./telephony.md) | [Plugin Chat](./chat.md)| [Plugin Video](./video.md) | [Reageren op deze marktverkenning](./reactions.md) |
| ----- | ----- | ----- | ----- | ----- |

# ID Contact Marktconsultatie
De gemeenten Arnhem, Nijmegen en de Drechtsteden werken samen met de Belastingdienst, Digicampus (Logius), NOVUM (Sociale Verzekeringsbank), Hogeschool Arnhem-Nijmegen (HAN) en het iHub (Radboud Universiteit) aan de innovatiepilot ID Contact. Het project werkt iteratief (SCRUM) aan de ontwikkeling in samenwerking met ontwikkelpartner Tweede Golf.
Het doel is om middels authenticatie op afstand vast te stellen of iemand daadwerkelijk is wie die beweert te zijn door specifieke persoonsgegevens te delen. Hierna is de identiteit vastgesteld en kunnen persoonlijke zaken makkelijke, veilige en betrouwbare wijze worden afgehandeld. Zowel via de telefoon (ID Bellen) als via chat (ID Chat) als via videocontact (ID Video). 
ID Contact heeft de potentie om op te schalen naar alle Nederlandse gemeenten en ook commerciële partijen tonen inmiddels belangstelling.

Meer algemene informatie is te vinden op [idcontact.nl](https://www.idcontact.nl).

## Wat is ID Contact
De codebase van ID Contact is open source. Het project ID Contact levert vrij toegankelijke bouwblokken op die (opnieuw) te gebruiken zijn door (overheids-)organisaties. Deze bouwblokken beschrijven het gebruik van open software, de werkwijze van de pilot, de communicatiestrategie en zowel de manier van onderzoeken als de resultaten.

ID Contact werkt met een kernapplicatie welke communiceert met authenticatie plugins en communicatie plugins. Over de eerste gaan de gegevens van de inwoner, over de tweede de communicatie met de gemeente. Een communicatie plugin heeft twee basisfuncties: de informatie uit de authenticatie plugin tonen en zorgen dat de inwoner en gemeente met elkaar kunnen communiceren. We bouwen een communicatieplugin voor bellen, chat en video. 

De werking van ID Contact en de techniek die daarvoor is ontwikkeld staat beschreven op de website [docs.idcontact.nl](https://docs.idcontact.nl). Hier vind je ook een uitgebreide beschrijving van de werking van de communicatieplugin, maar we vatten de verantwoordelijkheden van een communicatieplugin hier in een aantal punten kort samen:
- Bij het aanmaken van een sessie bepalen waar gebruiker naartoe kan worden verwezen om de communicatie te starten. Bij bellen is het typisch een telefoonnummer + dtmf, bij chat en video een URL met sessie ID.
- Bij het aanmaken van een sessie bepalen waar een authentiecatieplugin attributen voor deze sessie naartoe kan sturen nadat authenticatie doorlopen is.
- Het kortstondig opslaan van attributen met als enige doel om deze te tonen aan de agent bij de communicatiesessie
- Het verbinden van de inwoner en de agent om de communicatie plaats te laten vinden.

Voor ID Video is er nog een extra verantwoordelijkheid te onderscheiden, omdat er bij deze plugin pas authenticatie plaatsvindt nadat de communicatie gestart is.
- Het tonen van een keuzemenu van de beschikbare authenticatiemethoden, om na een keuze door te kunnen verwijzen naar de omgeving van de gekozen authenticatiemethode middels een browser-redirect.

Meer informatie over deze communicatieplugins vind je bij [ID Bellen](./telephony.md), [ID Chat](./chat.md) en [ID Video](./video.md).

## Waar staat ID Contact nu?
We bevinden ons momenteel in fase I van het project dat loopt tot de zomer van 2021. Voor Bellen en Chat hebben we met een Proof on Concept (PoC) inmiddels aangetoond dat het kan werken. Voor deze PoC hebben we een authenticatieplugin gebouwd voor de authenticatiemethode IRMA en communicatieplugins voor de opensource platformen Amazon Connect (bellen) en Matrix (chat). In een iteratief proces met inwoners ontwerpen en ontwikkelen we momenteel op volle kracht de UI guidelines. In fase II van het project zal de focus liggen op opschaling en legitimatie van het product. 

## Onze vraag aan de markt
In fase I zoeken we input van de markt. Kunnen potentiële integratiepartners aansluiten op basis van wat we tot nu toe hebben ontwikkeld? Of zijn er nog aanpassingen aan ID Contact nodig? En als partners kunnen aansluiten, wat is daarvoor nodig? Hoe ziet het technisch ontwerp er dan uit? Maar ook zoeken we naar de haalbaarheid in de vorm van geschatte doorlooptijd, de eenmalige kosten en het commerciële model dat de integratiepartner voor ogen heeft. En natuurlijk staan we open voor mogelijke alternatieve oplossingen voor de plugins of verbetervoorstellen voor zowel plugins als de core-applicatie.

Graag willen we alle mogelijke integratiepartners op het vlak van bellen, chat en video de mogelijkheid bieden om mee te denken over de verdere ontwikkeling van deze plugins. 
In deze fase van het project is het niet mogelijk om een vergoeding te stellen tegenover de inzet van de potentiële integratiepartners. 

## Over deze marktconsultatie
ID Contact is een innovatief project. Dat betekent dat we momenteel volop in de eerste fases van productontwikkeling zitten. In latere fases wordt ID Contact steeds meer productiewaardig, en in de tussentijd onderzoeken we steeds hoe het beter kan. Wij realiseren ons goed dat het product pas van waarde is als het actief wordt gebruikt en doorontwikkeld. 
Input van experts uit de markt en stakeholders is voor de ontwikkeling van ID Contact van grote meerwaarde. We nodigen daarom iedereen uit om mee te denken middels deze marktconsultatie. 
Het projectteam kan bovendien ondersteuning bieden bij het ontwikkelen van een bouwsteen voor ID Contact, zoals een authenticatie of communicatie plugin. Ook dit zou voor ons van enorme meerwaarde zijn om de toepassing van ID Contact in de praktijk te toetsen. Het projectteam heeft beperkte capaciteit voor het begeleiden van een dergelijke integratie. Indien de situatie zich voor doet dat de animo groter is dan de capaciteit, Zullen we ons beraden op een transparante selectie .Het kan dus zijn dat we hierin een keuze moeten maken tussen indieners. Desalniettemin zijn alle partijen welkom om op eigen initiatief een integratie plugin te ontwikkelen m.b.v. de open source beschikbare documentatie en code. Alle informatie is openbaar en te vinden op [docs.idcontact.nl](https://docs.idcontact.nl).

## Uitgangspunten voor de markconsultatie
- Door voor een brede vertegenwoordiging van ondernemers te kiezen wil AD voorkomen dat de schijn gewekt wordt dat de aanbesteding wordt toegeschreven naar één ondernemer en wil AD daarmee van meet af aan maximaal voldoen aan het transparantie- en het gelijkheidsbeginsel
- Bij een transparante werkwijze is de kans op het succesvol afronden van de toekomstige Europese aanbesteding maximaal.
- De door ondernemers aangeleverde feedback zijn adviezen van de ondernemers. AD behoudt zich het recht voor deze adviezen (deels) wel of (deels) niet over te nemen.
- De verkregen informatie van de ondernemers wordt vertrouwelijk behandeld en geanonimiseerd en heeft - in positieve of negatieve zin - geen enkele invloed op de individuele beoordelingen van toekomstige inschrijvingen en de kans op het verkrijgen van de opdracht. Ook als een uitgenodigde ondernemer besluit om van deelname aan deze marktverkenning af te zien, heeft dat geen enkele invloed op de individuele beoordelingen van toekomstige inschrijvingen en de kans op het verkrijgen van de opdracht.

Gedurende de marktverkenning wordt door AD geen informatie verstrekt aangaande de overige aanbestedingsstukken en/of de beoordelingsmethodiek. Enerzijds om recht te blijven doen aan het gelijkheidsbeginsel betreffende ondernemers die niet uitgenodigd zijn voor deze marktverkenning. Anderzijds zal de wijze waarop de aanbesteding uitgeschreven gaat worden mede afhankelijk kunnen zijn van de ontvangen feedback. 

Marktpartijen die geïnteresseerd zijn om mee te denken, worden gevraagd deze marktconsultatie zorgvuldig te lezen en te reageren op de genoemde vragen. Deze zijn per kanaal gegroepeerd in de verschillende tabbladen. Meer informatie over dit marktraadplegingsproces is te vinden in [Reageren op deze marktverkenning](./reactions.md).
