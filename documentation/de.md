<!-- ELUCENIA technical documentation · nrs-2002 · de · no clinical/professional/rights approval -->

# NRS-2002

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/nrs-2002)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Beeinträchtigung des Ernährungszustands

`estado`

- `0` — Nicht vorhanden: normaler Ernährungszustand
- `1` — Leicht: Gewichtsverlust \> 5 % in 3 Monaten oder Aufnahme von 50 bis 75 % des Bedarfs in der letzten Woche
- `2` — Mäßig: Verlust \> 5 % in 2 Monaten oder BMI 18,5 bis 20,5 bei beeinträchtigtem Allgemeinzustand oder Aufnahme von 25 bis 60 %
- `3` — Schwer: Verlust \> 5 % in 1 Monat (\> 15 % in 3 Monaten) oder BMI \< 18,5 bei beeinträchtigtem Allgemeinzustand oder Aufnahme von 0 bis 25 %

### Krankheitsschwere (erhöhter Bedarf)

`gravidade`

- `0` — Nicht vorhanden: normaler Ernährungsbedarf
- `1` — Leicht: Hüftfraktur, chronische Erkrankung mit akuter Komplikation (Zirrhose, COPD, Hämodialyse, Diabetes, Krebs)
- `2` — Mäßig: große Bauchoperation, Schlaganfall, schwere Pneumonie, hämatologische Neoplasie
- `3` — Schwer: Schädeltrauma, Knochenmarktransplantation, Intensivstation mit APACHE II \> 10

### Alter ≥ 70 Jahre

`idade`

## Fassung der Methode

NRS 2002/ESPEN Kondrup 2003: 2 Domänen 0–3, Alter≥70 +1, gesamt 0–7

## Dokumentierte Formel

Score = beeinträchtigter Ernährungszustand (0–3) + Krankheitsschwere (0–3) + 1 Punkt bei Alter ≥70 Jahre. Gesamt 0–7.

Score ≥3: Ernährungsrisiko.

## Grenzen und Population

NRS-2002 ist ein Risikoscreening aus Ernährungszustand und Krankheitsschwere. Bei seiner Entwicklung wurden Studiengruppen mit höherer Nutzenwahrscheinlichkeit unterschieden; eine Summe garantiert kein individuelles Ansprechen und verordnet weder Applikationsweg noch Dosis der Ernährungstherapie. Definitionen, Eignung und Alter müssen zur Version passen.

## Referenzen

- [Kondrup J et al. Nutritional risk screening (NRS 2002): a new method based on an analysis of controlled clinical trials. Clin Nutr, 2003.](https://doi.org/10.1016/S0261-5614(02)00214-5)

- [Kondrup J et al. ESPEN guidelines for nutrition screening 2002. Clin Nutr, 2003.](https://doi.org/10.1016/S0261-5614(03)00098-0)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026
