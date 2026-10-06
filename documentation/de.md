<!-- ELUCENIA technical documentation · sodio-corrigido-hiperglicemia · de · no clinical/professional/rights approval -->

# Natriumkorrektur bei Hyperglykämie

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/sodio-corrigido-hiperglicemia)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Gemessenes Natrium

`na`

mEq/L · Bereich: 100–180

### Blutzucker

`glic`

mg/dL · Bereich: 50–2000

## Fassung der Methode

Katz 1973 Faktor 1,6 und Hillier 1999 Faktor 2,4 je 100 mg/dL Glukose über 100

## Dokumentierte Formel

Hillier: korrigiertes Na = Na + 2,4 × (Glukose − 100) ÷ 100.

Katz: korrigiertes Na = Na + 1,6 × (Glukose − 100) ÷ 100.

## Grenzen und Population

Hillier 1999 untersuchte induzierte akute Hyperglykämie bei sechs gesunden Teilnehmenden. Die Natrium-Glukose-Beziehung war nichtlinear, besonders über 400 mg/dL; der mittlere Faktor 2,4 beschreibt nicht alle Populationen und Konzentrationen mit universeller Genauigkeit. Katz 1,6 und Hillier 2,4 sind getrennt dargestellte unterschiedliche Varianten. Korrigiertes Natrium ist eine Schätzung, keine garantierte zukünftige Messung oder Verordnung einer Korrekturgeschwindigkeit.

## Referenzen

- [Katz MA. Hyperglycemia-induced hyponatremia: calculation of expected serum sodium depression. N Engl J Med, 1973.](https://doi.org/10.1056/NEJM197310182891607)

- [Hillier TA, Abbott RD, Barrett EJ. Hyponatremia: evaluating the correction factor for hyperglycemia. Am J Med, 1999.](https://doi.org/10.1016/S0002-9343(99)00055-8)

- [https://pubmed.ncbi.nlm.nih.gov/10225241/](https://pubmed.ncbi.nlm.nih.gov/10225241/)

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

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Korrigiertes Natrium normal: die gemessene Hyponatriämie ist auf Glukose zurückzuführen (Wassertranslokation)

| Ergebnisdetails | |
| --- | --- |
| Korrigiertes Natrium (Katz, 1,6) | 138,0 mEq/L |


### 2

Echte Hyponatriämie auch nach Korrektur

| Ergebnisdetails | |
| --- | --- |
| Korrigiertes Natrium (Katz, 1,6) | 131,2 mEq/L |


### 3

Korrigiertes Natrium erhöht: es besteht ein freier Wasserdefizit

| Ergebnisdetails | |
| --- | --- |
| Korrigiertes Natrium (Katz, 1,6) | 153,2 mEq/L |

