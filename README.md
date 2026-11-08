# Belapp

Belhulp voor cold calling (Clever Concepts): gespreksboom, bellijst, afspraken, terugbellijst en spiekbrief. Eén zelfstandig HTML-bestand. Er staan geen gegevens of sleutels in deze repo.

Online: https://marcoryn-lang.github.io/belapp/

## Backup naar GitHub

Je gegevens staan in de browser van het apparaat. Met **Instellingen → Backup naar GitHub → Nu opslaan (backup)** gaat alles als één bestand (`belhulp.json`) naar een aparte **private** repo. Met **Laden van GitHub** haal je het op een ander apparaat weer binnen. Elke backup is een commit, dus oude versies blijven terug te vinden.

Eenmalig instellen:

1. Maak een private repo `belapp-data` aan (mag leeg zijn).
2. Maak een fine-grained token aan: GitHub → Settings → Developer settings → Fine-grained tokens. Kies bij Repository access alleen `belapp-data`, en bij Permissions → Contents: Read and write.
3. Open de app, ga naar Instellingen → Backup naar GitHub en plak het token. Gebruiker, repo en bestand zijn al ingevuld.

Wat er meegaat: bellijst, afspraken, terugbellijst, gesprekslog, spiekbrief, tellers, laatste verslag, aangepaste teksten, instellingen en het lopende gesprek. Het Pipedrive-token en het GitHub-token gaan bewust niet mee; die stel je per apparaat in.

## Gesprekken uitdraaien (CSV)

Elk gesprek komt als één regel in het gesprekslog, ook bij geen gehoor, voicemail, verkeerd nummer of niet meer bellen. Een gesprek telt zodra je één stap in het script zet of een uitkomst kiest. De begintijd is het moment waarop je op "Nieuw gesprek" klikt (of op "Bel nu" in de terugbellijst, of op "Volgende" in de bellijst).

Via **Instellingen → Uitdraaien → Gesprekken exporteren (CSV)** download je het log, eventueel voor een periode (Van / Tot en met). Kolommen: datum, tijd, bedrijf, contactpersoon, telefoon, zoekt, uitkomst, vervolg (demo of terugbelmoment dat je tijdens het gesprek vastlegde), bezwaren, kosten besproken, opening, notities en gebeld door. Het bestand gebruikt puntkomma's en opent direct in Excel. Het log begint bij de eerste versie met deze functie; eerdere gesprekken zitten er niet in.
