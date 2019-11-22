# WEB 0.01

**Table of Contents**

[TOCM]

Простейшая среда разработки на php включает в себя следующие компоненты:

- PHP 7.2-fpm;
- Composer
- Mysql 5.7
- Nginx 1.17
- Yarn

Install ubuntu :
------------
## docker 

	sudo apt remove docker docker-engine docker.io
	sudo apt update && sudo apt install -y apt-transport-https lsb-release ca-certificates

	wget "https://download.docker.com/linux/ubuntu/dists/disco/pool/stable/amd64/containerd.io_1.2.6-3_amd64.deb"
	wget "https://download.docker.com/linux/ubuntu/dists/disco/pool/stable/amd64/docker-ce-cli_19.03.3~3-0~ubuntu-disco_amd64.deb"
	wget "https://download.docker.com/linux/ubuntu/dists/disco/pool/stable/amd64/docker-ce_19.03.3~3-0~ubuntu-disco_amd64.deb"
	sudo dpkg -i "containerd.io_1.2.6-3_amd64.deb"
	sudo dpkg -i "docker-ce-cli_19.03.3~3-0~ubuntu-disco_amd64.deb"
	sudo dpkg -i "docker-ce_19.03.3~3-0~ubuntu-disco_amd64.deb"

## docker-compose
	sudo curl -L https://github.com/docker/compose/releases/download/1.24.0/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
	sudo chmod +x /usr/local/bin/docker-compose

# Файловая структура
-  database - «проброс» файлов бд.
-  Docker - папка в которой лежат конфигурации контейнеров
-  www - папка с проектом
-  www/db -  папка для dump.sql

# Ссылки 
`<Site>` : <http://localhost>
`<PMA>` : <http://localhost:8686>
`<Mail>` : <http://localhost:8025>

------------

# Основные команды
- docker-compose up
- docker-compose down
- docker exec -it web-php bash
- docker system prune -a
- docker system prune --volumes
- docker kill

------------
