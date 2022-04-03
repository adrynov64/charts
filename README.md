# TP5-charts

Ce chart à pour objectif de déployer un serveur web et une base de donnée mariadb avec des volumes partagés.
Tous les noms utilisent celui du chart lors de l'installation.

# Soucis
Au début ça marchait mais mtn il n'y a plus de synchro entre gh-pages et main.

# Prérequis

Installer Minikube (et Docker, kubectl, helm)

## Executer : 
1.minikube start

2.minikube addons enable ingress

3.minikube tunnel (pour le loadbalencer)

4.echo "192.168.49.2 deno.minikube" | sudo tee -a /etc/hosts
L'adresse IP est défini par la commande : minikube ip

Suivre NOTES.txt après l'installaiton.

# Usage
git clone git@github.com:adrynov64/tp4-charts.git


helm install my-chart .

my-chart = nom à choisir

## helm upgrade 

Incrémenter la valeur de version du Chart.yaml :

helm upgrade my-chart . --install

# Images Docker

https://hub.docker.com/_/mariadb

https://hub.docker.com/r/codebuds/deno-webserver

# Github pages

https://adrynov64.github.io/tp4-charts/


