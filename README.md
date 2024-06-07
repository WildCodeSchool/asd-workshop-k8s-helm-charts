# asd-workshop-k8s-helm-charts

Cet atelier a pour objectif de te faire manipuler : 

- Kubernetes
- Helm
- Helm Charts

L'objectif final est de te faire créer et déployer une application web simple sur un cluster Kubernetes en utilisant Helm pour gérer les déploiements, les mises à jour et les rollbacks.

## Getting started

Voici les liens qui vont te permettre de démarrer : 

- [Kubernetes](https://kubernetes.io/docs/home/)
- [Helm](https://helm.sh/docs/)
- [Helm Charts](https://helm.sh/docs/topics/charts/)

Pour utiliser cet atelier, il te faut nécessairement un cluster Kubernetes sur lequel tu as les droits d'administration.

Si tu en as un à disposition alors tu peux l'utiliser sinon tu peux suivre les étapes de l'atelier et notamment celle où je te demande d'installer minikube (optionnel).

Une fois que tu te sens d'attaque, tu peux démarrer cet atelier en effectuant les tâches ci-dessous.

Bonne pratique !

## To-do

- [ ] Étape 01 : Installer Kubernetes et Minikube pour créer un cluster local (si ce n'est pas déjà fait).
- [ ] Étape 02 : Installer Helm sur ta machine.
- [ ] Étape 03 : Ajouter un repository Helm (par exemple, le repo stable) en utilisant la commande `helm repo add bitnami https://charts.bitnami.com/bitnami`.
- [ ] Étape 04 : Mettre à jour les repositories Helm en utilisant la commande `helm repo update`.
- [ ] Étape 05 : Rechercher un chart Helm (par exemple, nginx) en utilisant la commande `helm search repo nginx`.
- [ ] Étape 06 : Installer un chart Helm dans ton cluster Kubernetes en utilisant la commande `helm install my-nginx bitnami/nginx`.
- [ ] Étape 07 : Lister les releases Helm dans ton cluster en utilisant la commande `helm list`.
- [ ] Étape 08 : Mettre à jour un chart installé en utilisant la commande `helm upgrade my-nginx bitnami/nginx`.
- [ ] Étape 09 : Créer ton propre Helm Chart pour une application PHP simple.
  - Créer une page PHP simple.
  - Créer un fichier `Dockerfile` pour containeriser l'application.
  - Créer la structure de ton application.
- [ ] Étape 10 : Créer la structure de ton Helm Chart pour l'application PHP :
  ```bash
  helm create my-php-app
  ```
- [ ] Étape 11 : Adapter les fichiers générés dans le dossier `my-php-app` pour déployer ton application PHP :
  - Modifier `values.yaml` pour correspondre à ton application (ports, image Docker, etc.)
  - Mettre à jour les templates `deployment.yaml`, `service.yaml`, etc., si nécessaire.
- [ ] Étape 12 : Emballer (package) ton Helm Chart en utilisant la commande `helm package ./my-php-app`.
- [ ] Étape 13 : Déployer ton propre Helm Chart dans le cluster Kubernetes en utilisant la commande :
  ```bash
  helm install my-app ./my-php-app
  ```
- [ ] Étape 14 : Tester le déploiement de ton Helm Chart en vérifiant que l'application fonctionne correctement (par exemple, en accédant à l'application via un navigateur web).
- [ ] Étape 15 : Mettre à jour ton application en modifiant le Helm Chart et en utilisant la commande :
  ```bash
  helm upgrade my-app ./my-php-app
  ```
- [ ] Étape 16 : Revenir à une version précédente de ton application en utilisant la commande :
  ```bash
  helm rollback my-app [revision]
  ```
- [ ] Étape 17 : Supprimer un chart Helm du cluster en utilisant la commande :
  ```bash
  helm uninstall my-app
  ```
- [ ] Étape 18 : Partager ton Helm Chart en le poussant sur ce repository.

N'oublie pas de consulter la documentation officielle pour plus de détails et de bonnes pratiques.
