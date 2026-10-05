<!-- ELUCENIA technical documentation · sodio-corrigido-hiperglicemia · fr · no clinical/professional/rights approval -->

# Natrémie corrigée pour l’hyperglycémie

[conditions, sources et autorisations](https://elucenia.org/fr/outils/sodio-corrigido-hiperglicemia)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Sodium mesuré

`na`

mEq/L · intervalle: 100–180

### Glycémie

`glic`

mg/dL · intervalle: 50–2000

## Édition de la méthode

Katz 1973 facteur 1,6 et Hillier 1999 facteur 2,4 pour 100 mg/dL glucose au-dessus de 100

## Formule documentée

Hillier: Na corrigé = Na + 2,4 × (glucose − 100) ÷ 100.

Katz: Na corrigé = Na + 1,6 × (glucose − 100) ÷ 100.

## Limites et population

Hillier 1999 a étudié une hyperglycémie aiguë induite chez six participants sains. La relation sodium–glucose était non linéaire, surtout au-dessus de 400 mg/dL ; le facteur moyen de 2,4 ne décrit pas avec une exactitude universelle toutes les populations et concentrations. Katz 1,6 et Hillier 2,4 sont des variantes distinctes présentées séparément. Le sodium corrigé est une estimation, pas une mesure future garantie ni une prescription de vitesse de correction.

## Références

- [Katz MA. Hyperglycemia-induced hyponatremia: calculation of expected serum sodium depression. N Engl J Med, 1973.](https://doi.org/10.1056/NEJM197310182891607)

- [Hillier TA, Abbott RD, Barrett EJ. Hyponatremia: evaluating the correction factor for hyperglycemia. Am J Med, 1999.](https://doi.org/10.1016/S0002-9343(99)00055-8)

- [https://pubmed.ncbi.nlm.nih.gov/10225241/](https://pubmed.ncbi.nlm.nih.gov/10225241/)

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
