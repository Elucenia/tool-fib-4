<!-- ELUCENIA technical documentation · fib-4 · fr · no clinical/professional/rights approval -->

# FIB-4 (fibrose hépatique)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/fib-4)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Âge

`idade`

ans · intervalle: 18–100

### Aspartate aminotransférase (ASAT)

`ast`

U/L · intervalle: 1–5000

### Alanine aminotransférase (ALAT)

`alt`

U/L · intervalle: 1–5000

### Plaquettes

`plq`

× 10³/mm³ · intervalle: 5–1500

### Contexte

`etio`

- `masld` — Stéatose (MASLD/NAFLD)
- `viral` — Hépatite C ou VIH/VHC

## Édition de la méthode

FIB-4/Sterling 2006 ; seuils VHC/VIH 1,45/3,25 versus MASLD 1,3/2,67 et âge ≥65 ans 2,0

## Formule documentée

FIB-4 = (âge × AST) ÷ (plaquettes \[10⁹/L\] × √ALT).

MASLD : \< 1,30 exclut la fibrose avancée (\< 2,0 dès 65 ans) ; \> 2,67 suggère une fibrose avancée. Hépatite C/VIH : \< 1,45 et \> 3,25.

## Limites et population

Le FIB-4 de Sterling 2006 a été développé chez des patients co-infectés par le VIH et le VHC, avec des seuils \<1,45 et \>3,25 évalués par rapport à une fibrose Ishak 4–6. La formule utilise l’âge en années, l’AST et l’ALT en U/L et les plaquettes en 10^9/L. Ces seuils et cette population originale ne sont pas automatiquement interchangeables avec les critères MASLD ou les ajustements selon l’âge ; ces variantes exigent leurs propres sources.

## Références

- [Sterling RK et al. Development of a simple noninvasive index to predict significant fibrosis in patients with HIV/HCV coinfection. Hepatology, 2006.](https://doi.org/10.1002/hep.21178)

- [Shah AG et al. Comparison of noninvasive markers of fibrosis in patients with nonalcoholic fatty liver disease. Clin Gastroenterol Hepatol, 2009.](https://doi.org/10.1016/j.cgh.2009.05.033)

- [McPherson S et al. Age as a confounding factor for the accurate non-invasive diagnosis of advanced NAFLD fibrosis. Am J Gastroenterol, 2017.](https://doi.org/10.1038/ajg.2016.453)

- [Rinella ME et al. AASLD Practice Guidance on the clinical assessment and management of nonalcoholic fatty liver disease. Hepatology, 2023.](https://doi.org/10.1097/HEP.0000000000000323)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

Faible probabilité de fibrose avancée (FIB-4 < 1,30)


### 2

Résultat indéterminé : compléter par élastographie


### 3

Résultat indéterminé : compléter par élastographie


### 4

Résultat indéterminé : compléter par élastographie

À partir de 65 ans (stéatose hépatique non alcoolique/MASLD), le seuil inférieur utilisé est 2,0.


### 5

Forte probabilité de fibrose avancée (FIB-4 > 2,67)

