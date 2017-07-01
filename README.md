# My PuPHPet Vagrant Config

- Ubuntu 16.04
- Apache 2.4
- MySQL 5.7
- PHP 7.1 _(cli, intl, xml, gd, mbstring, mcrypt, curl, zip, bz2)_
- PHPMyAdmin 4.7.2
- MailHog
- Xdebug

### Mapping

www/project/web will be automatically mapped to http://project.dev. No extra vhost needed.


Host file example: 

        192.168.56.101 pma.dev


### How to use

- `vagrant up`: install or starts the machine


### How to edit config:

- `vagrant provision`: reloads puphpet/config.yaml


### How to SSH

##### Automatically:
- `vagrant ssh`: ssh to vm

##### Manually:
- Host: `127.0.0.1`
- Port: `2222`
- Username: `vagrant`
- Private key: `./puphpet/files/dot/ssh/id_rsa`