# fa-playground

Set up a networked FusionAuth instance to play around with in experimetal projects.
Tested on Ubuntu 22.04 LTS server VM instance with Docker & docker-compose installed.

- Make sure DNS A record for $HOSTNAME is set to correct IP

-  `cp .env.example .env` and fill in.
 
- `sudo usermod -aG docker ${USER}`

- `(source .env; envsubst '$HOSTNAME' <http_default.template >http_default.conf)`

- `chmod 755 ./init-letsencrypt.sh; sudo ./init-letsencrypt.sh`
 
- `docker-compose up -d`
