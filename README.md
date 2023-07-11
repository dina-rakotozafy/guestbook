# Guestbook(Livre d'or) avec Symfony

Un site pour publier des conferences.

## Environnement de devoleppement

### Pre-requis

* PHP 8.2.1
* Composer
* Symfony CLI
* Docker
* Docker-compose
* nodejs and yarn

Verifier la configuration requise avec:

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

## Lancer le test

```bash
make tests
```


php -d xdebug.mode=coverage bin/phpunit --coverage-html var/log/test/test-coverage

