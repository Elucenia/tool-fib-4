<!-- ELUCENIA technical documentation · fib-4 · de · no clinical/professional/rights approval -->

# FIB-4 (Leberfibrose)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/fib-4)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Alter

`idade`

Jahre · Bereich: 18–100

### Aspartat-Aminotransferase (AST/GOT)

`ast`

U/L · Bereich: 1–5000

### Alanin-Aminotransferase (ALT/GPT)

`alt`

U/L · Bereich: 1–5000

### Thrombozyten

`plq`

× 10³/mm³ · Bereich: 5–1500

### Kontext

`etio`

- `masld` — Steatose (MASLD/NAFLD)
- `viral` — Hepatitis C oder HIV/HCV

## Fassung der Methode

FIB-4/Sterling 2006; HCV/HIV-Grenzen 1,45/3,25 gegenüber MASLD 1,3/2,67 und ≥65 Jahre 2,0

## Dokumentierte Formel

FIB-4 = (Alter × AST) ÷ (Thrombozyten \[10⁹/L\] × √ALT).

MASLD: \< 1,30 schließt fortgeschrittene Fibrose aus (\< 2,0 ab 65 Jahren); \> 2,67 spricht dafür. Hepatitis C/HIV: \< 1,45 und \> 3,25.

## Grenzen und Population

FIB-4 nach Sterling 2006 wurde bei Patienten mit HIV/HCV-Koinfektion mit Schwellen \<1,45 und \>3,25 gegenüber Ishak-Fibrose 4–6 entwickelt. Die Formel verwendet Alter in Jahren, AST und ALT in U/L und Thrombozyten in 10^9/L. Diese Schwellen und die Originalpopulation sind nicht automatisch mit MASLD-Kriterien oder Altersanpassungen austauschbar; diese Varianten erfordern eigene Quellen.

## Referenzen

- [Sterling RK et al. Development of a simple noninvasive index to predict significant fibrosis in patients with HIV/HCV coinfection. Hepatology, 2006.](https://doi.org/10.1002/hep.21178)

- [Shah AG et al. Comparison of noninvasive markers of fibrosis in patients with nonalcoholic fatty liver disease. Clin Gastroenterol Hepatol, 2009.](https://doi.org/10.1016/j.cgh.2009.05.033)

- [McPherson S et al. Age as a confounding factor for the accurate non-invasive diagnosis of advanced NAFLD fibrosis. Am J Gastroenterol, 2017.](https://doi.org/10.1038/ajg.2016.453)

- [Rinella ME et al. AASLD Practice Guidance on the clinical assessment and management of nonalcoholic fatty liver disease. Hepatology, 2023.](https://doi.org/10.1097/HEP.0000000000000323)

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
