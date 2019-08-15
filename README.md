
## Description
#### quick start  
wordpress & mysql & phpMyadmin build with docker-compose

## Usage
#### container build
make a wordpress project name  
`$ mkdir { my-wordpress-dir-name }`

change directry  
`$ cd { my-wordpress-dir-name }`

container up  
`$ docker-compose up -d`  

login to Browser(your chrome or etc)  
http://localhost:8000 or http://address:8000

#### DB login
check the container status  
`$ docker-compose ps`  

login to db container  
`$ docker exec -it {my-container-name-db} /bin/bash`

check the container env  
`# env`

login to mysql(mysql_root_user)  
`# mysql -u root -p`  
Enter the password

login to mysql(mysql_user)  
`# mysql -u wordpress -p`  
Enter the password

#### login to phpMyadmin
http://localhost:8080 or http://address:8080  
username:mysql_user  
password:mysql_password

#### Network
check the network  
`$ docker network ls`  
`$ docker network inspect [Network ID or NAME]`  
