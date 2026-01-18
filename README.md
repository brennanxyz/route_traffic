# Wraut

Pronounced "route".

### A companion to Traefik and Docker

Wraut is a CI/CD server for automatically deploying
Dockerized apps through Traefik, applying configuration
for security and route handling.

It also serves as a dashboard to view the running status
of the containers.

### System requirements

Wraut assumes that the system where it's installed
satisfies the following constraints:
1. Is a Linux system
1. Has Docker with `compose` installed
1. Has Traefik 3.5.2 running as a Docker container
  with the following settings:
  - ports 80 and 443 exposed
  - volume: `"/var/run/docker.sock:/var/run/docker.sock:ro"`

There will be some config you'll need to provide Wraut as
a `.env` file (TODO: commit the `.env.sample` and a guide to
selecting the appropriate values).
