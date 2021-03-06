# DIY Micro Framework
A PHP minimal framework which allows you to control every bit of it.

# HOW TO USE
- Install composer globally. Do the following on a Linux. Visit [here](https://getcomposer.org/doc/00-intro.md) for windows.

```bash
$ php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
$ php -r "if (hash_file('SHA384', 'composer-setup.php') === 'e115a8dc7871f15d853148a7fbac7da27d6c0030b848d9b3dc09e2a0388afed865e6a3d6b3c0fad45c48e2b5fc1196ae') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
$ php composer-setup.php
$ php -r "unlink('composer-setup.php');"
$ mv composer.phar /usr/local/bin/composer
```

- Create a new project using composer.

```bash
$ composer create-project diy/framework [project_name] -s dev
```

- Run the config script.

```bash
$ cd [project_name] && php manage.php app:config
```

# Todo
- Customise the way mail are sent using the PHPMailer library.
- Add more custom sessionhandlers or create one that accepts any form of session store.
- Create an easy to use dashboaord for admin manipulations like in Django Framework.
- Support PHP in-built development server.
- Handle static files with nodejs' gulp library.