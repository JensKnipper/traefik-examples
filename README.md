# Traefik Examples

This repository covers basic examples for using [Traefik](https://traefik.io) and Docker. All examples can be executed locally, which allows easy testing and adjusting to your own needs.  
The examples are primarily used in my blog [blog.jensknipper.de](https://blog.jensknipper.de) to show and explain the code in the articles.  
Feel free to open tickets or merge requests if you think something is missing.  

## Overview

### Dashboard

#### Expose Traefik Dashboard to Subdomain
- [Example code](dashboard/expose-traefik-dashboard-to-subdomain/docker-compose.yml)

#### Secure Traefik Dashboard
- [Example code](dashboard/secure-traefik-dashboard/docker-compose.yml)

### Logging

#### Enable Logging
- [Example code](logging/enable-logging/docker-compose.yml)

#### Enable Access Logging
- [Example code](logging/enable-access-logging/docker-compose.yml)

### Redirects

#### HTTP to HTTPS redirect

##### Global HTTP to HTTPS redirect
- [Article](https://blog.jensknipper.de/blog/traefik-http-to-https-redirect/#global-http-to-https-redirect)
- [Example code](redirects/http-to-https-redirect/http-redirect-global/docker-compose.yml)

##### Per Domain HTTP to HTTPS redirect
- [Article](https://blog.jensknipper.de/blog/traefik-http-to-https-redirect/#per-domain-http-to-https-redirect)
- [Example code](redirects/http-to-https-redirect/http-redirect-per-domain/docker-compose.yml)

#### HTTP to HTTPS and with www redirect

##### Global HTTP to HTTPS and www to non-www redirect
- [Example code](redirects/http-to-https-with-www-redirect/global-www-to-non-www-https-redirect/docker-compose.yml)

#### Redirect to external url
- [Example code](redirects/redirect-to-external-url/docker-compose.yml)

#### Redirect to subdomain
- [Example code](redirects/subdomain-redirect/docker-compose.yml)

### SSL

#### Auto-SSL with Let's Encrypt

##### Auto-SSL with HTTP-Challenge (NOT WORKING LOCALLY!)
- [Example code](ssl/auto-ssl/http-challenge/docker-compose.yml)


## Upcoming Topics
- https and www redirect - www to non-www version
- https and www redirect - per service
- auto-ssl dns challenge
- ssl including own (wildcard) certificate