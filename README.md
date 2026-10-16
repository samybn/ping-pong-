# Pong Game

Un jeu de Pong en **C**, réalisé avec **raylib**. Il propose une interface à menus, des parties en solo contre une IA ou en duel local, plusieurs niveaux de difficulté, un score en temps réel et des effets sonores.

> Projet de jeu réalisé dans un cadre d’apprentissage et de pratique de la programmation en C et de raylib.

## Fonctionnalités

- Jeu de Pong en 2D dessiné avec raylib.
- Menus d’accueil, de sélection du mode et de difficulté, puis écran de résultat.
- Mode **Solo (PvE)** contre une raquette contrôlée automatiquement.
- Mode **Deux joueurs (PvP)** sur le même ordinateur.
- Quatre niveaux de difficulté en solo : **Facile**, **Moyen**, **Difficile** et **Beast**.
- Score affiché pendant la partie ; elle se termine lorsqu’un joueur atteint **11 points**.
- Rebond de la balle sur les raquettes et les limites verticales du terrain.
- Effets sonores prévus pour le fond, les rebonds, les points et la victoire.
- Fenêtre dimensionnée à partir de l’écran et boucle de jeu réglée à 100 images par seconde.

## Modes de jeu

### Solo — PvE

Le joueur contrôle la raquette de gauche. La raquette de droite suit la position de la balle grâce à un comportement automatique dont la réactivité varie selon la difficulté sélectionnée.

### Deux joueurs — PvP

Deux personnes peuvent jouer sur le même clavier : l’une contrôle la raquette de gauche, l’autre celle de droite.
 |

## Règles

- La balle est replacée sur le terrain après chaque point.
- Un point est attribué lorsque la balle dépasse l’un des côtés du terrain.
- Les rebonds sur les raquettes et les bords supérieur et inférieur sont détectés par collision.
- Le premier joueur à atteindre **11 points** remporte la partie.
- L’écran de fin indique le résultat et propose de rejouer ou de revenir au menu.

## Technologies

- **Langage :** C.
- **Bibliothèque :** [raylib](https://www.raylib.com/) pour la fenêtre, le dessin, les entrées clavier/souris, les collisions et l’audio.
- **Exécutable fourni :** version Windows.

## Structure du projet

- Pong Game.c : code source du jeu.
- Pong Game.exe : exécutable Windows fourni.
- Pong Game.o : fichier objet fourni.
- Pong-game.ico : icône du jeu.
- ressources/ : contient bounce.wav, score.wav, mute.png et test.txt.

## Compilation et lancement

### Prérequis

- Un compilateur C, par exemple GCC.
- raylib installée et configurée pour le compilateur utilisé.


### Windows avec GCC/MinGW

Depuis le dossier du projet :

    gcc "Pong Game.c" -o "Pong Game.exe" -lraylib -lopengl32 -lgdi32 -lwinmm

Lancez ensuite l’exécutable depuis le dossier contenant les ressources nécessaires.

---

Développé en C avec raylib.
