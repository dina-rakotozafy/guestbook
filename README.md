# Guestbook(Livre d'or) avec Symfony

Un site pour publier des conferences.

## Cloner le projet:
```bash
git clone https://github.com/dina-rakotozafy/guestbook.git
cd guestbook
```

## Environnement de developpement

### Pre-requis:

* PHP 8.2.1
* Composer
* Symfony CLI
* Docker
* Docker-compose
* nodejs and yarn

Verifier la configuration requise(symfony) avec:

```bash
symfony check:requirements
```
### Lancer l'environnement de developpement

```bash
composer install
yarn install
yarn build
docker-compose up -d
symfony serve -d
```
## Ajouter quelques conferences:
```bash
symfony console doctrine:fixtures:load
```
## Ouvrir le site dans un navigateur
```bash
symfony open:local
```

## Lancer le test

```bash
make tests
```


