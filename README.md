# Projet VR
## Jeu du Serveur (Tristan VL)

### Description
Jeu du Serveur est un jeu d'adresse et de concentration où le but est de ne pas faire tomber la bille que tu contrôles, tout en tenant jusqu'à ce que toutes les balles adverses aient été tirées.

### Règles du jeu

Objectif : Garder ta bille en équilibre le plus longtemps possible.
Fin de partie : La partie se termine quand toutes les balles ont été tirées ou si ta bille tombe.

### Problèmes rencontrés

Œillères de réflexion : Certaines limitations dans la conception initiale ont pu influencer les choix techniques ou créatifs.
(Aucun autre problème majeur à signaler pour l'instant.)

### Comment jouer ?

Attrapez le plateau puis esquivez.

## Jeu de tire à l'arc (Hugo Magnier)

### Description
Une 'simulation' de tire à l'arc dans laquelle le joueur peut expérimenté avec un arc et des flèches. Des cible sont aussi mise à disposition pour tester son aim.

### Comment Jouer
- Les arcs ainsi que les flèches peuvent être grab de manière normal.
- En tenant un arc, une flèche peut être insérer en la droppant en ayant la main qui la tien au niveau de l'arc.
- Une flèche insérer dans un arc peut être tiré en tenant l'arc dans une main et en grabbant le bout de la flèche puis en tirant en arrière (une jauge de force se remplira) et en lachant.

### Problèmes rencontrés
- Collision entre la flèche et l'arc au moment du tiré de la flèche

## Jeu de BeatSaber (Léo Guillemart)

### Description
Une reproduction du jeu beatsaber avec un scope réduit, proposant des sabres associés à une couleur, un score et un temps de jeu maximum défini à 60 secondes.

### Comment Jouer
- La partie débute à la prise en main de l'un des deux sabres.
- Dès lors, des cubes de deux couleurs différentes arrivent vers le joueur à un interval régulier.
- Tout les cubes qui sont détruit font gagner un point de score au joueur, tout les cubes qui sont ratés font perdre un point de score au joueur. La partie se termine au bout de 60 secondes

### Problèmes rencontrés
- La gestion du gameplay se fait principal par les sabres qui font office de game manager. Appliquer cette logique n'était pas évidente au début.

## Jeu de tire au sniper (Axami Mohamed)

### Description
Une 'simulation' de tire au sniper dans laquelle le joueur peut expérimenter des tirs su sniper ainsi qu'un rechargement manuelle entre chaque tirs.

### Comment Jouer
- Le sniper et le levier permettant le rechargement peuvent être grab de manière normal.
-Entre chaque tir, l’utilisateur doit recharger son arme en effectuant le mouvement caractéristique d’un fusil de précision : tirer le levier vers l’arrière puis le ramener vers l’avant. Ce mouvement permet d’éjecter la douille usagée de la chambre et de préparer l’arme pour le tir suivant.

### Problèmes rencontrés
- Interaction a deux main sur un même Object

## Jeu d'escalade (Ruben PIRES)
Description
Une "simulation" d'escalade dans laquelle le joueur peut escalader des murs en s'agrippant à des accroches avec ses deux mains. Il a également le pouvoir de se propulser dans les airs à l'aide de la force de ses bras. De plus, il est limité par une barre de stamina pour chacune de ses mains, ce qui nécessite une grande rapidité d'exécution.

### Comment Jouer
Lorsque le joueur s'approche d'accroches fixées sur les murs, il peut s'y agripper avec chacune de ses mains.
Dès qu'il attrape une accroche, une barre de stamina s'affiche sur sa main, indiquant ce qu'il lui reste d'énergie avant de lâcher prise automatiquement. Il peut relâcher l'accroche pour que sa stamina remonte.
De plus, le joueur peut se jeter dans les airs à l'aide des accroches : si le joueur amorce un mouvement et relâche l'accroche au dernier moment, il sera propulsé dans les airs dans la direction souhaitée.
Le but est d'aller tout en haut de la tour.

### Problèmes rencontrés
Erreur lors du calcul de la vélocité du joueur (angle erroné et inversé). De plus, la vélocité me balançait contre le mur et la force continuait de m'attirer vers celui-ci, mais le sweep (détection de collision) empêchait le joueur de continuer au travers. Par conséquent, la vélocité me laissait complètement bloqué contre le mur.
