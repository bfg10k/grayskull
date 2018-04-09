# GraySkull 

Skeleton proyect PHP-FPM-APACHE with docker

- Create ssh keys

``` 
example:
ssh-keygen -f ./id_rsa -C www-data@grayskull
```

- Incluir en /etc/hosts: 127.0.0.1  grayskull.local grayskull-gestion.local
- mkdir -p ~/NAS/grayskull  //para crear NAS en la Home del usuario
- mkdir /home/$USER/.composer para cache de composer
- sudo setfacl -R -m u:www-data:rwx -m u:`whoami`:rwx var/cache var/logs
- sudo setfacl -dR -m u:www-data:rwx -m u:`whoami`:rwx var/cache var/logs
- chmod 600 ./docker/ssh/id_rsa
