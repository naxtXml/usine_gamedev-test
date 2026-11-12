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
- La nuit tombe à l'approche de chaque attaque : tes bâtiments éclairent la carte.
- Monstres volants (dès la vague 4) qui survolent les murs, stations de réparation, mini-carte et effets sonores.
- **Lanceurs de matériaux** (niv 10) : construis des bases avancées n'importe où, elles envoient leurs ressources par les airs vers un réceptionneur à côté de ton noyau.
- **5 zones** à débloquer avec les niveaux : Plaines, Désert (niv 8, cuivre), Marais (niv 15, cobalt), Toundra (niv 22, titane), Volcan (niv 30, uranium).
- Nouvelles machines (forge, centrifugeuse, éolienne, réacteur à fusion, foreuse laser, tapis express) et défenses (lance-flammes, tourelle cryo, canon électromagnétique, mur en titane, bouclier).
- Nouveaux monstres (kamikaze, blindé, guérisseur) et **4 boss** : Titan (vague 10), Reine des essaims (20), Golem de cristal (30), Dragon (40), puis le cycle recommence en plus fort.

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

## Multijoueur à deux

Bouton **Multijoueur** : l'un crée la partie et donne le code de 5 lettres, l'autre le saisit. Chacun a son noyau et son stock, vous pouvez vous donner des matériaux (clic droit sur le noyau de l'autre), réanimer le noyau tombé du coéquipier une fois la vague éliminée, et lancer la vague plus tôt si vous êtes prêts tous les deux. Vagues toutes les 15 minutes.

Les deux jeux communiquent par un relais internet gratuit (serveur MQTT public), sans compte. L'hôte garde son onglet ouvert.

### Amis

Chaque joueur a un **code ami**. Pendant une partie à deux, ajoute ton coéquipier en un clic. Ensuite, le menu Multijoueur montre qui est en ligne, permet d'**inviter** un ami (il reçoit une fenêtre « Rejoindre ») ou de **rejoindre** directement sa partie.

## Sauvegarde

La partie est sauvegardée automatiquement dans le navigateur. Le bouton **Sauvegarde** donne un code à copier pour reprendre ta partie sur un autre appareil.

## Technique

Un seul fichier `index.html` (HTML, CSS et JavaScript). Seule dépendance : [MQTT.js](https://github.com/mqttjs/MQTT.js), chargée à la demande pour le multijoueur.
