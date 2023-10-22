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


# Pré-requis :

Il y a quelques pré-requis pour lancer le programme (et leur lien de dl parceque des fois c'est difficile de les trouver) :
-JBcrypt (https://cdn.discordapp.com/attachments/1016290977998176287/1165261948384981043/jBCrypt-0.4.3.jar)
-Apache commons net (https://cdn.discordapp.com/attachments/626086445215645710/1165707716711428267/commons-net-3.10.0-bin.zip)
-JDBC (https://cdn.discordapp.com/attachments/1016290977998176287/1165271945613422703/mysql-connector-java-8.0.27.jar)

Voir aussi les identifiants de connexion et ip à modifier.
Si vous avez la flemme (ce que je peux comprendre, moi aussi j'ai la flemme) Ou que vous voulez voir
la totale, avec des imgaes prêtes et la base prêtes et toouuuut

Voici une VM toute prête : (g pas le lien encore)

Service | Login | Pass

Phpmyadmin | oui | oui

Machine | root | 0550002D


