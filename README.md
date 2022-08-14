# Traefik Examples

This repository covers basic examples for using [Traefik](https://traefik.io) and Docker. All examples can be executed locally, which allows easy testing and adjusting to your own needs.  
A lot of these examples are explained in detail in my blog: [jensknipper.de](https://jensknipper.de). In case you are running in some problems or need some background information you should take a look at these articles.

For the purpose of simpler declaration I will not make use of configuration files, but only use docker labels.

Feel free to open tickets or merge requests if you think something is missing.  

## Overview

### Authentication

#### Basic Authentication - e.g. secure Traefik dashboard
- [Article](https://jensknipper.de/blog/basic-authentication-with-traefik)
- [Example code](authentication/basic-authentication/docker-compose.yml)

### Dashboard

#### Expose Traefik Dashboard to Subdomain
- [Article](https://jensknipper.de/blog/exposing-traefik-dashboard/)
- [Example code](dashboard/expose-traefik-dashboard-to-subdomain/docker-compose.yml)

### Logging

#### Enable Logging
- [Example code](logging/enable-logging/docker-compose.yml)
- [Article](https://jensknipper.de/blog/traefik-logging#logging)

#### Enable Access Logging
- [Example code](logging/enable-access-logging/docker-compose.yml)
- [Article](https://jensknipper.de/blog/traefik-logging#activate-access-logging)

### Ports

#### Additional entrypoint
- [Example code](ports/additional-entrypoint/docker-compose.yml)

#### Serve non HTTP/HTTPS ports
- [Example code](ports/serve-non-http-ports/docker-compose.yml)

### Redirects

#### HTTP to HTTPS redirect

##### Global HTTP to HTTPS redirect
- [Article](https://jensknipper.de/blog/traefik-http-to-https-redirect#global-http-to-https-redirect)
- [Example code](redirects/http-to-https-redirect/http-redirect-global/docker-compose.yml)

##### Per Domain HTTP to HTTPS redirect
- [Article](https://jensknipper.de/blog/traefik-http-to-https-redirect#per-domain-http-to-https-redirect)
- [Example code](redirects/http-to-https-redirect/http-redirect-per-domain/docker-compose.yml)

#### HTTP to HTTPS and with www redirect

##### Global HTTP to HTTPS and www to non-www redirect
- [Example code](redirects/http-to-https-with-www-redirect/global-www-to-non-www-https-redirect/docker-compose.yml)

#### Redirect to external url
- [Article](https://jensknipper.de/blog/traefik-redirect-to-external-domain/)
- [Example code](redirects/redirect-to-external-url/docker-compose.yml)

#### Redirect to subdomain
- [Example code](redirects/subdomain-redirect/docker-compose.yml)

### Reverse Proxy
- [Example code](reverse-proxy/docker-compose.yml)

### SSL

#### Auto-SSL with Let's Encrypt

##### Auto-SSL with HTTP-Challenge (NOT WORKING LOCALLY!)
- [Example code](ssl/auto-ssl/http-challenge/docker-compose.yml)


## Upcoming Topics
- https and www redirect - www to non-www version
- https and www redirect - per service
- auto-ssl dns challenge
- ssl including own (wildcard) certificate
- digest auth
- rate limiting
- load balancing
- port instead of domain
