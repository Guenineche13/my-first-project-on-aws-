


Projet Hébergement Site Statique AWS S3 avec CI/CD GitHub

1. Création du site

On fait un petit site web fichier text sans base de donnée 

Il n’y a pas de serveur compliqué, juste des pages simples.

2. Hébergement sur S3 (Amazon)

On crée un “bucket” S3, qui est comme un dossier sur internet.

On met notre site dedans et on le rend accessible sur internet.

La page principale s’appelle index.html.

3. Sécurité du bucket

Les gens peuvent seulement lire le site, ils ne peuvent rien modifier.

C’est sécurisé, personne ne peut supprimer ou changer nos fichiers.

4. Utilisateur spécial pour GitHub

On crée un compte spécial (IAM) pour mettre à jour le site automatiquement.

Ce compte peut seulement ajouter, supprimer ou lister les fichiers du site.

Il ne peut rien faire d’autre pour plus de sécurité.

5. Déploiement automatique avec GitHub Actions

Chaque fois qu’on change le site dans GitHub, le site se met à jour automatiquement sur S3.

GitHub utilise des codes secrets pour se connecter à Amazon.

La commande principale copie les fichiers du site sur S3 et supprime ceux qui ne sont plus utilisés.

6. Vérification

On regarde si le site fonctionne bien.

On vérifie que tout est sécurisé et accessible au public.

Résultat final

Site web en ligne
Mise à jour automatique quand on change quelque chose dans GitHub.

Site sécurisé et disponible pour tout le monde.



## Vidéo de démonstration

Voici une vidéo qui montre que mon projet fonctionne bien :  
[Voir la vidéo ici](https://drive.google.com/file/d/1jaGdij7iAg3uLPDz97n4vS-a7tlA2PQB/view?usp=sharing)

