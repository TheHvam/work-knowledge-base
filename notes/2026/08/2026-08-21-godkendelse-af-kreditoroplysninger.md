# Kontrol af ændringer i kreditoroplysninger

Dato: 2026-08-21

Tags: relate-and-learn, business-central, procure-to-pay, kreditoroplysninger, intern-kontrol, funktionsadskillelse

## Noter

Relate & Learn skal afklare en mulig løsning til kontrol af ændringer i kreditorers bankoplysninger. Området er en del af Business Centrals Procure to Pay-proces og skal adressere revisionskrav om forebyggende kontroller af ændringer i kritiske kreditorstamdata.

## Forventet slutmål

- Have en klar implementeringside og kunne identificere tekniske udfordringer ved en senere løsning.
- Udarbejde procesdiagrammer, der forklarer processen fra start til slut.
- Gennemføre feasibility og etablere et godt grundlag for Firm Foundation.
- Om muligt afklare relevante forhold for den efterfølgende Build & Deliver-fase.

## Afgrænsning

- Fokus er ændringer i kreditorstamdata, særligt kreditors bankoplysninger, og deres betydning for udbetalinger.
- Processen skal beskrive anmodning, dokumentation, kontrol, godkendelse, implementering, betaling og efterfølgende overvågning.
- Revisionens konkrete krav skal afklares med Kurt, som har dialogen med revisoren.

## Krav til kontrol

- Ingen må kunne ændre en kreditors kritiske oplysninger uden en uafhængig godkendelse.
- Forebyggende kontroller skal så vidt muligt automatiseres, da afdelingen ikke har yderligere ressourcer.
- Opdagende kontroller behøver ikke være automatiserede, men skal være robuste og give høj sikkerhed for, at regelbrud og undtagelser opdages.
- Løsningen skal understøtte funktionsadskillelse gennem rettigheder og workflow.

## Roller og funktionsadskillelse

| Funktion | Ansvar | Må ikke udføre |
| --- | --- | --- |
| Anmoder | Oprette forslag til ændring og vedhæfte dokumentation | Godkende eller implementere egen ændring |
| Kreditoradministrator | Vedligeholde kreditorstamdata efter godkendelse | Godkende egen ændring eller ændringer, som vedkommende selv har oprettet |
| Godkender | Kontrollere ændringen og godkende eller afvise | Oprette eller implementere den samme ændring |
| Betalingsansvarlig | Gennemføre eller frigive betalinger | Ændre kreditorens bankoplysninger |
| Kontrolfunktion/revision | Overvåge ændringer, undtagelser og brud på regler | Daglig behandling af ændringsanmodninger |
| Systemadministrator | Administrere systemadgang og workflow | Foretage forretningsmæssige ændringer uden særskilt logning og efterkontrol |

## Interessenter

- Direktør eller finansdirektør skal kontaktes først for overblik over den interne organisering og ansvarlige for processerne.
- Kurt skal kontaktes for at konkretisere revisors krav til forebyggende kontroller og regeloverholdelse.

## Leverancer og næste skridt

- Afdæk nuværende proces, stamdatafelter, udbetalingsflow, roller, rettigheder og eksisterende revisionsspor i Business Central.
- Beskriv krav, undtagelser og tekniske afhængigheder for workflow, godkendelse, logning og adgangsstyring.
- Udarbejd procesdiagrammer for nuværende proces og ønsket fremtidig proces.
- Vurder feasibility og dokumenter beslutninger og åbne tekniske spørgsmål som input til Firm Foundation og eventuelt Build & Deliver.
