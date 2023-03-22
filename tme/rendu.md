<img src="Logo-CFAINSTA.png"
     alt="logo cfa"
     style="height: 100px; margin-left: 450px;" />

# Hébergement et rendu

Nous allons parler ici des modalités de rendu.

Cela comprends l'hébergement de l'application.

## Modalités de rendu du projet :

Barème (cf le sujet du projet).

Rendus :

- un repository git publique (pas de privé!! J'ai pas envie de devoir accepter des invitations, et vous n'avez rien à cacher) comprenant tout le code (backend et frontend).

- un fichier JSON dans ce repo à la racine appelé group.json sous cette forme :

```json
{
  "group": [
    {
      "name": "escriou",
      "firstName": "arthur"
    }, {...}// le reste du groupe
  ],
  "project": {
    "frontend": "https://url_du_front",
    "backend": "https://url_du_back",
  }
}
```

- un fichier rapport.pdf à la racine du repo également

- un user admin/admin dans la base de données de votre projet hébergé pour pouvoir tester

(Veillez à respecter les formats, je vais utiliser un script pour récupérer vos projets).

M'envoyer par mail ou discord le lien de votre repository.

## Hébergement du projet

On veut héberger notre projet mais les deux parties front et back nécessite des services différents. En effet un front n'a besoin que d'un hébergement de fichier statique alors que le backend à besoin d'une base de donnée et de ressource CPU et RAM.

On veillera à utiliser des versions gratuites ou des freetier des services ci dessous.

### Frontend

On veut un service de type CDN pour cette hébergement :

- netlify
- github pages
- gitlab pages
- firebase
- render

### Backend

Le plus simple pour l'hébergement d'un django et d'utiliser heroku : https://devcenter.heroku.com/articles/deploying-python

Pensez bien à modifier les configurations host et cors pour fonctionner avec l'URL de votre serveur et frontend déployés.

### Votre application devra être disponible en ligne pendant au moins une semaine après le rendu.
