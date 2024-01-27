# radicale-agendav-lldap
Deploy radicale and agendav with LLDAP

The etc/radicale folder is mandatory because I did set :
https://github.com/shroomify-it/docker-deploy_radicale-agendav-lldap/blob/6e36f91b20157bb9ccaae778c0be0c9125f0abb7/docker-compose.yml#L70 
https://github.com/shroomify-it/docker-deploy_radicale-agendav-lldap/blob/6e36f91b20157bb9ccaae778c0be0c9125f0abb7/radicaleconfig/config#L3
https://github.com/shroomify-it/docker-deploy_radicale-agendav-lldap/blob/345a0925a721b021513b15f1c2dbd3229aefb657/radicaleconfig/config#L27

I use traefik as a reverse proxy, I commented out the related traefik entries.
Don't forget to change all the CHANGEME to your environment settings.
