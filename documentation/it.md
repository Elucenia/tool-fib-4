<!-- ELUCENIA technical documentation · fib-4 · it · no clinical/professional/rights approval -->

# FIB-4 (fibrosi epatica)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/fib-4)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Età

`idade`

anni · intervallo: 18–100

### Aspartato aminotransferasi (AST)

`ast`

U/L · intervallo: 1–5000

### Alanina aminotransferasi (ALT)

`alt`

U/L · intervallo: 1–5000

### Piastrine

`plq`

× 10³/mm³ · intervallo: 5–1500

### Contesto

`etio`

- `masld` — Steatosi (MASLD/NAFLD)
- `viral` — Epatite C o HIV/HCV

## Edizione del metodo

FIB-4/Sterling 2006; soglie HCV/HIV 1,45/3,25 rispetto a MASLD 1,3/2,67 e ≥65 anni 2,0

## Formula documentata

FIB-4 = (età × AST) ÷ (piastrine \[10⁹/L\] × √ALT).

MASLD: \< 1,30 esclude fibrosi avanzata (\< 2,0 da 65 anni); \> 2,67 suggerisce fibrosi avanzata. Epatite C/HIV: \< 1,45 e \> 3,25.

## Limiti e popolazione

Il FIB-4 di Sterling 2006 è stato sviluppato in pazienti con coinfezione HIV/HCV, con soglie \<1,45 e \>3,25 valutate rispetto alla fibrosi Ishak 4–6. La formula usa età in anni, AST e ALT in U/L e piastrine in 10^9/L. Queste soglie e la popolazione originale non sono automaticamente intercambiabili con i criteri MASLD o gli aggiustamenti per età; tali varianti richiedono fonti proprie.

## Riferimenti

- [Sterling RK et al. Development of a simple noninvasive index to predict significant fibrosis in patients with HIV/HCV coinfection. Hepatology, 2006.](https://doi.org/10.1002/hep.21178)

- [Shah AG et al. Comparison of noninvasive markers of fibrosis in patients with nonalcoholic fatty liver disease. Clin Gastroenterol Hepatol, 2009.](https://doi.org/10.1016/j.cgh.2009.05.033)

- [McPherson S et al. Age as a confounding factor for the accurate non-invasive diagnosis of advanced NAFLD fibrosis. Am J Gastroenterol, 2017.](https://doi.org/10.1038/ajg.2016.453)

- [Rinella ME et al. AASLD Practice Guidance on the clinical assessment and management of nonalcoholic fatty liver disease. Hepatology, 2023.](https://doi.org/10.1097/HEP.0000000000000323)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Bassa probabilità di fibrosi avanzata (FIB-4 < 1,30)


### 2

Risultato indeterminato: integrare con elastografia


### 3

Risultato indeterminato: integrare con elastografia


### 4

Risultato indeterminato: integrare con elastografia

A partire dai 65 anni (NAFLD/MASLD), il cut-off inferiore utilizzato è 2,0.


### 5

Alta probabilità di fibrosi avanzata (FIB-4 > 2,67)

