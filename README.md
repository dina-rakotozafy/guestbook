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
### Installer les dependances

```bash
composer install
yarn install
yarn build
```
## Ajouter quelques conferences:
```bash
symfony console doctrine:database:create
symfony console doctrine:migrations:migrate
symfony console doctrine:fixtures:load
```
## Lancer l'environnement de developpement et ouvrir le site dans un navigateur
```bash
docker-compose up -d
symfony serve -d
symfony open:local
```

## Lancer le test

```bash
make tests
```


