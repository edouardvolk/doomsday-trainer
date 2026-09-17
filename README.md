# Doomsday — entraînement au jour de la semaine

Entraîneur pour calculer de tête le jour de la semaine de n'importe quelle date,
avec l'algorithme Doomsday de John Conway.

**Jouer : https://edouardvolk.github.io/doomsday-trainer/**

## Ce que ça fait

- 4 modes : dates repères du mois, doomsday de l'année, date complète, mixte.
- Séries de 5 / 10 / 20 questions ou mode infini, avec chrono.
- Après chaque réponse, le calcul complet est détaillé étape par étape.
- Récapitulatif de fin de série et rejeu des seules erreurs.
- Progression conservée dans le navigateur : temps moyen par série, taux
  d'erreur par mois.
- Antisèche intégrée : ancres de siècle, dates repères, doomsday année par année.
- Plage d'années réglable (1600–2400), option « années bissextiles seulement ».
- Thème clair / sombre.

## Utilisation

Un seul fichier, aucune dépendance, fonctionne hors ligne : ouvre `index.html`
dans un navigateur.

Au clavier : `1`–`7` pour les jours, chiffres pour les quantièmes,
`Espace` affiche la réponse, `Entrée` enchaîne.

Sur mobile, les 7 jours tiennent en un écran et le bloc de réponse sert de
bouton « suivant ».

## Vérification

`index.html?selftest` recalcule toutes les dates de 1600 à 2400 et les compare à
l'objet `Date` de JavaScript.

La logique pure est isolée entre les marqueurs `LOGIC START` / `LOGIC END` dans
`index.html`, ce qui permet de l'extraire pour la tester sous Node.
