# Usine Assiégée

Jeu de navigateur en vue du dessus : construis une usine (foreuses, tapis roulants, fonderies, assembleurs, énergie) et défends ton noyau contre des vagues de monstres toutes les 30 minutes.

**▶ Jouer :** https://naxtxml.github.io/usine_gamedev-test/

## Le principe

- Extrais des ressources (fer, quartz, or, diamant, pétrole) et transforme-les en lingots, acier, circuits, lentilles, batteries…
- Amène tout au **noyau** par tapis : c'est ton stock pour construire.
- Construis des défenses : murs, mitrailleuses, lasers, canons plasma, tours Tesla.
- Toutes les 30 minutes une vague attaque, avec un **boss** à la vague 10.
- Gagne de l'XP en tuant des monstres : tous les 5 niveaux, de nouveaux bâtiments et recettes se débloquent.
- Au niveau 20, **renais** pour gagner des points de talent permanents.

## Commandes

| Action | Touche |
|---|---|
| Poser un bâtiment | Clic (glisser pour une ligne de tapis ou de murs) |
| Démolir (remboursé) | Clic droit |
| Tourner | R |
| Choisir un bâtiment / changer de catégorie | 1 à 9 / Tab |
| Déplacer la vue | Z Q S D, flèches, ou glisser |
| Zoom | Molette |
| Pause | Espace |

## Sauvegarde

La partie est sauvegardée automatiquement dans le navigateur. Le bouton **Sauvegarde** donne un code à copier pour reprendre ta partie sur un autre appareil.

## Technique

Un seul fichier `index.html` (HTML, CSS et JavaScript, sans dépendance). Le mode multijoueur et la sauvegarde sur compte ne fonctionnent que dans la version hébergée sur claude.ai.
