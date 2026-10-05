<!-- ELUCENIA technical documentation · fib-4 · es · no clinical/professional/rights approval -->

# FIB-4 (fibrosis hepática)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/fib-4)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Edad

`idade`

años · intervalo: 18–100

### Aspartato aminotransferasa (AST)

`ast`

U/L · intervalo: 1–5000

### Alanina aminotransferasa (ALT)

`alt`

U/L · intervalo: 1–5000

### Plaquetas

`plq`

× 10³/mm³ · intervalo: 5–1500

### Contexto

`etio`

- `masld` — Esteatosis (MASLD/EHGNA)
- `viral` — Hepatitis C o VIH/VHC

## Edición del método

FIB-4/Sterling 2006; umbrales VHC/VIH 1,45/3,25 frente a MASLD 1,3/2,67 y ≥65 años 2,0

## Fórmula documentada

FIB-4 = (edad × AST) ÷ (plaquetas \[10⁹/L\] × √ALT).

MASLD: \< 1,30 excluye fibrosis avanzada (\< 2,0 desde 65 años); \> 2,67 sugiere fibrosis avanzada. Hepatitis C/VIH: \< 1,45 y \> 3,25.

## Límites y población

El FIB-4 de Sterling 2006 se desarrolló en pacientes con coinfección VIH/VHC, con puntos de corte \<1,45 y \>3,25 evaluados frente a fibrosis Ishak 4–6. La fórmula utiliza edad en años, AST y ALT en U/L y plaquetas en 10^9/L. Esos puntos de corte y la población original no son automáticamente intercambiables con criterios MASLD o ajustes por edad; dichas variantes requieren fuentes propias.

## Referencias

- [Sterling RK et al. Development of a simple noninvasive index to predict significant fibrosis in patients with HIV/HCV coinfection. Hepatology, 2006.](https://doi.org/10.1002/hep.21178)

- [Shah AG et al. Comparison of noninvasive markers of fibrosis in patients with nonalcoholic fatty liver disease. Clin Gastroenterol Hepatol, 2009.](https://doi.org/10.1016/j.cgh.2009.05.033)

- [McPherson S et al. Age as a confounding factor for the accurate non-invasive diagnosis of advanced NAFLD fibrosis. Am J Gastroenterol, 2017.](https://doi.org/10.1038/ajg.2016.453)

- [Rinella ME et al. AASLD Practice Guidance on the clinical assessment and management of nonalcoholic fatty liver disease. Hepatology, 2023.](https://doi.org/10.1097/HEP.0000000000000323)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
