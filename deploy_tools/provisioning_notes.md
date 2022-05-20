Provisionamento de um novo site
===============================

## Pacotes Necessários:

* nginx
* Python 3.6
* virtualenv + pip
* Git

Por exemplo, no ubuntu:

    sudo add-apt-repository ppa:fkrull/deadsnakes
    sudo apt-get install nginx git python 3.6 python3.6-venv

## Config do Nginx Virtual Host

* Veja nginx.template.conf
* Substitua SITENAME, por exemplo, por www.violet-software-solutions.com

## Serviço Systemd

* Veja gunicorn-systemd.template.service
* Substitua SITENAME, por exemplo, por www.violet-software-solutions.com


## Estrutura das pastas:
Suponha que temos uma conta de usuário em /home/username

/home/username
    sites
        SITENAME
            database
            source
            static
            virtualenv

