# Library_HR
![developer](https://img.shields.io/badge/Developed%20By%20%3A-NISSOUL%20HAMZA%20-RED)
---
## Functions
## Client
- Le client peut afficher / rechercher des produits sans connexion.
- Le client peut également ajouter / supprimer un produit au panier sans connexion (si le client essaie d'ajouter le même produit au panier. Il n'en ajoutera qu'un)
- Lorsque le client essaie d'acheter un produit, il doit se connecter au système.
- Après avoir créé un compte et connecté au système, il / elle peut passer commande.
- Il y a aussi une page de paiement (juste pour la démo, NE REMPLISSEZ PAS LES DÉTAILS DE VOTRE CARTE, D'ailleurs, le site Web n'enregistre pas ces détails)
- Si le client clique sur le bouton de paiement, son paiement sera effectué et sa commande sera passée.
- Le client peut vérifier les détails de sa commande en cliquant sur le bouton des commandes.
- Le client peut voir l'état de la commande (en attente, confirmée, livrée) pour chaque commande
- Le client peut télécharger sa facture de commande pour chaque commande
- Le client peut envoyer des commentaires à l'administrateur (sans connexion) ---
### Admin
- Le premier administrateur se connectera (pour le nom d'utilisateur / mot de passe, exécutez la commande suivante dans cmd) ```

py manage.py createsuperuser
```
### Autres caractéristiques
- le client passe commande et l'administrateur a supprimé cet utilisateur (détection de fraude), puis ses commandes seront automatiquement supprimées 
- suppose 1 customer places 4 products order and admin deleted 2 product from website, then that 2 product order will also be deleted and other 2 will be their
- If user click on purchase button without having products in their cart, then website will ask to add product in cart first.


## COMMENT EXÉCUTER CE PROJET 
- Installez Python (3.7.6) (N'oubliez pas de cocher Ajouter au chemin lors de l'installation de Python)
- Ouvrez le terminal et exécutez les commandes suivantes: 
```
pip install django==3.0.5

pip install django-widget-tweaks

pip install xhtml2pdf

py manage.py makemigrations

py manage.py migrate

py manage.py runserver

http://127.0.0.1:8000/
