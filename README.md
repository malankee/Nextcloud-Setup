Install Docker
$curl -sSL https://get.docker.com/ | CHANNEL=stable sh
$sudo systemctl enable docker
$sudo systemctl start docker

Install Docker Compose
$sudo curl -L "https://github.com/docker/compose/releases/download/1.25.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

Install Nextcloud
$docker network create nextcloud_network

Edit the docker compose file 
$vim docker-compose.yml

Start everything up
$docker-compose up -d
