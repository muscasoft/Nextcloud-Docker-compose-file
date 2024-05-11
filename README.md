***All you need for your own Nextcloud-app***

# Instruction
Place all the files in one directory and start the docker container with the following commands:
```
set -a
source .my-env
docker compose pull
docker compose up -d
```
# Available files
| Files                | Description | 
| -------------------- | --------------------------------------------------------------------------------------------------- | 
| .my-env              | your personal data like passwords and domain in this file |
| .env                 | secrets and enviroment data that is used in the docker compose file |
| nginx.conf           | configuration file for nginx |
| php-fpm-www.conf     | configuration file for php-fpm-www |
| docker-compose.yaml  | docker compose file containing a reverse-proxy (caddy), web-server (nginx), database (mariadb-database), cache manager (redis-dbcache), task scheduler (cron) and the nextcloud application all installed on Linux alpine|
