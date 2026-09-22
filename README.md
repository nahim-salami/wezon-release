# Wézon · chaîne de compilation

Ce dépôt **ne contient aucun code applicatif**. Il contient trois fichiers
de configuration qui compilent et publient l'application mobile Wézon, dont
le code vit dans un dépôt privé.

Pourquoi séparer : les machines d'intégration sont gratuites pour un dépôt
public, et le code n'a pas à l'être. Le code est cloné dans la machine
d'exécution, compilé, puis la machine est détruite.

- `init-platforms.yml` génère les dossiers Android et iOS d'un projet
  Flutter neuf. Il n'accède à rien de privé.
- `check.yml` analyse et teste le code privé.
- `release-android.yml` et `release-ios.yml` signent et publient.

Wézon est un service de Ahime, Abomey-Calavi, Bénin.
https://wezon.ahime.net
