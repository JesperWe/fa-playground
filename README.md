# fa-playground

Set up a networked FusionAuth instance to play around with in experimetal projects.
Tested on Ubuntu 22.04 LTS server VM instance with Docker & docker-compose installed.

1. `cp .env.example .env` and fill in.
2. `chmod 755 ./init-letsencrypt.sh; sudo ./init-letsencrypt.sh`
3. Make sure DNS A record for $HOSTNAME is set to correct IP
4. `envsubst <http_default.template >http_default.conf`
5`docker-compose up -d`
