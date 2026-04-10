# Dynamischer Strompreis Einsiedeln

Webseite zur Anzeige des dynamischen Stromtarifs von EKZ Einsiedeln AG in Echtzeit.

**[Live ansehen](https://ronaldreichmuth.github.io/strompreis-einsiedeln/)**

## Features

- Aktueller Strompreis in 15-Minuten-Intervallen (96 pro Tag)
- Tages-Übersicht mit Tiefstwert, Höchstwert und Durchschnitt
- Balkendiagramm mit farblicher Abstufung (grün = günstig, rot = teuer)
- Umschaltbar zwischen Gesamtpreis (Energie + Netz + Abgaben) und reinem Energiepreis
- Preise für morgen verfügbar ab ca. 18:00 Uhr
- Automatische Aktualisierung alle 5 Minuten

## Datenquelle

- [EKZ Tariffs API](https://api.tariffs.ekz.ch/swagger) (öffentlicher Endpoint, keine Authentifizierung nötig)
- Tarif: `integrated_400D_E` (EKZ Energie Dynamisch + Netz 400D, Einsiedeln)
- Alle Preise in Rp./kWh, exkl. MwSt.

## Technologie

Einzelne HTML-Datei ohne Build-Prozess. Verwendet [Chart.js](https://www.chartjs.org/) für die Visualisierung.
