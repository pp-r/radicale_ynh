# Radicale pour YunoHost

[![Niveau d'intégration](https://dash.yunohost.org/integration/radicale.svg)](https://dash.yunohost.org/appci/app/radicale) ![](https://ci-apps.yunohost.org/ci/badges/radicale.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/radicale.maintain.svg)  
[![Installer Radicale avec YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=radicale)

*[Read this readme in english.](./README.md)*
*[Lire ce readme en français.](./README_fr.md)*

> *Ce package vous permet d'installer Radicale rapidement et simplement sur un serveur YunoHost.
Si vous n'avez pas YunoHost, regardez [ici](https://yunohost.org/#/install) pour savoir comment l'installer et en profiter.*

## Vue d'ensemble

Radicale est un petit mais puissant serveur CalDAV (calendriers, listes de tâches) et CardDAV (contacts).


**Version incluse :** 1.1.6~ynh6



## Avertissements / informations importantes

## Configuration

Utilisez le fichier `/etc/radicale/config` pour modifier la configuration principale de radicale.
Le fichier `/etc/radicale/logging` pour changer le niveau de journalisation.
Et le fichier `/etc/radicale/rights` pour éditer la façon dont les calendriers seront partagés.

InfCloud a son propre fichier de config, à /var/www/radicale/infcloud/config.js

## Fonctionnalités spécifiques à YunoHost

* Ce package propose une interface web pour radicale nommée InfCloud.

#### Support multi-utilisateurs

Supportée, avec LDAP et SSO seulement avec radicale, pas pour InfCloud.

## Limitations

* La version 1.1.6 est relativement ancienne. Il existe une version 2 de radicale, mais cette nouvelle version ne supporte pas encore ldap.

## Documentations et ressources

* Site officiel de l'app : http://radicale.org
* Documentation officielle de l'admin : https://github.com/Kozea/Radicale/blob/website/pages/user_documentation.rst
* Dépôt de code officiel de l'app : https://github.com/Kozea/Radicale
* Documentation YunoHost pour cette app : https://yunohost.org/app_radicale
* Signaler un bug : https://github.com/YunoHost-Apps/radicale_ynh/issues

## Informations pour les développeurs

Merci de faire vos pull request sur la [branche testing](https://github.com/YunoHost-Apps/radicale_ynh/tree/testing).

Pour essayer la branche testing, procédez comme suit.
```
sudo yunohost app install https://github.com/YunoHost-Apps/radicale_ynh/tree/testing --debug
ou
sudo yunohost app upgrade radicale -u https://github.com/YunoHost-Apps/radicale_ynh/tree/testing --debug
```

**Plus d'infos sur le packaging d'applications :** https://yunohost.org/packaging_apps