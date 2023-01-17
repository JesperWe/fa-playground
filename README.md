# fa-playground

Set up a networked FusionAuth instance to play around with in experimetal projects.
Tested on Ubuntu 22.04 LTS server VM instance with Docker & docker-compose installed.

-  `cp .env.example .env` and fill in.
 
- `sudo usermod -aG docker ${USER}`

- `envsubst <http_default.template >http_default.conf`

- `chmod 755 ./init-letsencrypt.sh; sudo ./init-letsencrypt.sh`
 
- Make sure DNS A record for $HOSTNAME is set to correct IP

- `docker-compose up -d`
