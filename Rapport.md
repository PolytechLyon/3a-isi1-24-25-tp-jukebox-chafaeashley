# Compte Rendu TP Jukebox
## Binôme
- Ashley Padayodi 
- Chafae Qallouj
## Choix de conception et de réalisation
L'application est divisée en trois sections principales :
-Contrôleur Audio : Gère la lecture, la pause, et la progression du titre en cours. Une barre de progression interactive permet à l'utilisateur de sauter à une position spécifique dans le titre.
-Liste de Lecture : Affiche les titres ajoutés par l'utilisateur. Chaque titre est accompagné de boutons pour jouer ou supprimer le titre. Les titres en cours de lecture sont mis en évidence, et les titres défectueux sont désactivés.
-Formulaire d'Ajout : Permet d'ajouter des titres soit par lien URL, soit par fichier audio.

Fonctionnalités implémentées:
-Contrôle de lecture : Lecture, pause, et modes de répétition (Liste, Titre, Aucun).
-Barre de progression : Interactive, permet de sauter à une position spécifique dans le titre.
-Gestion des playlists : Ajout, suppression, et sélection de titres.
-Sauvegarde des titres publics : Les titres ajoutés par lien sont sauvegardés entre les rafraîchissements de la page.

Fichiers de contrôle
Pour implémenter ces fonctionnalités, nous avons principalement travaillé avec trois fichiers :
-BoiteMusicApp.vue : Ce fichier contient la logique principale de l'application, y compris la gestion des playlists, la lecture audio, et les interactions utilisateur. Il gère également les méthodes pour ajouter, supprimer, et sélectionner des titres.
-MusicPlaylist.vue : Ce fichier est responsable de l'affichage de la liste de lecture et des interactions associées, comme jouer ou supprimer un titre. Il communique avec BoiteMusicApp.vue pour mettre à jour l'état de la lecture et des playlists.
-PlaylistManager.vue : Ce fichier gère la création et la sélection des différentes listes de lecture. Il permet à l'utilisateur de naviguer entre les playlists et de les gérer (ajout, suppression).
## Difficultés rencontrées (optionnel)
-Barre de contrôle audio : La création d'une barre de progression interactive a été un défi. Nous avons dû manipuler les propriétés de l'élément <audio> pour gérer les événements de clic et mettre à jour la position de lecture.
-Gestion des playlists : Nous avons rencontré des problèmes lors de la sélection des playlists. Parfois, la playlist sélectionnée ne changeait pas correctement.
-Basculement entre les pages : Lors de la mise en place du routeur avec Vue Router, les fichiers n'ont pas été générés automatiquement. Nous avons dû créer manuellement un dossier router et un fichier 'index.js' pour gérer la navigation entre les pages.
Problème de lecture en boucle : Lorsque le mode de répétition "Liste" était activé, le lecteur ne passait pas automatiquement au titre suivant après la fin du titre en cours. 
-Animation CSS : Initialement, nous avions envisagé d'utiliser une animation CSS pour faire tourner une image pendant la lecture, mais nous n'avons pas réussi à implémenter cette fonctionnalité. Nous avons donc opté pour une image statique.
-Compréhension des fonctions JavaScript : La création et la compréhension des fonctions JavaScript, notamment celles liées à la gestion des playlists et à la lecture audio, ont été complexes. Nous avons dû revoir plusieurs fois le code pour corriger des erreurs et améliorer la fonctionnalité.
## Extensions réalisées (optionnel)
Nous avons ajouté deux extensions principales à l'application :
-Gestion des playlists : La possibilité de créer et gérer plusieurs playlists a été implémentée. Chaque playlist peut être nommée, sélectionnée ou supprimée. Nous avons utilisé Vue Router pour gérer la navigation entre ces playlists.
-Style CSS personnalisé : Pour améliorer l'apparence de l'application, nous avons ajouté des styles CSS personnalisés.
##
Ce projet nous a permis de développer nos compétences en Vue 3 et en gestion d'état dans une application web. Malgré les difficultés rencontrées, nous avons réussi à implémenter les fonctionnalités principales et à ajouter des extensions pour améliorer l'expérience utilisateur. 

