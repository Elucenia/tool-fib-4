<!-- ELUCENIA technical documentation · fib-4 · pt-BR · no clinical/professional/rights approval -->

# FIB-4 (fibrose hepática)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/fib-4)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Idade

`idade`

anos · intervalo: 18–100

### AST (TGO)

`ast`

U/L · intervalo: 1–5000

### ALT (TGP)

`alt`

U/L · intervalo: 1–5000

### Plaquetas

`plq`

× 10³/mm³ · intervalo: 5–1500

### Contexto

`etio`

- `masld` — Esteatose (MASLD/DHGNA)
- `viral` — Hepatite C ou HIV/HCV

## Edição do método

FIB 4/Sterling 2006; limiares HCV/HIV 1,45/3,25 vs MASLD 1,3/2,67 e≥65 anos 2,0

## Fórmula documentada

FIB-4 = (idade × AST) ÷ (plaquetas \[10⁹/L\] × √ALT).

MASLD: \< 1,30 exclui fibrose avançada (\< 2,0 a partir de 65 anos); \> 2,67 sugere fibrose avançada. Hepatite C/HIV: \< 1,45 e \> 3,25.

## Limites e população

O FIB-4 de Sterling 2006 foi desenvolvido em pacientes com coinfecção HIV/HCV, com cortes \<1,45 e \>3,25 avaliados contra fibrose Ishak 4–6. A fórmula usa idade em anos, AST e ALT em U/L e plaquetas em 10^9/L. Esses cortes e a população original não são intercambiáveis automaticamente com critérios MASLD ou ajustes por idade; essas variantes exigem suas próprias fontes.

## Referências

- [Sterling RK et al. Development of a simple noninvasive index to predict significant fibrosis in patients with HIV/HCV coinfection. Hepatology, 2006.](https://doi.org/10.1002/hep.21178)

- [Shah AG et al. Comparison of noninvasive markers of fibrosis in patients with nonalcoholic fatty liver disease. Clin Gastroenterol Hepatol, 2009.](https://doi.org/10.1016/j.cgh.2009.05.033)

- [McPherson S et al. Age as a confounding factor for the accurate non-invasive diagnosis of advanced NAFLD fibrosis. Am J Gastroenterol, 2017.](https://doi.org/10.1038/ajg.2016.453)

- [Rinella ME et al. AASLD Practice Guidance on the clinical assessment and management of nonalcoholic fatty liver disease. Hepatology, 2023.](https://doi.org/10.1097/HEP.0000000000000323)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

Baixa probabilidade de fibrose avançada (FIB-4 < 1,30)


### 2

Resultado indeterminado: complementar com elastografia


### 3

Resultado indeterminado: complementar com elastografia


### 4

Resultado indeterminado: complementar com elastografia

A partir de 65 anos (DHGNA/MASLD), o corte inferior usado é 2,0.


### 5

Alta probabilidade de fibrose avançada (FIB-4 > 2,67)

