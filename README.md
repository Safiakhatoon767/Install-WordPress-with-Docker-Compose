# Install-WordPress-with-Docker-Compose
An organization XYZ private limited is developing a blogging platform using WordPress and MySQL they have containerized their application now they are seeking your help in writing a docker-compose file to manage both the application together

Step 1: Installing Docker Engine:

apt-get install apt-transport-https curl ca-certificates curl software-properties-common -y

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | apt-key add -

add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable" 

apt-get install docker-ce -y

docker --version

Step 2: Installing Docker Compose:

curl -L https://github.com/docker/compose/releases/download/1.29.2/docker-compose-Linux-x86_64 -o /usr/local/bin/docker-compose

chmod +x /usr/local/bin/docker-compose

docker-compose --version

Step 3: Setting Up YML File:

mkdir wordpress

cd wordpress

vim docker-compose.yml

Step 4: Building WordPress Container:

docker-compose up -d

docker-compose images

docker-compose ps

docker-compose logs wordpress

docker-compose logs database

Step 5: Getting Access to WordPress Website:

http://your-server-ip
