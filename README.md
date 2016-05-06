# symfony-formation

You need Vagrant and Virtual Box to run the virtual machine

## Install packages manually

```bash
sudo apt-get install php5 php5-fpm php5-mysql php5-pgsql php5-mcrypt php5-cli php5-common php5-curl php5-dev php5-gd php5-ldap php-apc php5-intl
```

## Install symfony

```bash
sudo curl -LsS https://symfony.com/installer -o /usr/local/bin/symfony
sudo chmod a+x /usr/local/bin/symfony
cd /var/www/symfony-formation/current
symfony new symfony-formation
```

## Run Symfony built-in webserver

```bash
cd symfony-formation
php bin/console server:start 0.0.0.0:8000
```
