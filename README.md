# Logimmo

Logimmo c'est une appli de gestion de biens.

Chaque bien est constitué de pièces, elles mêmes constitués d'équipements.
Chaque élément peut être lier à une photo.

# COMMENT CA MARCHE ??

alors déjà, bon courage pour la lecture (s'il faut je peux vous payer un café)

Ensuite, voici le déroulement des pages :

Login gère la connexion

V

App affiche tous les biens, quand on clique sur un bien on peut en voir une preview

V

AddBien ici c'est soit pour modifier un bien, soit pour en ajouter
si c'est pour modifier, ça précharge les champs
si c'est pour ajouter, ça masque les pièces et les photos


(AddPhoto accessible de toute les pages à partir de ce stade, 
permet d'ajouter simplement une photo en FTP)

V

AddPiece agit dans le meme principe que AddBien mais pour les pieces

V

AddEquipement agit dans le meme principe que AddBien mais pour les equipements

# Les classes :

Il y a une classe par table (Piece, Photo, Biens, Equipements) Y compris pour l'autre base SQLLogException.

Ensuite il y a les controlleurs qui font le lien entre les views, les autres controlleurs et surtout :

DataBase, classe indispensable, qui gère toute les interactions avec la base
FTPManager, classe qui gère toutes les interactions en FTP, pour les photos (uploader et supprimer)
