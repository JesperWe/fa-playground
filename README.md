# fa-playground

Set up a networked FusionAuth instance to play around with in experimetal projects.

- Get yourself a VM instance running Ubuntu 22.04 LTS

- Install docker & docker-compose

- Set up a DNS name (A record) for the VM IP

- `cp .env.example .env` and fill in DNS hostname in HOSTNAME
 
- `sudo usermod -aG docker ${USER}`

- `(export $(grep -v '^#' .env | grep HOST |  xargs -d '\n'); envsubst '$HOSTNAME' <http_default.template >http_default.conf)`

- `chmod 755 ./init-letsencrypt.sh; sudo ./init-letsencrypt.sh`
 
- `docker-compose up -d`
