# jenkins docker-compose
To use the external volume, it must exist before docker-compose is run. Docker-compose will not create it itself (but you can change it to use an internal volume, which it will create).

docker-compose uses a project name and it prepends it to names. By default it’s the directory name which prevents collisions with existing containers. -p can be used to change it but it can't be blank.
