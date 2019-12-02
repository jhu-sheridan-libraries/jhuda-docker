# About
This repo contain code, configurations, documentation which enable the integration of JHUDA components for development purposes.

# Quickstart
Insure that the the DNS name `archive.local` is aliased your Docker host.

* Invoke `docker-compose pull`

* Invoke `docker-compose up -d`

Valid usernames are (password: moo):
* `depositor`
* `curator`
* `honestbroker`

# Services

* Fedora may be accessed at: https://archive.local/fcrepo/rest

# Docker Compose maintenance

* Services in `docker-compose.yml` use image tags to ensure all users are working off of the same images
* Services may be configured by environment variables in `.env`

# Image maintenance

Images are maintained in their individual repositories, and deployed using the Docker build infrastructure.  Updates to images should take place using pull requests to their respective repositories.

* Fedora: https://github.com/jhu-sheridan-libraries/jhuda-docker-fcrepo
* ActiveMQ: https://github.com/jhu-sheridan-libraries/jhuda-docker-activemq
* HTTP (SSL termination) Proxy: https://github.com/jhu-sheridan-libraries/jhuda-docker-proxy 
* IdP: https://github.com/jhu-sheridan-libraries/jhuda-docker-idp
* SP (Shib proxy): https://github.com/jhu-sheridan-libraries/jhuda-docker-sp
* LDAP: https://github.com/jhu-sheridan-libraries/jhuda-docker-ldap
* Assets: https://github.com/jhu-sheridan-libraries/jhuda-docker-assets
