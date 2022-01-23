# Variables to change

## confs/traefik.toml

* `MY_MAIL` = change w/ your email address. Useful to receive expiration notice

## docker-compose.yml

* `MY_SERVER_HTTP` : This is the name of the http router. Change it to an unique name : two containers connected to traefik must have different MY_SERVER_HTTP name.
* `MY_SERVER_HTTPS` : This is the name of the https router. Change it to an unique name : two containers connected to traefik must have different MY_SERVER_HTTPS name.
* `MY_DOMAIN` : Change to the fqdn that should bind this service. eg : `mbti.artheriom.fr`. Note that you can set multiple domain names
  * Example : Host(`artheriom.fr`) || Host(`www.artheriom.fr`)
* `MY_SERVICE_NAME` : Service name for traefik. Must be unique.

Btw, you should change the "my_server" part of the file, to make him match the container's configuration you want.