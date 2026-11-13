# TP Git/GitHub - Mon assistant de révision

## Présentation

Ce projet a été réalisé pour le TP « Publier et synchroniser un projet Python » du cours Outils collaboratifs (Git/GitHub)

Le programme est un petit assistant de révision écrit en Python. Il pose quelques questions à l'utilisateur (son prénom, la matière qu'il révise et la durée de sa séance) puis affiche un message pour l'encourager. Tout le programme se trouve dans un seul fichier, `main.py`, qui a évolué en quatre versions pendant le TP.

## Versions V1 à V4

Les quatre versions sont les états successifs du même fichier `main.py`.

 Version Ce qui a été fait :
| V1 | Création du programme en local avec un simple message de bienvenue. 
| V2 | Ajout du prénom de l'utilisateur, puis premier push vers GitHub. 
| V3 | Ajout de la matière à réviser, modifié directement sur GitHub, puis récupéré sur mon PC avec `git pull`. |
| V4 | Ajout de la durée de révision sur mon PC, puis nouveau `git push`. |

Voici le code final (V4) :

python:
print("=== Mon assistant de revision ===")
nom = input("Quel est votre prenom ? ")
print(f"Bonjour {nom} ! Bon courage pour tes revisions.")
matiere = input("Quelle matiere revises-tu ? ")
print(f"Tu revises : {matiere}.")
duree = input("Combien de minutes vas-tu reviser ? ")
print(f"Objectif : reviser {matiere} pendant {duree} minutes.")


## Comment exécuter le programme

Outils nécessaires :
- Visual Studio Code (avec l'extension Python)

Étapes pour lancer le programme dans VS Code :
1. Ouvrir le dossier "TP_Git_Python" dans VS Code (File > Open Folder).
2. Cliquer sur le fichier "main.pye".
3. Cliquer sur le bouton  "Run Python File" en haut à droite de l'éditeur. 
4. Dans le terminal intégré , répondre aux questions et valider chaque réponse.

Informations demandées à l'utilisateur :
- son prénom
- la matière qu'il révise
- la durée de révision en minutes

## Commandes Git utilisées

- `git init` : initialise un dépôt Git dans le dossier du projet.
- `git add` : prépare les fichiers modifiés pour le prochain commit.
- `git commit` : enregistre une version du projet dans l'historique, avec un message.
- `git push` : envoie mes commits locaux vers le dépôt GitHub.
- `git pull` : récupère les commits de GitHub (comme la V3) et les intègre dans mon dossier local.