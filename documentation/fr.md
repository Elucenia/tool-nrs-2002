<!-- ELUCENIA technical documentation · nrs-2002 · fr · no clinical/professional/rights approval -->

# NRS-2002

[conditions, sources et autorisations](https://elucenia.org/fr/outils/nrs-2002)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Altération de l’état nutritionnel

`estado`

- `0` — Absente : état nutritionnel normal
- `1` — Léger : perte de poids \> 5 % en 3 mois ou apport de 50 à 75 % des besoins la semaine précédente
- `2` — Modéré : perte \> 5 % en 2 mois, ou IMC de 18,5 à 20,5 avec état général altéré, ou apport de 25 à 60 %
- `3` — Sévère : perte \> 5 % en 1 mois (\> 15 % en 3 mois), ou IMC \< 18,5 avec état général altéré, ou apport de 0 à 25 %

### Gravité de la maladie (augmentation des besoins)

`gravidade`

- `0` — Absente : besoins nutritionnels normaux
- `1` — Léger : fracture de hanche, maladie chronique avec complication aiguë (cirrhose, BPCO, hémodialyse, diabète, cancer)
- `2` — Modérée : chirurgie abdominale majeure, AVC, pneumonie sévère, hémopathie maligne
- `3` — Sévère : traumatisme crânien, greffe de moelle osseuse, réanimation avec APACHE II \> 10

### Âge ≥ 70 ans

`idade`

## Édition de la méthode

NRS 2002/ESPEN Kondrup 2003 : 2 domaines 0–3, âge≥70 +1, total 0–7

## Formule documentée

Score = altération nutritionnelle (0–3) + gravité de maladie (0–3) + 1 point si âge ≥70 ans. Total 0–7.

Score ≥3 : risque nutritionnel.

## Limites et population

Le NRS-2002 est un dépistage du risque combinant l’état nutritionnel et la sévérité de la maladie. Son développement distinguait des groupes d’études ayant une plus forte probabilité de bénéficier d’un soutien ; un total ne garantit pas une réponse individuelle et ne prescrit ni la voie ni la dose du soutien nutritionnel. Les définitions, l’éligibilité et l’âge doivent correspondre à la version.

## Références

- [Kondrup J et al. Nutritional risk screening (NRS 2002): a new method based on an analysis of controlled clinical trials. Clin Nutr, 2003.](https://doi.org/10.1016/S0261-5614(02)00214-5)

- [Kondrup J et al. ESPEN guidelines for nutrition screening 2002. Clin Nutr, 2003.](https://doi.org/10.1016/S0261-5614(03)00098-0)

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

Aucun risque nutritionnel à ce jour

Répéter le dépistage chaque semaine ; en cas de chirurgie majeure programmée, envisager un plan nutritionnel préventif.


### 2

Patient à risque nutritionnel

Initier un plan de thérapie nutritionnelle.


### 3

Patient à risque nutritionnel

Initier un plan de thérapie nutritionnelle.

