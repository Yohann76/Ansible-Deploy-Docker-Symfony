"# Ansible-Deploy-Docker-Symfony" 

## Technology 

This architecture proposes a reutilisable code and easy to maintain. It also provides good practice like MVC layout and object oriented.

This application works with the symfony framework ( 5.0.5 ).

- Symfony
- Docker ( configure your environment)
- Ansible ( deploy with ansible folder)

for now, the application is deployed on a raspberry (local IP in Ansible)

### Use this project 

-  clone this project on your environment 
-  configure your variable environment
-  run `composer install`
-  run `php bin/console d:d:c`
-  run `php bin/console d:m:m`
-  run `php bin/console d:f:l -n`

-  You can run this project with docker containers ( docker-compose included in this repository )

##### For Docker run :

run this project with docker containers (docker-compose included in this repository )
```
docker-compose up -d
```
## Deployment

##### For Ansible, create your ansible/hosts.ini and run:
```
ansible-playbook ansible/playbook.yml -i ansible/hosts.ini --ask-vault-pass
```

if you want to modify this project,
the following links you may be useful

1. https://symfony.com/doc/current/index.html#gsc.tab=0
2. https://www.docker.com/
3. https://docs.ansible.com/ansible/latest/index.html

## Other information 

Standard :
1. PSR2 ( https://www.php-fig.org/psr/psr-2/ )
