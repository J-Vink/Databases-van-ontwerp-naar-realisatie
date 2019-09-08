# Hoofdstuk 2: Datamodellering
- Opdracht 2.1.1: geef een korte, samengevatte, omschrijving van het conceptueel model.
    - Een conceptueel model dient als, zoals een managementsamenvatting, een korte maar exacte beschrijving over hoe de database eruit komt te zien. Hierin worden punten zoals wensen en eisen van de klant benoemd.

- Opdracht 2.2.1: Wat is het attribuut dat de verschillende klassen binnen je school onderscheidt?
    - Klasnummer is hier de factor dat voor de onderscheiding zorgt.

- Opdracht 2.2.2: Wat zijn de waarden van de unique identifier van de klaslokalen?
    - Lokaalnummer is de unique identifier van de klaslokalen.

- Opdracht 2.2.3: Stel dat je een database moet maken voor een autohandelaar. Benoem een aantal entiteiten dat binnen het ERM gerealiseerd moet worden.
    - Vestigingen[id, locatie, managerid] Medewerkers[id, positie, salaris, vestigingsid] Auto[Merk, type, kenteken, cataloguswaarde, kmstand, vestiginsid].

- Opdracht 2.2.4: Wat zou je zelf voorstellen als unique identifier voor een auto te gebruiken?
    - Het kentekennummer.

- Opdracht 2.2.5: Wat valt je op aan de unique identifier van de onderste entiteit? Is dit dan wel een geschikte unique identifier? Wat zou je zelf voorstellen?
    - Het ligt aan de context of een artiestennaam geschikt is als unique identifier. Een betere oplossing als unique identifier zal een ID of zelfs zoiets als een BSN zijn.

- Opdracht 2.2.6: Zou een e-mailadres mandatory of optioneel zijn binnen de database van jouw school?
    - Mandatory, puur wegens het feit dat lesmateriaal gekoppeld wordt aan jouw account (in dit geval je school-account)

- Opdracht 2.2.7: Zou een combinatie van voornaam en achternaam echt een goede unique identifier zijn? Wat zou een betere zijn?
    - Op Mondriaan bevinden zich wel meerdere individuen met de naam 'Jeffrey Vink', een betere identifier is een studentnummer.

- Opdracht 2.2.8: Welke unique identifier hebben alle personen gekregen binnen Nederland?
    - Het burgerservicenummer (BSN)

- Opdracht 2.2.9: Benoem entiteiten die gebruikt zouden kunnen worden bij de classificering van een online-spel in een database.
    - Platform, Game

- Opdracht 2.2.10: Benoem enkele instanties van de entiteit MMORPG.
    - (RuneScape 3, Jagex, Verenigde staten, 2001) (World of Warcraft, Blizzard, Verenigde staten, 2006)

- Opdracht 2.2.11: Schrijf een aantal attributen op dat betrekking heeft op de entiteit game. Welk attribuut zou hier als unique identifier kunnen dienen?
    - Naam, ontwikkelaar, land, releasedatum. Een unique identifier kan ook hier een ID zijn, maar ook een combinatie van naam en ontwikkelaar of releasedatum.

- Opdracht 2.2.12: Ga naar (link) en typ daar een merknaam in. Wat is meestal toegevoegd naast een merknaam om een unique identifier te verkrijgen?
    - Merk nr is in dit geval een unique identifier.

- Opdracht 2.3.1: Benoem de elementen binnen een ERD en probeer vast te stellen hoe ze grafisch worden weergegeven.
    - Studentid, voornaam, achternaam, klas.

- Opdracht 2.3.2: Bepaal in bovenstaande tabel de entiteiten. Noteer de attributen per entiteit.
    - Entiteiten: auto(type, brandstof, carrosserievorm) merk(merknaam) dealer(adres, postcode)

- Opdracht 2.4.1: Bekijk de afbeeldingen en noteer wat ze uitbeelden.
    - Emoties: tevreden, ontevreden, boos.

- Opdracht 2.4.2: Bestaat een conceptueel model geheel uit een ERD?
    - Nee, een ERD maakt beeld het ERM alleen visueel uit.

- Opdracht 2.4.3: Welk attribuut is de unique identifier? Welke attributen zijn mandatory of optioneel?
    - afdeling_id is uniek en mandatory, 'naam' en 'manager_id' zijn mandatory. 'commentaar' is hierbij optioneel.

- Opdracht 2.4.4: Als je naar het ERD kijkt van de entiteit afdeling, kun je dan de conclusie trekken of er verschillende afdelingen met dezelfde id zijn binnen de organisatie waar de entiteit betrekking op heeft?
    - Omdat de afdeling_id uniek moet zijn, zijn er geen meerdere afdelingen die dezelfde id dragen. Daarentegen kunnen verschillende afdelingen wel dezelfde manager_id hebben, omdat deze niet uniek moet zijn.

- Opdracht 2.4.5: Kunnen er van de entiteit verkoper diverse instanties zijn met dezelfde achternaam?
    - Ja, achternaam is wel een verplicht veld, echter hoeft deze niet uniek te zijn.

- Opdracht 2.6.1: Kun je bij het zien van de softbox afdeling concluderen of elke afdeling een manager heeft? Verklaar je antwoord.
    - Ja, omdat manager id een verplicht veld is.

- Opdracht 2.6.2: Moet elke afdeling een andere manager hebben? Verklaar je antwoord.
    - Nee, ondanks dat het veld verplicht is, dient het niet uniek te zijn.

- Opdracht 2.6.3: Nu is er in het ERD hierboven een directe relatie tussen de agdeling en haar manager. Zou dit ook mogelijk zijn tussen de entiteiten verkoper en manager? Wat zou je zelf handiger/duidelijker vinden?
    - De verkoper kan beter een directe relatie hebben met de afdeling dan met de manager, aangezien de manager een relatie kan hebben met meerdere afdelingen. Hierdoor kan het lastig worden om te zien bij welke afdeling de verkoper daadwerkelijk werkzaam is.

- Opdracht 2.6.4: Door de relatielijn tussen afdeling en manager is er een overbodig attribuut in een van beide tabellen. Verbeter nu bovenstaand ERD.
    - .

- Opdracht 2.7.1: Teken het ERD dat hoort bij onderstaand scenario. Schrijf eerst voor jezelf de business rule op waar het om gaar. Schrijf daarna de relatie uit in ERDish. Gebruik daarbij Engels.
    - Eén docent moet les geven aan meerdere klassen, maar een klas kan les krijgen van één docent.
    - ERDish: EACH DOCENT must be teaching one / more than one KLAS
    - ERDISH: EACH KLAS may be teached by one DOCENT

- Opdracht 2.7.2: Teken het ERD dat hoort bij onderstaand scenario. Schrijf eerst voor jezelf de business rule op waar het om gaar. Schrijf daarna de relatie uit in ERDish. Gebruik daarbij Engels.
    - Een docent moet les geven aan meerdere klassenen een klas moet van minstens één docent les krijgen.
    - ERDish: EACH DOCENT must be teaching one / more than one KLAS
    - ERDISH: EACH KLAS must be teached by one / more than one DOCENT





