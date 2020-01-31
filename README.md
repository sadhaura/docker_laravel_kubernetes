                                  Laravel App built with Docker Compose and kubernetes

For Docker:-

Enviroments:-
. Mysql5.7
. phpmyadmin
. php:7.2.10-apache-stretch

Installation:-
Clone this repository on your local computer. 


1. git clone https://github.com/sadhaura/docker_laravel_kubernetes.git

2. cd docker_laravel

3. docker-compose up -d

and run the command below

Your Laravel App is now ready!! You can access it via http://localhost:9004.

You can access phpmyadmin via http://localhost:9005 with username root and password secret


For Kubernetes:-

Requirements:-
you must have kubernetes cluster up and running:-


1. Clone the repository on kubernetes cluster

git clone https://github.com/sadhaura/docker_laravel_kubernetes.git

2. cd docker_laravel_kubernetes/kubernetes

3. run the below command 

kubectl create -f apache.yml,configmap.yml,secret.yml,mysql.yml,volume.yml

4. Your kubernetes deployments,pods,service will be up and running with persistent storage for database.

You can check access your website with EXTERNAL IP of kubernetes service(my-laravel-server).

 

