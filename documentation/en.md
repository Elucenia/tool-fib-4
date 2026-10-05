<!-- ELUCENIA technical documentation · fib-4 · en · no clinical/professional/rights approval -->

# FIB-4 (liver fibrosis)

[conditions, sources and permissions](https://elucenia.org/en/tools/fib-4)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Age

`idade`

years · range: 18–100

### Aspartate aminotransferase (AST)

`ast`

U/L · range: 1–5000

### Alanine aminotransferase (ALT)

`alt`

U/L · range: 1–5000

### Platelets

`plq`

× 10³/mm³ · range: 5–1500

### Context

`etio`

- `masld` — Steatosis (MASLD/NAFLD)
- `viral` — Hepatitis C or HIV/HCV

## Method edition

FIB-4/Sterling 2006; HCV/HIV thresholds 1.45/3.25 versus MASLD 1.3/2.67 and age ≥65 years 2.0

## Documented formula

FIB-4 = (age × AST) ÷ (platelets \[10⁹/L\] × √ALT).

MASLD: \< 1.30 rules out advanced fibrosis (\< 2.0 from age 65); \> 2.67 suggests advanced fibrosis. Hepatitis C/HIV: \< 1.45 and \> 3.25.

## Limits and population

Sterling’s 2006 FIB-4 was developed in patients with HIV/HCV coinfection, with \<1.45 and \>3.25 cutoffs assessed against Ishak 4–6 fibrosis. The formula uses age in years, AST and ALT in U/L and platelets in 10^9/L. Those cutoffs and the original population are not automatically interchangeable with MASLD criteria or age adjustments; those variants require their own sources.

## References

- [Sterling RK et al. Development of a simple noninvasive index to predict significant fibrosis in patients with HIV/HCV coinfection. Hepatology, 2006.](https://doi.org/10.1002/hep.21178)

- [Shah AG et al. Comparison of noninvasive markers of fibrosis in patients with nonalcoholic fatty liver disease. Clin Gastroenterol Hepatol, 2009.](https://doi.org/10.1016/j.cgh.2009.05.033)

- [McPherson S et al. Age as a confounding factor for the accurate non-invasive diagnosis of advanced NAFLD fibrosis. Am J Gastroenterol, 2017.](https://doi.org/10.1038/ajg.2016.453)

- [Rinella ME et al. AASLD Practice Guidance on the clinical assessment and management of nonalcoholic fatty liver disease. Hepatology, 2023.](https://doi.org/10.1097/HEP.0000000000000323)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
