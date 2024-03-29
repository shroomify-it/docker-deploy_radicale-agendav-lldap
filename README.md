# radicale-agendav-lldap
Deploy a docker stack with radicale + agendav + LLDAP

https://github.com/tomsquest/docker-radicale

https://github.com/nagimov/agendav-docker/

https://github.com/lldap/lldap

## Note about etc/radicale
In this example, the etc/radicale folder is mandatory **even if you are not using radicale's auth file and rights section**.

You can always adapt the code to not use them at all. It is aimed to make it easier if you are new to radicale by providing the folder structure.

https://github.com/shroomify-it/docker-deploy_radicale-agendav-lldap/blob/6e36f91b20157bb9ccaae778c0be0c9125f0abb7/docker-compose.yml#L70 
https://github.com/shroomify-it/docker-deploy_radicale-agendav-lldap/blob/6e36f91b20157bb9ccaae778c0be0c9125f0abb7/radicaleconfig/config#L3
https://github.com/shroomify-it/docker-deploy_radicale-agendav-lldap/blob/345a0925a721b021513b15f1c2dbd3229aefb657/radicaleconfig/config#L30

## Note about comments in the docker-compose.yml
I use traefik as a reverse proxy but I commented out the related traefik entries.

## One last thing before running docker-compose up 
Don't forget to change all the CHANGEME to your desired environment settings. Change the domain "example.domain.com" too.

You need to generate a JWT Token for LLDAP.

Files concerned by thoses changes : **docker-compose.yml** and **radicaleconfig/config**
