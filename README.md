# fa-playground

Set up a networked FusionAuth instance to play around with in experimetal projects.

1. `cp .env.example .env` and fill in.
2. Make sure DNS A record for $HOSTNAME is set to correct IP
3. `envsubst <http_default.template >http_default.conf`
4. docker-compose up -d

