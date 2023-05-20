
# Cahier des charges - Déploiement d'une infrastructure Kubernetes sur AKS avec scaling horizontal
## Objectif

Le but de ce projet est de déployer une infrastructure Kubernetes sur Azure Kubernetes Service (AKS) en utilisant Terraform et Helm. L'infrastructure déployée devra permettre le scaling horizontal des ressources. Ensuite, nous devrons déployer les services suivants sur Kubernetes : GitLab, Rocket.Chat, n8n, Prometheus et Grafana. GitLab sera utilisé pour mettre en place une intégration continue et un déploiement continu (CI/CD) pour les autres services.

## Infrastructure Kubernetes sur AKS

Nous utiliserons Terraform pour déployer l'infrastructure Kubernetes sur AKS. Les principales fonctionnalités de cette infrastructure seront les suivantes :

- Mise en place d'un cluster Kubernetes sur AKS.
- Configuration de l'autoscaling horizontal pour les nœuds du cluster afin d'ajuster automatiquement les ressources en fonction de la charge.
- Configuration de la haute disponibilité pour assurer la résilience du cluster.

## Déploiement des services sur Kubernetes

Nous utiliserons Helm pour déployer les services suivants sur le cluster Kubernetes :

### GitLab

GitLab sera déployé en tant que service principal pour gérer le code source, les dépôts et les pipelines CI/CD. Les fonctionnalités suivantes devront être prises en compte :

- Déploiement de GitLab en utilisant les meilleures pratiques recommandées.
- Configuration des connexions sécurisées et de l'accès au code source.
- Configuration des règles d'accès et des autorisations pour les utilisateurs.

### Rocket.Chat

Rocket.Chat sera déployé sur Kubernetes en utilisant les images de conteneur disponibles. Les points clés à considérer sont les suivants :

- Configuration de l'évolutivité horizontale pour Rocket.Chat afin de gérer la charge.
- Configuration des paramètres de connexion et d'accès sécurisés.
- Intégration avec n8n pour la mise en place d'un système de notification.

### n8n

n8n sera déployé sur Kubernetes pour permettre l'automatisation et l'orchestration des flux de travail. Les aspects importants à prendre en compte sont les suivants :

- Configuration de l'évolutivité horizontale pour n8n afin de gérer les demandes de flux de travail.
- Configuration des paramètres de connexion et d'accès sécurisés.
- Intégration avec Rocket.Chat pour la notification des événements.

### Prometheus et Grafana

Prometheus sera déployé pour la collecte de métriques et la surveillance de l'infrastructure Kubernetes. Grafana sera utilisé pour visualiser les données collectées par Prometheus. Les tâches suivantes devront être effectuées :

- Déploiement de Prometheus et Grafana en utilisant les meilleures pratiques recommandées.
- Configuration de la collecte de métriques pour Kubernetes et les services déployés.
- Configuration des tableaux de bord personnalisés dans Grafana pour la supervision.

## Livrables attendus

À la fin du projet, les livrables suivants devront être fournis :

- Code Terraform pour le déploiement de l'infrastructure Kubernetes sur AKS.
- Fichiers Helm Chart pour le déploiement des services (GitLab, Rocket.Chat, n8n, Prometheus, Grafana) sur Kubernetes.
- Documentation décrivant les étapes de déploiement et de configuration.Cahier des charges - Déploiement d'une infrastructure Kubernetes sur AKS avec scaling horizontal

