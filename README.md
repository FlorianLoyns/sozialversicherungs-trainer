# Sozialversicherungs-Trainer

**Die fünf Säulen der deutschen Sozialversicherung interaktiv lernen — Lerntool für die Pflegeausbildung**

[![Lizenz: CC BY-NC-SA 4.0](https://img.shields.io/badge/Lizenz-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.de)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue)](https://florianloyns.github.io/sozialversicherungs-trainer/)
![Keine Abhängigkeiten](https://img.shields.io/badge/Abh%C3%A4ngigkeiten-keine-brightgreen)
![PWA](https://img.shields.io/badge/PWA-offline--f%C3%A4hig-teal)

Eine browser-basierte App für Pflege-Auszubildende: die fünf Säulen der Sozialversicherung (Kranken-, Pflege-, Renten-, Unfall-, Arbeitslosenversicherung) als visuelle Tempel-Architektur erkunden — Säule anklicken, Detail-Karte erscheint mit Träger, Beitragssatz, Versichertenkreis, Leistungen und historischer Einordnung. Plus Übungs-Modus mit gestaffelten Schwierigkeitsgraden für die Examensvorbereitung.

**[Jetzt lernen](https://florianloyns.github.io/sozialversicherungs-trainer/)**

## Was die App enthält

Die fünf Säulen nach Stand 2025:

- **Krankenversicherung** (KV) — SGB V, 14,6 % + Zusatzbeitrag (~ 2,5 %), inkl. Familienversicherung und Krankengeld-Höhe
- **Pflegeversicherung** (PV) — SGB XI, 3,4 % (mit Kindern) bis 4,0 % (kinderlos), mit Hinweis auf Kinder-Abstaffelung und 5 Pflegegrade
- **Rentenversicherung** (RV) — SGB VI, 18,6 %, Wartezeit 5 Jahre für Regelaltersrente
- **Unfallversicherung** (UV) — SGB VII, allein vom Arbeitgeber getragen
- **Arbeitslosenversicherung** (AV) — SGB III, 2,6 %, Anspruch ALG I ab 12 Monaten Beitragszeit, mit Abgrenzung zum steuerfinanzierten Bürgergeld (SGB II)

Pro Säule werden zusätzlich Träger, Versichertenkreis, wesentliche Leistungen, abgesichertes Risiko und das **Einführungsjahr** (1883 KV bis 1995 PV) erläutert.

## Didaktischer Aufbau

**Lern-Modus** (Default): Visualisierung als Tempel-Architektur mit Dach, fünf Säulen und Fundament („Solidargemeinschaft"). Jede Säule klickbar — wird selektiv hervorgehoben, Detail-Karte aktualisiert sich live. Lernen durch Erkunden.

**Üben-Modus**: 15 Praxis-Szenarien in drei Schwierigkeitsstufen — drei einfache (Schlüsselwort-Erkennung), fünf mittlere (Anwendung, z. B. Wegeunfall, Berufskrankheit), sieben schwere (Stolperfallen wie Hausfrau-Putzen, Umweg-Wegeunfall, Reha bei Erwerbstätigen vs. Rentnern, Berufskrankheit-Reha). Schwierigere Fragen geben mehr Punkte. Auswertung mit prozentualem Score und Lerntipp.

## Technik

- Einzelne HTML-Datei, Vanilla JavaScript, keine Frameworks, kein Build-Tool
- Kein externes CDN, keine Abhängigkeiten zur Laufzeit
- **PWA**: installierbar auf Desktop und Smartphone, offline-fähig via Service Worker
- Mobile-First-Layout mit `safe-area-inset` für iPhone-Notch und Home-Indicator, Touch-Targets ≥ 44 px
- Mode-Wechsel (Lernen/Üben) als kompaktes Header-Dropdown
- DSGVO-konform: keine Tracker, keine externen Ressourcen, keine Datenübertragung

## Wartung

Beitragssätze, Versicherungspflichtgrenzen und Pflege-Beträge ändern sich regelmäßig. Empfohlen: einmal jährlich (typischerweise Januar) prüfen und im Code (`SAEULEN`-Objekt in `index.html`) aktualisieren. Die Jahresangabe im Disclaimer und im Lern-Intro entsprechend mit anpassen.

## Quellen

SGB III (Arbeitsförderung), SGB V (Krankenversicherung), SGB VI (Rentenversicherung), SGB VII (Unfallversicherung), SGB XI (Pflegeversicherung) — alle gemeinfreie amtliche Werke nach § 5 UrhG. Beitragssätze Stand 2025. Historische Einführungsdaten: Allgemeingut der deutschen Sozialgeschichte.

## Impressum

Verantwortlich: Florian Loyns. Pflichtangaben nach § 5 DDG: [Impressum](https://florianloyns.github.io/Impressum/)

## Lizenz

[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.de) · Nutzen, anpassen und teilen — unter Namensnennung, nicht-kommerziell und unter gleichen Bedingungen.
